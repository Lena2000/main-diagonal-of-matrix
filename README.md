# main-diagonal-of-matrix
Ввод элементов квадратной матрицы. Вывод элементов главной диагонали матрицы. Вывод положительных элементов над главной диагональю матрицы. Вывод суммы этих положительных элементов.
package двумер.задание1;

import java.util.Scanner;

/**
 *
 * @author LENOVO
 */
public class ДвумерЗадание1 {

    /**
     * @param args the command line arguments
     */
    public static void main(String[] args) {
        Scanner sc= new Scanner(System.in);
        System.out.println("введите размер квадратной матрицы: ");
        int n=sc.nextInt(); 
        int m=n*n;
        System.out.println("Введите "+m+" элементов матрицы");
        int i;
        int j;
        int[][] mas = new int[n][n];
        for ( i=0; i<n; i++){
         for( j=0; j<n; j++){
          mas[i][j]=sc.nextInt();
         }
        }
        
           System.out.println("Ваши элементы массива: ");
        for ( i=0; i<mas.length; i++){
         for( j=0; j<mas[i].length; j++){
            
             System.out.print(mas[i][j]+ "\t");
         }
            System.out.println();
        }
        System.out.println("Элементы главной диагонали матрицы: ");
        
         for (i=0; i<n; i++)
        
        
            System.out.println(mas[i][i]+" ");   
        int sum=0;
        System.out.println("Положительные элементы над главной диагональю матрицы:");
        for ( i=0; i<mas.length; i++){
         for( j=0; j<mas[i].length; j++){
        if(j>i&&mas[i][j]>0){
            sum=sum+mas[i][j];
            System.out.println(mas[i][j]+" ");   
        }
         }       
            }
        System.out.println("Сумма положительных элементов:");
        System.out.println(sum);
         }
        
         }
    


    
   

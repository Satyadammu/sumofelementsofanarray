# sumofelementsofanarray
import java.util.Arrays;
import java.util.Scanner;
public class SumOfElementsOfAnArray {
   public static void main(String args[]){
      System.out.println("Enter the required size of the array :: ");
      Scanner s = new Scanner(System.in);
      int size = s.nextInt();
      int myArray[] = new int [size];
      int sum = 0;
      int sum1=0;
      int res;
      System.out.println("Enter the elements of the array one by one ");

      for(int i=0; i<size/2; i++){
         myArray[i] = s.nextInt();
         sum = sum + myArray[i];
      }
      for(int i=size/2;i<size;i++){
         myArray[i] = s.nextInt();
         sum1 = sum1+ myArray[i];
      }
      res=sum*sum1;
      
     System.out.println("Sum of the elements of the array ::"+res);
   }
}

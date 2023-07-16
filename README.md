# Problem-4.T2021-2-4

import java.util.Arrays;

public class TotalCount {
    public static void main(String[] args) {
        int[] numbers = {1, 2, 8, 9, 12, 46, 76, 82, 15, 20, 30};
        int[] multiples = new int[10]; 
     
        for (int number : numbers) {
            for (int i = 1; i <= 9; i++) {
                if (number % i == 0) {
                    multiples[i]++;
                }
            }
        }
        
       
        for (int i = 1; i <= 9; i++) {
            System.out.println(i + ": " + multiples[i]);
        }
    }
}

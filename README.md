# Student-Grade-Calculator
//use java programming language
import java.util.Scanner;
public class GradeCalculator{
    public static void main(String args[]){
   
        Scanner sc = new Scanner(System.in);
        System.out.println("Enter marks of five subjects:");
        
        // Input
int M1, M2, M3, M4, M5;


while (true) {
    System.out.print("Marks of First Subject (0-100): ");
    M1 = sc.nextInt();

    if (M1 >= 0 && M1 <= 100) break; // valid input  
    System.out.println("Invalid input! Enter again.");
}
while (true) {
            System.out.print("Marks of Second Subject (0–100): ");
            M2 = sc.nextInt();
            if (M2 >= 0 && M2 <= 100) break;
            System.out.println("Invalid! Enter again.");
        }
       
               while (true) {
            System.out.print("Marks of Third Subject (0–100): ");
            M3 = sc.nextInt();
            if (M3 >= 0 && M3 <= 100) break;
            System.out.println("Invalid! Enter again.");
        }
        
         while (true) {
            System.out.print("Marks of Fourth Subject (0–100): ");
            M4 = sc.nextInt();
            if (M4 >= 0 && M4 <= 100) break;
            System.out.println("Invalid! Enter again.");
        }

 while (true) {
            System.out.print("Marks of Fifth Subject (0–100): ");
            M5 = sc.nextInt();
            if (M5 >= 0 && M5 <= 100) break;
            System.out.println("Invalid! Enter again.");
        }




        // Process

        int total = M1 + M2 + M3 + M4 + M5 ;
        double percentage = total / 5.0 ;

        char grade;

         if ( percentage >= 90 )
            grade = 'A';
         
         else if ( percentage >= 75 )
            grade = 'B';

         else if ( percentage >= 60 )
            grade = 'C';


         else if ( percentage >= 40 )
            grade = 'D';

         else 
            grade = 'F';

            // Output

            System.out.println("Total Marks =  " + total +" "+ "Out of 500");
            System.out.println("Percentage =  " + percentage);
            System.out.println("Grade =  " + grade);
    }
}

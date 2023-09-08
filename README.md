# CODSOFT

import java.util.Scanner;

public class GradeCalculator {
   public static void main(String[] args) {
      Scanner input = new Scanner(System.in);
      
      // Take input marks in each subject
      System.out.print("Enter marks obtained in subject 1: ");
      double sub1 = input.nextDouble();
      
      System.out.print("Enter marks obtained in subject 2: ");
      double sub2 = input.nextDouble();
      
      System.out.print("Enter marks obtained in subject 3: ");
      double sub3 = input.nextDouble();
      
      System.out.print("Enter marks obtained in subject 4: ");
      double sub4 = input.nextDouble();
      
      System.out.print("Enter marks obtained in subject 5: ");
      double sub5 = input.nextDouble();
      
      // Calculate total marks
      double totalMarks = sub1 + sub2 + sub3 + sub4 + sub5;
      
      // Calculate average percentage
      double averagePercentage = totalMarks / 5;
      
      // Grade Calculation
      String grade;
      if (averagePercentage >= 90) {
         grade = "A+";
      } else if (averagePercentage >= 80) {
         grade = "A";
      } else if (averagePercentage >= 70) {
         grade = "B";
      } else if (averagePercentage >= 60) {
         grade = "C";
      } else if (averagePercentage >= 50) {
         grade = "D";
      } else {
         grade = "F";
      }
      
      // Display Results
      System.out.println("Total Marks: " + totalMarks);
      System.out.println("Average Percentage: " + averagePercentage);
      System.out.println("Grade: " + grade);
   }
} 


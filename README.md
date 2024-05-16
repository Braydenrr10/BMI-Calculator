# BMI-Calculator
Body Mass Index Calculator using Java
import java.util.Scanner;

class HealthChartMain {
    public static void main (String[] args) {
    Scanner scnr = new Scanner(System.in);
    
    String First_Name; // Intialized string varibale for first name //
    String Last_Name;  // Intialized string varibale for last name //
    int Age;    // Intialized Int varibale for Age //
    double Weight;   // Intialized string varibale for first name //
    int height_Feet;  // Intialized string varibale for first name //
    int height_Inches; // Intialized string varibale for first name //
    
System.out.print("Please enter your first name: ");  // Print statement for first name //
    First_Name = scnr.next();  // Input command for first name //
System.out.print("Please enter your last name: ");   // Print statement for last name //
    Last_Name = scnr.next();   // Input command for last name //
System.out.print("Please enter your age: "); // Print statement for your age //
    Age = scnr.nextInt();      // Input command for age //
System.out.print("Please enter your weight: "); // Print statement for weight //
    Weight = scnr.nextDouble();  // Input command for weight //
System.out.print("Enter your height (Feet Only) : "); // Print statement for height in feet only //
    height_Feet = scnr.nextInt();   // Input command for height in feet //
System.out.print("Enter your the remaining inches for your height: "); // Print statement for inches in height //
    height_Inches = scnr.nextInt();   // Input command for height in inches remaining //
    
    double Weight_metric = Weight * 0.45359237; // Weight conversion to metric //
    int height_Feet_allinches = height_Feet * 12;  // Foot conversions to inches // 
    double height_metric = (double)(height_Feet_allinches + height_Inches) * (double)(0.0254); // Inches conversion to metric //
    double BMI = Weight_metric / Math.pow(height_metric,2); // BMI calculation //
    
System.out.printf("<" + First_Name + " " + Last_Name + "> you have a BMI value of %.3f", BMI); // Print statement back to the patient //
    
    
    }
}
     

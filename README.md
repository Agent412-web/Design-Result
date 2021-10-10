# Design-Result
Create result using java program included total marks , percentage and grade.

// Start your code here 

package Agent412-web.com;

import java.util.Scanner;

public class Main{

    public static void main(String[] args) {

        float eng , maths , phy , chem , comp ;
        double total , percentage ;

        Scanner sc = new Scanner(System.in);
        System.out.println("Enter marks of five subject");

        System.out.println("Enter marks of english subject");
        eng= sc.nextFloat();

        System.out.println("Enter marks of maths subject");
        maths = sc.nextFloat();

        System.out.println("Enter marks of physics subject");
        phy = sc.nextFloat();

        System.out.println("Enter marks of chemistry subject");
        chem = sc.nextFloat();

        System.out.println("Enter marks of computer subject");
        comp = sc.nextFloat();

        total = (eng + maths + phy + chem + comp);
        percentage = (total/500)*100;

        System.out.println("Total Marks = "+total);
        System.out.println("Total Percentage = "+percentage);

        if (percentage >=85 && percentage<100)
            System.out.println("Grade A");
        else if (percentage >= 70 && percentage<85)
            System.out.println("Grade B");
        else if (percentage >=50 && percentage<70)
            System.out.println("Grade C");
        else if (percentage >=33 && percentage<50)
            System.out.println("Grade D");
        else
            System.out.println("Fail");



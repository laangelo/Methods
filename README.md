import java.util.Scanner;

public class Methods {
    public static void main(String[] args) {
        findAndDisplayMinMax();
    }

    public static void findAndDisplayMinMax() {
        Scanner object = new Scanner(System.in);

        System.out.println("Enter the first number");
        double num1 = object.nextDouble();

        System.out.println("Enter the second number");
        double num2 = object.nextDouble();

        System.out.println("Enter the third number");
        double num3 = object.nextDouble();

        double smallestNumber = num1;
        double largestNumber = num1;

        if (num2 < smallestNumber) {
            smallestNumber = num2;
        } else if (num2 > largestNumber) {
            largestNumber = num2;
        }

        if (num3 < smallestNumber) {
            smallestNumber = num3;
        } else if (num3 > largestNumber) {
            largestNumber = num3;
        }

        System.out.println("The smallest number is " + smallestNumber);
        System.out.println("The largest number is " + largestNumber);
        System.out.println(largestNumber + " is your largest number, and " + smallestNumber + " is your smallest number");
    }
}

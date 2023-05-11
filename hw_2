package hw_2;

import java.util.InputMismatchException;
import java.util.Scanner;
public class hw2 {
    public static void main(String[] args) {
        task_1();
        task_2();
        task_3();
        task_4();
    }


    public static void task_1() {
        Float number = null;
        do {
            try {
                System.out.println("Enter fractional number: ");
                Scanner scanner = new Scanner(System.in);
                number = scanner.nextFloat();
                scanner.close();
            } catch (InputMismatchException e) {
                System.out.println("Wrong, you need to enter fractional number");
            }
        } while (number == null);
        System.out.println("Done, you enter number " + number);
    }

    public static void task_2() {
        try {
            int d = 0;
            int[] intArray = new int[9];
            intArray[8] = 15;
            double catchedRes1 = intArray[8] / d;
            System.out.println("catchedRes1 = " + catchedRes1);
        } catch (ArithmeticException e) {
            System.out.println("Catching exception: " + e);
        }
    }

    public static void task_3() {
        try {
            int a = 90;
            int b = 3;
            System.out.println(a / b);
            printSum(23, 234);
            int[] abc = {1, 2};
            abc[3] = 9;
        } catch (NullPointerException ex) {
            System.out.println("A pointer cannot point to null");
        } catch (IndexOutOfBoundsException ex) {
            System.out.println("The array is out of its size");
        } catch (Throwable ex) {
            System.out.println("Something goes wrong");
        }
    }

    public static void printSum(Integer a, Integer b) {
        System.out.println(a + b);
    }

    public static void task_4() {
        String line = null;
        do {
            Scanner scanner = new Scanner(System.in);
            try {
                System.out.println("Enter something: ");
                line = scanner.nextLine();
                if ("".equals(line)) {
                    throw new InputMismatchException();
                }
                scanner.close();
            } catch (InputMismatchException e) {
                System.out.println("Do nut enter empty string");
            }
        } while (line == null || "".equals(line));
        System.out.println("Well done, you entered: " + line);
    }
}

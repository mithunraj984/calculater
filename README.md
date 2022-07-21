# calculater
import java.util.Scanner;

public class Calculation1 {
    public static void main(String[] args) {
        Scanner calculater =new Scanner(System.in) ;

        // ask users to enter numbers
        System.out.println("Enter first number");
       double number1 = calculater.nextDouble();
        System.out.println("Choose an operator: +, -, *, or /");
        char  operator = calculater.next().charAt(0);

        System.out.println("Enter second number");
       double number2 = calculater.nextDouble();

        switch (operator) {

            case '+':
             double   result = number1 + number2;
                System.out.println(number1 + " + " + number2 + " = " + result);
                break;


            case '-':
                result = number1 - number2;
                System.out.println(number1 + " - " + number2 + " = " + result);
                break;


            case '*':
                result = number1 * number2;
                System.out.println(number1 + " * " + number2 + " = " + result);
                break;


            case '/':
                result = number1 / number2;
                System.out.println(number1 + " / " + number2 + " = " + result);
                break;

            default:
                System.out.println("Invalid operator!");
                break;
        }


    }
}

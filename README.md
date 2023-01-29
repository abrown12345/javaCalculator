# javaCalculator
import java.util.Scanner;
public class javaCalculator {

	public static void main(String[] args) {
		char operator;
		int number1;
		int number2;
		Scanner input=new Scanner(System.in);
		
		System.out.println("Enter your first number."); 
		number1= input.nextInt();
		
		System.out.println("Enter your second number.");
		number2= input.nextInt();
		
		System.out.println("Choose an operator: +, -, *, /, or i for squaring your first entered integer");
		operator= input.next().charAt(0);
		
		switch (operator) {
		case '+':
			System.out.println(addNumbers(number1, number2));
			break;
		case '-': 
			System.out.println(subNumbers(number1,number2));
			break;
		case '*': 
			System.out.println(multNumbers(number1,number2));
			break;
		case '/': 
			System.out.println(divNumbers(number1,number2));
			break;
		case 'i':
			System.out.println(squareNumbers(number1,number2));
			break;
		}
	} 

	public static int addNumbers(int number1, int number2) {
		int sum= number1+number2;
		return sum;
		}
	public static int subNumbers(int number1, int number2) {
		int difference= number1-number2;
		return difference;
	}
	
	public static int multNumbers(int number1, int number2) {
		int product= number1*number2;
		return product;
	}
	
	public static int divNumbers(int number1, int number2) {
		int quotient= number1/number2;
		return quotient;
	}
	
	public static int squareNumbers(int number1, int number2) {
		int square= number1*number1;
		return square;
	}
}

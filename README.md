# Invest
Helps one find the final amount resulted from an investment

	import java.util.Scanner;
	import java.lang.Math;

	public class Invest
	{
		private static Scanner myScanner = new Scanner(System.in); 

		public static void main(String[] args)
		{
			System.out.println("Enter an amount to be invested.");
			double investAmount = myScanner.nextDouble(); 

	    System.out.println("Enter the interest rate.");
			double interestRate = myScanner.nextDouble(); 

	    System.out.println("Enter the amount of times you want to compound the investment.");
			int numOfTimeCompounded = myScanner.nextInt(); 

	    System.out.println("Enter the amount of years you want to invest for.");
			int years = myScanner.nextInt(); 

	    int power = numOfTimeCompounded * years;
	    System.out.println(power);

	    double midEquation = 1 + (interestRate / numOfTimeCompounded);

	    double equationWithoutPrincipal =  Math.pow(midEquation, power);
	    System.out.println(equationWithoutPrincipal);

	    double finalAmount = equationWithoutPrincipal * investAmount;
	    System.out.println(finalAmount);





	  }

	}

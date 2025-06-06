import java.util.Scanner;
public class SumofEvenA5 
{
	public static void main(String[] args)
	{
					Scanner scan=new Scanner(System.in);
					System.out.println("Enter the value of n");
					int n=scan.nextInt();
					findEven(n);
					findOdd(n);
	}
		public static void findEven(int n)
		{
			// variable to store sum of even numbers
			int evenSum=0;
			System.out.print("Even numbers are : ");
		// searching all even numbers in the range of 1 to n
	for(int i=1; i<=n; i++)
		{
			//checking whether number is even
		if(i%2==0)
		{
			// calculating the sum of all even numbers, storing in evenSum
			evenSum+=i;
			// checking whether number is less than n-1
			if(i<(n-1)) 
			{
				// if true print after value
				System.out.print(i+",");
			}
		// if number is equal to n or n-1
			else
				{
					// do not print ,
				System.out.println(i);
				}
		}
	}
	System.out.println("Sum of Even numbers is : "+evenSum);
}
		public static void findOdd(int n)
		{
			// variable to store sum of Odd numbers
			int oddSum=0;
			System.out.print("Odd Numbers are : ");
		// searching all odd	Numbers in the range of 1 to n
	for(int i=1; i<=n; i++)
		{
			//checking whether number is odd
		if(i%2!=0)
		{
			// calculating the sum of all odd numbers, storing in oddSum
			oddSum+=i;
			// checking whether number is less than n-1
			if(i<(n-1)) 
			{
				// if true print after value
				System.out.print(i+",");
			}
		// if number is equal to n or n-1
			else
				{
					// do not print ,
				System.out.println(i);
				}
		}
	}
	System.out.println("Sum of Odd numbers is : "+oddSum);
}
}

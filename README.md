# sum_of_digit_of_number

import java.util.Scanner;
public class pattern16 {

	public static void main(String[] args) {
		// TODO Auto-generated method stub
		Scanner s=new Scanner(System.in);
		long n=s.nextInt();
		long y=print(n);
		System.out.print(y);                                                      ////sum of the digits
	}
	public static long print(long n) {
		if(n<10) 
			return n; 
		else {
			return (n%10 + print(n/10));                                           /////using recursion
		}
	}
}


output::

123456789
45

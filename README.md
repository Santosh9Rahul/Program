package aaa;
import java.util.Scanner;
public class Calculator 
{

	public static void main(String[] args) 
	{
		Scanner scan=new Scanner(System.in);
		System.out.println("enter a value of A");
		double a=scan.nextDouble();
		System.out.println("enter a value of B");
		double b=scan.nextDouble();
		System.out.println("enter a type of operation");
		System.out.println("press -addition- to add");
		System.out.println("press -subtraction- to sub");
		System.out.println("press -multiplication- to mul");
		System.out.println("press -division- to div");
		System.out.println();
		double c=0;
		String s=scan.next();
		switch(s)
		{
		case "addition":c=a+b;
		System.out.println("the additoin of "+a+" + "+b+" "+"is:- "+c);
		break;
		case "subtraction":c=a-b;
		System.out.println("the subtraction of "+a+" - "+b+" "+"is:- "+c);
		break;
		case "multiplication":c=a*b;
		System.out.println("the multiplication of "+a+" * "+b+" "+"is:- "+c);
		break;
		case "division":c=a/b;
		System.out.println("the division of "+a+" / "+b+" "+"is:- "+c);
		break;
		default:System.out.println("select valid operation");
		System.exit(0);
		}
		scan.close();
	}

}




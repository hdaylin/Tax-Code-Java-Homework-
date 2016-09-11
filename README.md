# Tax-Code-Java-Homework- 

import java.util.Scanner;

public class taxCode {

	public static void main(String[] args) {
		{
			int customerId; 
			String customerFName; 
			String customerLname;
			double salesAmount;  
			String taxCode; 
			
			Scanner keyboard = new Scanner (System.in);   
			
			System.out.print( "Enter the Customer ID: " );
			customerId = keyboard.nextInt();  
			
			System.out.print( "Enter the Customer's First Name: " );
			customerFName = keyboard.next(); 
			
			System.out.print( "Enter the Last Name: " );
			customerLname = keyboard.next();
			
			System.out.print( "Enter the sales amount: " );
			salesAmount = keyboard.nextDouble();  
			
			System.out.print( "Enter the Tax Code: " );
			taxCode = keyboard.next();  
			
			if (taxCode.equals ("NRM")){ 
			System.out.println("Customer ID: " + customerId); 
			System.out.println("Customer Name: " + customerFName + " "+customerLname);  
			System.out.println("Sales Amount: " + "$" + salesAmount); 
			System.out.println("Tax Code: " + taxCode); 
			System.out.println("Total Amount Due: " + ("$" + salesAmount + (salesAmount * .06))); 
			
			}else if(taxCode.equals ("NPF")){ 
			System.out.println("Customer ID: " + customerId); 
			System.out.println("Customer Name: " + customerFName + " "+ customerLname);  
			System.out.println("Sales Amount: " + "$" + salesAmount); 
			System.out.println("Tax Code: " + taxCode); 
			System.out.println("Total Amount Due: " + ("$" + salesAmount)); 
			
			}else{ 
			System.out.println("Customer ID: " + customerId); 
			System.out.println("Customer Name: " + customerFName + " "+ customerLname);  
			System.out.println("Sales Amount: " + "$" + salesAmount); 
			System.out.println("Tax Code: " + taxCode); 
			System.out.println("Total Amount Due: " + ("$" + salesAmount + (salesAmount * .045)));
		
		} 
			keyboard.close(); 
	}
		} 
	
}

import java.util.Scanner;

public class RippleSales {
	static Scanner kb = new Scanner(System.in);
	static int packSize = 25;
	static final double price = 0.26;

	public static void main(String[] arg)
	{
		do
		{
			BuyRipple();
		}
		while(NewCustomer());		//loop while we have customers to serve
		
		System.out.println("\nThank you for using Ripple Systems.");
				
		kb.close();				//close the scanner
	}
	
	
	private static void BuyRipple()
	{
		int quantity = 0;

		System.out.print("\nEnter a quantity: ");
		quantity = kb.nextInt();
		kb.nextLine();	//clear the buffer
		
		if(quantity % packSize == 0)
		{
			System.out.printf("You have ordered %d ripples -- $%.02f\n", quantity, price * quantity);
		}
		else
		{
			System.out.println("Ripples can only be ordered only in packs of " + packSize + ".");
		}
			
		System.out.println();
	}
	
	
	private static boolean NewCustomer()
	{
		char a = ' ';
		while(a!='y' && a !='n')
		{
			System.out.print("Next Customer? [y/n]");
			a = kb.nextLine().trim().charAt(0);
		}
		
		if(a == 'y')
			return true;
		else
			return false;
	}
}

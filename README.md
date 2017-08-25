# Guessing_Game


import java.util.Scanner;

public class Guessinggame 
//Eli Manning
{

	public static void main(String[] args) 
	
	{
		Scanner cin = new Scanner(System.in);//started the scanner 
		
		System.out.println("Welcome to the guessing game please input a number 0-100.");//System prints out starting statement
		
		int a = 0;//initialized variable a as 0
		int b = 100;//initialized variable b as 100
		
		boolean won = false;//declared boolean variable as won which was set to equal false 
		
		
		int random = (int) (a + b*Math . random());//this is how the system generates a random #
		
		while(!won)//while not won 
		{
			int guess = cin.nextInt();//reads in the guess
			if(random < guess)// if the random number is less than your guess
			{
				System.out.println("Too high!");//if your guess was to high then the system will display the message Too high
			}
		
			else if (random > guess)//If your guess isn't too high then the system checks if it is too low
		
				{
					System.out.println("Too low!");//if your guess is too low then the system displays the Too low message 
				}
					else if (random == guess)//if none of the other two possibilities are true then it checks this one 
						
						
						{
							System.out.println("CONGRATS YOU GOT IT RIGHT!!");//Since none of the other two works then you must have won so this message is played.
							won = true;	//declares boolean variable won to become true 
		
						}
		
		
		
		}
		cin.close();//closes the loop
	}
}


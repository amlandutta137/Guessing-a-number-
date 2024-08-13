# Guessing-a-number-
import  java.util.Scanner;
public class Randomnumber {
    public static void main(String []args){
        Scanner sc= new Scanner(System.in);
        int myNumber= (int)(Math.random()*100);
        int userNumber= 0;
        
        do{
            System.out.println("Guess my number(1-115) : ");
            userNumber =sc.nextInt();
            
            if(userNumber == myNumber){
                System.out.println("WOHO YOU GUESS THE CORRECT NUMBER");
                break;
            }
            else if(userNumber > myNumber){
                System.out.println("your number is too large");
            }
            else{
                System.out.println("Your number is too small");
            }
        }
        while(userNumber >=0);

        System.out.println("My number was : ");
        System.out.println(myNumber);
    }
}

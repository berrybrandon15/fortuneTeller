import java.util.Random;
import java.util.Scanner;

public class fortuneTeller {

    public static void main(String[] args) {
        Scanner userInput = new Scanner(System.in);
        Random fortune = new Random();

        int num;
        String yesOrNo;

        System.out.println("Would you like to know what your future holds?");
            yesOrNo = userInput.nextLine();
            while(yesOrNo.equalsIgnoreCase("yes")) {
                num = fortune.nextInt(10);

                switch(num) {
                case 0:
                    System.out.println("You will be rich");
                    break;
                case 1:
                    System.out.println("You will have a beautiful girlfriend");
                    break;
                case 2: 
                    System.out.println("You will be broke");
                    break;
                case 3:
                    System.out.println("You will be sad");
                    break;
                case 4: 
                    System.out.println("You will be alone");
                    break;
                case 5:
                    System.out.println("You will have good luck");
                    break;
                case 6: 
                    System.out.println("You will get a higher paying job");
                    break;
                case 7:
                    System.out.println("You will get married");
                    break;
                case 8:
                    System.out.println("You will get fired");
                    break;
                case 9:
                    System.out.println("You will be happy");
                    break;
                }

            System.out.println("Do you wnat to know you fortune again?");
            yesOrNo = userInput.nextLine();
        }
    
        userInput.close();
        System.out.println("GoodBye");
    }
}

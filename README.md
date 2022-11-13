/**
* Name: Rosalyn C. Lawas
* Section: Fidelity
* Year: 4th Year
*/


import java.util.Scanner;

public class lawasStore{

    public static void main(String[] args) {
        Scanner rcl = new Scanner(System.in);
         int cakes,juices,drinks;
         int total = 0;
        int loop;
        System.out.println("==== Welcome to lawas store ====");
        do{

        System.out.println("\n Would you like to order? [1-YES||2-NO]");
        int wantToOrder = rcl.nextInt();
        
        
        if(wantToOrder == 1){
            loop = 1;
            System.out.println("1. cakes");
            System.out.println("2. juices");
            System.out.println("3. drinks");
            int likeToOrder = rcl.nextInt();
            
            switch(likeToOrder){
                case 1:{
                    System.out.println(" cakes");
                    System.out.println("1. Chocolate cake 150 php");
                    System.out.println("2. Red velvet cake 200 php");
                    System.out.println("3. Ube cake 250php");
                    System.out.println("4. Chocomoist cake 300 php");
                    cake = rcl.nextInt();
                    if(cakes == 1){
                     total += 150;
                     System.out.println("Chocolate cake added to cart");
                    }
                    else if(cakes == 2){
                     total += 200;
                     System.out.println("Red velvet cake added to cart");
                    }
                    else if(cakes == 3){
                     total += 250;
                     System.out.println("Ube cake added to cart");
                    }
                    else if(cakes == 4){
                     total += 300;
                     System.out.println("Chocomoist cake added to cart");
                    }
                    else{
                        System.out.println("Choose 1-4 only");
                    }
                    break;
                }
                    case 2:{
                    System.out.println("juices");
                    System.out.println("1. 4 season juice 100 php");
                    System.out.println("2. Mango juice 80 php");
                    System.out.println("3. Lemonade juice 80 php");
                    System.out.println("4. Orange juice 100 php");
                    juices = rcl.nextInt();
                    if(juices == 1){
                     total += 100;
                     System.out.println("4 season juice added to cart");
                    }
                    else if(juices == 2){
                     total += 80;
                     System.out.println("Mango juice added to cart");
                    }
                    else if(juices == 3){
                     total += 80;
                     System.out.println("Lemonade juice added to cart");
                    }
                    else if(juices == 4){
                     total += 100;
                     System.out.println("Orange juice added to cart");
                    }
                    
                    else{
                        System.out.println("Choose 1-4 only");
                    }
                    break;
                }
                case 3:{
                    System.out.println("drinks");
                    System.out.println("1. Coke 30 php");
                    System.out.println("2. Royal 30 php");
                    System.out.println("3. Sprite 30 php");
                    System.out.println("4. Mt. Dew 50 php");
                    drinks = rcl.nextInt();
                    if(drinks == 1){
                     total += 30;
                     System.out.println("Coke added to cart");
                    }
                    else if(drinks == 2){
                     total += 30;
                     System.out.println("royal added to cart");
                    }
                    else if(drinks == 3){
                     total += 30;
                     System.out.println("Sprite added to cart");
                    }
                    else if(drinks == 4){
                     total += 50;
                     System.out.println("Mt. Dew added to cart");
                    }
                    else{
                        System.out.println("Choose 1-4 only");
                    }
                    break;
                }
          
        }
        }
        else{
            loop = 0;
        }
        }while(loop == 1);
        
          System.out.println("Total Cost: "+total);
          System.out.println("Thank you for the orders! ");
    }
}

Coin-Game
=========

User interactive game.
import java.util.Scanner;
/**
 * This game will be able to play the game "don't get stuck with the last coin" by starting with 23 coins and working down to the last one. 
 * The coputer will ask the player "How many coins 1,2 or 0?" and react according to the players moves in order to win the game unless the player plays perfectly
 * @author (your name) Banerjee, Diya
 * @version (a version number or a date) 10/19/12
 */
public class CoinGame5
{
     public static void main (String []agrs)
     {
     
        Scanner kb = new Scanner (System.in);
        System.out.println("How many coins 1,2, or 0?");
        int x =kb.nextInt();
        if(x==1)//If player decides to start with 1 coin this set of code will execute
        {
            System.out.println("I am taking 1 coin");//computers response to player taking 1 coin
            System.out.println("How many coins 1 or 2?");
            x=kb.nextInt();
            if(x==1)//Player takes one coin after starting with one
           {
            System.out.println("I am taking 1 coin");//computers response to player taking 1 coin after taking one
            System.out.println("How many coins 1 or 2?");
            x=kb.nextInt();
            for(int i=0; i<3; ++i)//this for loop will run until the game ends 
                {
                    if (x==1)
                    {
                 
                    System.out.println("I am taking 2 coins");//If player takes 1 coin, computer will take 2
                    System.out.println("How many coins 1 or 2?");
                    x =kb.nextInt();
                    }
                    if (x==2)
                    {
                    System.out.println("I am taking 1 coin");//If player takes 2 coins, computer will take 1
                    System.out.println("How many coins 1 or 2?");
                    x =kb.nextInt();
                    }
                    
                }
              System.out.println("Sorry you lose!");//Response to player losing the game
           }
           if(x==2)//Player takes two coins after starting with one
           {
            System.out.println("I am taking 1 coin");//computers response to player taking 2 coins after taking one
            System.out.println("How many coins 1 or 2?");
            x=kb.nextInt();
            if(x==1)//player takes one coin then two coins then one coin
             { 
                System.out.println("I am taking 1 coin");//computers response to player taking 1 coin then two coins then one coin
                System.out.println("How many coins 1 or 2?");
                x=kb.nextInt();
                for(int i=0; i<3; ++i)//this for loop will run until the game ends 
                    {
                    if (x==1)
                    {
                 
                    System.out.println("I am taking 2 coins");//If player takes 1 coin, computer will take 2
                    System.out.println("How many coins 1 or 2?");
                    x =kb.nextInt();
                    }
                    if (x==2)
                    {
                    System.out.println("I am taking 1 coin");//If player takes 2 coins, computer will take 1
                    System.out.println("How many coins 1 or 2?");
                    x =kb.nextInt();
                    }
                    
                  }
                  System.out.println("Sorry you lose!");//Response to player losing the game
             }
             if(x==2)//Player takes one coin then two coins then two coins
             {   
                System.out.println("I am taking 1 coin");//computers response to player taking 1 coin then two coins then two coins
                System.out.println("How many coins 1 or 2?");
                x=kb.nextInt();
                for(int i=0; i<2; ++i)//this for loop will run until the game ends 
                    {
                    if (x==1)
                    {
                 
                    System.out.println("I am taking 2 coins");//If player takes 1 coin, computer will take 2
                    System.out.println("How many coins 1 or 2?");
                    x =kb.nextInt();
                    }
                    if (x==2)
                    {
                    System.out.println("I am taking 1 coin");//If player takes 2 coins, computer will take 1
                    System.out.println("How many coins 1 or 2?");
                    x =kb.nextInt();
                    }
                    
                  }
                 System.out.println("Congratulations You Have Played A Perfect Game!!!");//Response to player winning the game
             }
           } 
        }
        
        
        
        
        if(x==2)////if the Player starts with 2 coins this set of code will execute
      {
          System.out.println("I am taking 2 coins");//Computers response if player starts with 2 coins
          System.out.println("How many coins 1 or 2?");
          x=kb.nextInt();
          if(x==1)//Player decides to take another one coin after taking two
        {
          System.out.println("I am taking 2 coins");//Computers response if player takes 1 coin after taking 2
          System.out.println("How many coins 1 or 2?");
          x=kb.nextInt();
          for(int i=0; i<4; ++i)//this for loop will run until the game ends 
                {
                    if (x==1)
                    {
                 
                    System.out.println("I am taking 2 coins");//If player takes 1 coin, computer will take 2
                    System.out.println("How many coins 1 or 2?");
                    x =kb.nextInt();
                    }
                    if (x==2)
                    {
                    System.out.println("I am taking 1 coin");//If player takes 2 coins, computer will take 1
                    System.out.println("How many coins 1 or 2?");
                    x =kb.nextInt();
                    }
                    
                }
                System.out.println("Sorry you lose!");//Response to player losing the game
            
        }
        if(x==2)//if player takes two coins after originally taking two coins this set of code will execute
       {
           System.out.println("I am taking 1 coin");//Computers response if player takes two coins after originally taking two
           System.out.println("How many coins 1 or 2?");
           x=kb.nextInt();
           
                for(int i=0; i<4; ++i)//this for loop will run until the game ends 
                {
                    if (x==1)
                    {
                 
                    System.out.println("I am taking 2 coins");//If player takes 1 coin, computer will take 2
                    System.out.println("How many coins 1 or 2?");
                    x =kb.nextInt();
                    }
                    if (x==2)
                    {
                    System.out.println("I am taking 1 coin");//If player takes 2 coins, computer will take 1
                    System.out.println("How many coins 1 or 2?");
                    x =kb.nextInt();
                    }
                    
                }
                System.out.println("Sorry you lose!");//Response to player losing the game
       }
    
    }
     
    
    
    if(x==0)//Player decides computer should go first
        {
            System.out.println("I am taing 1 coin");//computers response if player decides computer should start
            System.out.println("How many coins 1 or 2?");
            x=kb.nextInt();
            if(x==1)//if player takes one coin after computers move
           {
              System.out.println("I am taing 1 coin");//computers response if player takes 1 coin
              System.out.println("How many coins 1 or 2?");
              x=kb.nextInt();
               if(x==1)
              {
                  System.out.println("I am taing 2 coins");//computers response if player takes another one coin
                  System.out.println("How many coins 1 or 2?");
                  x=kb.nextInt();
                  for(int i=0; i<3; ++i)//this for loop will run until the game ends 
                {
                    if (x==1)
                    {
                 
                    System.out.println("I am taking 2 coins");//If player takes 1 coin, computer will take 2
                    System.out.println("How many coins 1 or 2?");
                    x =kb.nextInt();
                    }
                    if (x==2)
                    {
                    System.out.println("I am taking 1 coin");//If player takes 2 coins, computer will take 1
                    System.out.println("How many coins 1 or 2?");
                    x =kb.nextInt();
                    }
                    
                }
                System.out.println("Sorry you lose!");//Response to player losing the game
              }
           }
        
        if(x==2)//if player decides to let computer start then takes two coins
        {
            System.out.println("I am taing 1 coin");//computers response if player takes 2 coins
            System.out.println("How many coins 1 or 2?");
            x=kb.nextInt();
            for(int i=0; i<3; ++i)//this for loop will run until the game ends 
                {
                    if (x==1)
                    {
                 
                    System.out.println("I am taking 2 coins");//If player takes 1 coin, computer will take 2
                    System.out.println("How many coins 1 or 2?");
                    x =kb.nextInt();
                    }
                    if (x==2)
                    {
                    System.out.println("I am taking 1 coin");//If player takes 2 coins, computer will take 1
                    System.out.println("How many coins 1 or 2?");
                    x =kb.nextInt();
                    }
                    
                }
            System.out.println("Sorry you lose!");//response to player losing the game
        }
    }
    
        
    }
}




















# nycscertweb

## Welcome!
my first repo :)

## Programming in Java
Here's a snippet of the Mancala program developed with Emma and Michelle. The picture shows the full board, players taking turns, and player 2 earning another turn after dropping the last stone in player 1's pot:

<img width="545" alt="Screen Shot 2021-07-22 at 2 55 35 PM" src="https://user-images.githubusercontent.com/80486821/126693756-8d255d6b-413a-4bb8-8d89-2c03bc4e9e3f.png">

The code that prints the game board is below. We used two `for` loops (one that incremented and one that decremented) and multiple `println` statements.
    
    public static void printGameboard(int[] gameBoard){
    System.out.println();
    
    //Print p2's row
    System.out.print("p2 ");

    //Decrement from the last index in the array to index 7. Output as P2's row.
    for(int i = 13; i > 6; i--)  {
      System.out.print(gameBoard[i] + " ");
    }

    //Print a new line and a space before P1's row
    System.out.println();
    System.out.print("     ");

    //Increment from the first index to index 6. Output as P1's row.
    for(int i = 0; i < 7; i++)  {
      System.out.print(gameBoard[i] + " ");
    }
    
    //Label p1's row
    System.out.println("p1");
    System.out.println();
    
    } //end printGameBoard
  

## Data Structures

## Methods I

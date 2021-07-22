# nycscertweb

## Welcome!
See below for some of my best work during the summer cert program :)

## Programming in Java
### Here's a snippet of the **Mancala** program developed with Emma and Michelle. 

The picture shows the full board, players taking turns, and player 2 earning another turn after dropping the last stone in player 1's pot:

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
### Working with Marisa and Stephannia, we built an algorithm for the **insertion sort**. 

The program constantly traverses the list to find the next smallest number. The program swaps that next smallest number with the number that is occupying the next smallest number's final resting position. The program repeats this until all the numbers are ordered correctly.

The insertion sort is an in-place sort that, in this solution, has _O(n^2)_ or quadratic runtime since it traverses the list as many times as the list is long.

<img width="484" alt="Screen Shot 2021-07-22 at 3 22 06 PM" src="https://user-images.githubusercontent.com/80486821/126697561-81ff2ecd-93b2-448a-bed8-d2d99c47f072.png">

The `sort()` method is below.

We needed a variable, `smallestIndex`, to store the index of the next smallest number. We also needed variable `valSmallIndex` to store the value at `smallestIndex` so it wouldn't get overwritten during the swap.

    public void sort(){
    int smallestIndex;
        for (int i = 0; i < data.size(); i++){
            smallestIndex = findSmallestIndex(i); //find index holding next smallest value from current value of i to end of list
            int valSmallIndex = data.get(smallestIndex); 
            data.set(smallestIndex, data.get(i));
            data.set(i, valSmallIndex); // swap the item at that index and i
        } //end for loop
    } //end sort
  



## Methods I
### Jiyoon and I developed an unplugged activity for students to further explore objects and attributes.
___
**Learning goal:** SWBAT explain how:
- objects are created from classes, and
- class attributes hold data about the object.

**Vocabulary:** object, class, attributes
___
As students walk in the room, each is given a card: playing card, Uno card, Yu-Gi-Oh card, etc.
Students are asked to find others like themselves.

**Elicit:**
- Each type of card is an object created from its own class (i.e. Uno cards have an Uno class).
- Each card has attributes such as number, suit, color, type, etc.
- A class is like a template with defined attributes to create objects/instances.
- Member methods defined in each class can only be used on objects in that class.

**Discussion / Questions:**
- "What does it mean to find others like yourself? How did you group yourselves?"
- "What similarities/differences do you see between you and other people in your group?"
- "Compare the attributes (instance vars) of a Yu-Gi-Oh card and a playing card."
- "Can we play an Uno card in defense mode, like red7.playDefenseMode()? Why doesn't that make sense?"
- "How might we extend this idea to other things?"
  - Every car has a certain number of doors, wheels, and engines.
  - Every Chipotle burrito has a choice of protein, rice, and beans.

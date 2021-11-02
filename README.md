# Console "Tic-Tac-Toe" Game

## Methods review:  
### &nbsp;&nbsp;&nbsp;&nbsp; **1. "main" method**  

&nbsp;&nbsp;&nbsp;&nbsp;We created a game board and printed it. Then we created a game loop by using a "while" statement   
   in which we ask a player to type in a number (from 1 to 9) using Scanner, store this number in the  
   ArrayList named "playerPositions" and check if there's a winner. The same goes for the computer.  
   We're placing symbols and checking if there is a winner until a player/computer won or there's a draw.    
	
	
### &nbsp;&nbsp;&nbsp;&nbsp; **2. "printGameBoard" method**  

&nbsp;&nbsp;&nbsp;&nbsp; *"printGameBoard"* is used to print our game board, which we created in the "main" method before.  
*"printGameBoard"* was created by using two "for-each" statements. The first loop is used for each row  
inside of the game board and the second loop is used for each symbol inside of the row. It helps to minimize  
  the amount of code in the *"main"* method and to re-use our code.    
	
  ### &nbsp;&nbsp;&nbsp;&nbsp; **3. "placePiece" method**
  
  &nbsp;&nbsp;&nbsp;&nbsp; *"placePiece"* is used to place a symbol on our game board.  
  
&nbsp;&nbsp;&nbsp;&nbsp;Method's parameters consist of:  
  
   &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; 1. Two-dimensional array in which we will place symbols;
      
   &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; 2. Position (int variable from 1 to 9) on the game board where we want to place our symbol;
       
   &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; 3. The type of user. It's either a player or a computer.  
      
&nbsp;&nbsp;&nbsp;&nbsp; *"placePiece"* was implemented by using a "switch" statement, which helps us to cover all of the 
  spots on the game board.   
  Additionally, I've added "if" statements to decide whether the symbol 
  should be 'X' or 'O' depending on the type of the user. 
	
  ### &nbsp;&nbsp;&nbsp;&nbsp; **4. "checkWinner" method** 
  
&nbsp;&nbsp;&nbsp;&nbsp; *"checkWinner"* is used to check where the player's and computer's positions are and see if there's a winner.  
We can organize the "winning" positions by using a "List" for every row, column, and cross (topRow, leftCol, firstCross, etc.).  
Then we create an ArrayList called "winning" which will contain all of our Lists with winning conditions.   

&nbsp;&nbsp;&nbsp;&nbsp; We have to store player's and computer's positions in another List so we can compare them to the winning conditions 
from an ArrayList called "winning". To implement that we should create two ArrayLists named "playerPositions" and "computerPosition" 
(before "main" method) to store player's and computer's positions.  

&nbsp;&nbsp;&nbsp;&nbsp; For comparison, we use "for-each" statement where we check if the winning conditions from the ArrayList called "winning" 
are contained in one of our ArrayLists named "playerPositions" and "computerPositions".





\# Initialize game  
Initialize start screen  

\# Start game loop  
When start button pressed:  
&emspInitialize mode selection screen  
&emsp&emspFor each button/option:  
&emsp&emspIf selected:  
&emsp&emsp&emspChange game parameter to match  
&emsp&emspElse:  
&emsp&emsp&emspUse other option or default  

While game is running:  
&emspDisplay current score  
&emspDisplay board as edited by player-chosen specifications  
&emspDisplay current players  
&emspFor each player turn:  
&emsp&emspWhen player hovers over box:  
&emsp&emsp&emspHighlight the box  
&emsp&emspIf click input:  
&emsp&emsp&emspPlace player’s token in grid spot  
&emsp&emsp&emspCheck for line completion in that box  
&emsp&emsp&emspUpdate score based on completed lines  
&emsp&emsp&emspComplete larger line box if possible  
&emsp&emsp&emspChange to next player turn  
&emspIf space pressed:  
&emsp&emspIf power-up available:  
&emsp&emsp&emspActivate power-up (e.g., change token, clear tied/unfinished box, etc.)  
&emsp&emspElse:  
&emsp&emsp&emspAlert player that no power-up is available  
&emspIf "pause" or Escape button pressed:  
&emsp&emspPause game  
&emsp&emspDisplay save and quit buttons  
&emsp&emspIf save button pressed:  
&emsp&emsp&emspSave game progress  
&emsp&emspIf quit button pressed:  
&emsp&emsp&emspExit current game  

\# Power-up logic  
For each active power-up:  
&emspCheck if power-up is available to current player  
&emspIf available:  
&emsp&emspTrigger corresponding effect (e.g., change token, clear tied/unfinished box, etc.)  
&emsp&emspRemove power-up from player  

\# Check for game over condition  
If grid is full or largest grid has completed line:  
&emspEnd game  
&emspDisplay "Game Over: Player [winner] won!"  

\# Continue next frame  
Update game screen with new state  

\# Line completion logic  
For each box:  
&emspIf box has completed line:  
&emsp&emspIf not the largest board:  
&emsp&emsp&emspChange completed box to token on next level of board
&emsp&emsp&emspIncrease score
&emsp&emspElse:  
&emsp&emsp&emspEnd game  

\# End of game  
If player finishes or exits game:  
&emspDisplay final score and winner  
&emspAsk if player wants to restart, save, or quit  

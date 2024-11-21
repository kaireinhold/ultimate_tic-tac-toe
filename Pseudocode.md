\# Initialize game  
Initialize start screen

\# Start game loop  
When start button pressed initialize mode selection screen  
	For each button/option:  
		If selected:  
			Change game parameter to match
   		Else:  
			Other option or default  
While game is running:  
	Display current score  
	Display board as edited by player-chosen specifications  
	Display current players  
	While each player turn:  
		When player hovers over box light up  
		If click input:  
			Place that player’s token in grid spot  
			Check for line completion in that box  
			Update score based on how many lines each player has  
			Complete larger line box if possible  
			Change player turn  
	If space pressed:  
		If powerup available:  
			Activate power-up (e.g., change chosen token, clear tied/unfinished box, etc.)  
		Else:  
			Alert player that no powerup is available          
	If player presses "pause" or presses Escape button:  
		Pause game  
		Display save and quit buttons  
		If save button is pressed:  
			Save game progress  
		If Quit button is pressed:  
			Exit current running game  
          
\# Power-up logic  
	For each active power-up:  
		Check if power-up is available to current player  
		If available:  
			Trigger corresponding effect (e.g., change chosen token, clear tied/unfinished box, etc.)  
			Remove power-up from player  
      
\# Check for game over condition  
	If grid is full or largest grid has completed line:  
		End game  
		Display "Game Over: Player \[whoever completed line in largest grid\] won\!"  
      
\# Continue next frame  
	Update game screen with new state

\# Line completion logic  
Check each box for complete line  
If a box has completed line:  
	Change completed box to a token on next level of board UNLESS it is the largest board, then end game  
	Increase score

\# End of game  
If player finishes the game or exits:  
	Display final score and player that won  
	Ask if player wants to restart, save, or quit  

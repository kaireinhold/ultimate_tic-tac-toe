\# Initialize game  
Initialize start screen  

\# Start game loop  
When start button pressed:  
    Initialize mode selection screen  
    For each button/option:  
        If selected:  
            Change game parameter to match  
        Else:  
            Use other option or default  

While game is running:  
    Display current score  
    Display board as edited by player-chosen specifications  
    Display current players  
    For each player turn:  
        When player hovers over box:  
            Highlight the box  
        If click input:  
            Place player’s token in grid spot  
            Check for line completion in that box  
            Update score based on completed lines  
            Complete larger line box if possible  
            Change to next player turn  
    If space pressed:  
        If power-up available:  
            Activate power-up (e.g., change token, clear tied/unfinished box, etc.)  
        Else:  
            Alert player that no power-up is available  
    If "pause" or Escape button pressed:  
        Pause game  
        Display save and quit buttons  
        If save button pressed:  
            Save game progress  
        If quit button pressed:  
            Exit current game  

\# Power-up logic  
For each active power-up:  
    Check if power-up is available to current player  
    If available:  
        Trigger corresponding effect (e.g., change token, clear tied/unfinished box, etc.)  
        Remove power-up from player  

\# Check for game over condition  
If grid is full or largest grid has completed line:  
    End game  
    Display "Game Over: Player [winner] won!"  

\# Continue next frame  
Update game screen with new state  

\# Line completion logic  
For each box:  
    If box has completed line:  
        If not the largest board:  
            Change completed box to token on next level of board  
        Else:  
            End game  
        Increase score  

\# End of game  
If player finishes or exits game:  
    Display final score and winner  
    Ask if player wants to restart, save, or quit  

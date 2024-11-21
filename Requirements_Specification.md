**Requirements Specification: Ultimate Tic-Tac-Toe**

**Game Name:** Ultimate Tic-Tac-Toe  
**Team Members:** Kai Reinhold, Andrew Gill  
**Client:** Team  
**Date:** 11/14/24 \- 11/20-22/24

**Game Overview**

	•	**Brief Description:** This is a tic-tac-toe clone, based on the ‘Ultimate’ version with extra abilities. The goal is to win a row in one box, and that box then gets turned into a tile for the next board layer. Each box/board completion earns the player who completed it points. The game has different modes that can be chosen to enhance challenge, skill, and enjoyability.

	•	**Main Goal:** The main goal is to complete as many boards as possible, rack up points, and complete a line in the largest board before the other player. Players will compete to either achieve the highest score and/or complete the largest board.

**Functional Requirements**

	•	**Core Features:**

	•	Classic Tic-Tac-Toe mechanics with a twist.

	•	Power-ups like changing tile placements, clearing random board space/square, Skipping the other person's turn.

	•	Player chooses modes, challenges, and other specifications for each game.

	•	Point tracking to keep track of the amount of boards they cleared.

	•	Save progress feature so players can resume from where they left off.

	•	**User Interactions:**

	•	**Controls:** Mouse for movement and interaction, Space for powerup, Escape for pause.

	•	**Power-up Usage:** Players can activate power-ups using the space key bind when the random power up timer goes down.

	•	**Game Flow:** Players will use a mouse and/or keyboard to start, pause, and interact with the game.

**Non-Functional Requirements**

	•	**Usability:**

	•	The game should be easy to understand with intuitive controls that feel natural.

	•	The layout should be clear with visual indicators for the game state (score, board state, power-up availability).

	•	**Performance:**

	•	The game should maintain a consistent frame rate of 60 FPS.

	•	Load time should be minimal, under 5 seconds.

	•	The game should run smoothly even with multiple players and board levels.

	•	**Cross-Platform Compatibility:**

	•	The game should be accessible on PC and mobile platforms (browser-based or downloadable).

	•	The layout and controls should adapt to different screen sizes.

**Design Requirements**

	•	**Graphics and Visuals:**

	•	Classic-style tic-tac-toe shapes for tokens and graphics.

	•	Smooth animations for power-ups and board completion, with clear visual cues.

	•	Tic-Tac-Toe grid should be simple but visually engaging.

	•	**Audio:**

	•	Upbeat background music to match the gameplay.

	•	Sound effects for power-ups, board/line completion, and game-over events.

	•	Optional sound effects for and score achievements and player turn changes.  
**Data Requirements**

	•	**What Data Needs to be Saved or Tracked:**

	•	player scores, player progress (boards completed, tiles placed), and power-ups used.

	•	Player’s saved game state.

	•	**How Will the Data be Stored:**

	•	Game data will be saved locally for a single session or stored online for players with accounts (if applicable).

	•	High scores and achievements will be stored in an online leaderboard.

**Collaboration with Client**

	•	**How Will You Gather Feedback from the Client in Each Sprint:**

	•	Feedback will be gathered through playtesting sessions with team members, friends/family, and other possible users.

	•	Surveys and direct meetings after each sprint to check progress and adjust features.

	•	**How Will You Ensure the Game is Developing According to the Client’s Needs:**

	•	The development team will conduct regular check-ins to ensure the client’s expectations are being met.

	•	The team will provide demos after major milestones and incorporate feedback to refine gameplay.  

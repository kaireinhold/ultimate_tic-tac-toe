**Test Plan Frame for Your Game**

**Part 1\. Unit Testing the Game Mechanics**

| Test Case | Test Data | Expected Outcome |
| :---- | :---- | :---- |
| Place tile on empty square | Attempt to place tile on empty square, Attempt to place tile on blocked square | When the player's mouse hovers over a square, they should be able to place a tile there only if the square is unblocked. |
| Place attempt in a filled tile | Attempt to place a tile on a filled square will be blocked | If the square is blocked, tile placement should be disabled. |
| Claiming a square  | The first player who does align three tiles in a row gets the square | If the player aligns three matching tiles in a row, they score a point, and the box in which they achieved the match gets marked as won by that player. |

---

**Part 2\. Logic Testing the Game Rules and Calculations**

| Test Case | Test Data | Expected Outcome |
| :---- | :---- | :---- |
| Claimed square | Checks if the square has been claimed if so point are given to the player who claimed it | When a player claims a square, they earn a point and can no longer place anything on that square. |

---

**Part 3\. Boundary Testing: Edge Cases and Limits**

| Test Case | Test Data | Expected Outcome |
| :---- | :---- | :---- |
| Multiple clicks at once | Run multiple clicks | If a player or multiple players click too quickly, the game will process only the first click on a tile, ignoring subsequent clicks.  |
| End game | Tie or win |  The game ends immediately if there's a tie or a winner. |
| No cross matched tiles | Check if there are only matching tiles in a raw for there square | Each square should function independently to ensure no interactions between tiles across different squares. |

---

**Part 4\. Integration Testing: System Interaction**  
**Description:**

| Test Case | Test Data | Expected Outcome |
| :---- | :---- | :---- |
| Point keeping to the player | Track the players points | Ensure points are accurately updated for the player who scores.  |
| Mouse tracking | Track the mouse position | Mouse tracking should be precise, preventing clicks on unintended elements.  |
| Pause or restart | Pause or restart the game | Players should be able to pause the game in single-player mode or multiplayer mode and reset the game if desired. |

---

**Part 5\. Handling Bad Input and Run-Time Errors**  
**Description:**

| Test Case | Test Data | Expected Outcome |
| :---- | :---- | :---- |
| Only left clicks  | Run both clicks  | If both the right and left mouse buttons are clicked simultaneously, the game will prioritize left clicks and ignore right clicks.  |
| Auto save and reset | Run the game to long  | If the game runs for an extended period, it should save progress and reset to ensure smooth performance.  |
| Error messages | Test the game? | Additionally, the game should notify players of any errors and prompt them to restart if necessary. |

---


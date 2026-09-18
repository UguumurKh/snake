# Notes

## What I Did

- Opened the game directly from `index.html` in a browser.
- Played the initial version and checked the game-over and restart flow.

## What I Observed

- Hitting a side stopped the run instead of sending the snake to the opposite side.
- After game over, pressing Space did not restart the game; a mouse click was required.

## What I Asked To Change

- Make the snake wrap through every edge while preserving its current body length.
- Make Space restart immediately after game over.

## Result Of The Fix

- The snake now emerges from the opposite edge when it reaches any side.
- The snake keeps its current length while wrapping.
- Space restarts a finished game immediately and still pauses or resumes an active game.
- Direct browser smoke testing confirmed that crossing an edge no longer shows game over.

## Manual Play-test Result

- Tested and confirmed that the game works as expected.
- The snake moves smoothly and quickly, with responsive changes in direction.

## Implementation

- The game is self-contained in `index.html` and uses no server, build step, or external assets.
- Open `index.html` directly in a browser to play.
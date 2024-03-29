# Continuous Deployment using S3 and Amazon Code Pipeline
A game's code is stored on GitHub. After setting up an S3 bucket to store static websites, we use AWS Code Pipeline to build a continuous deployment pipeline that will automatically push updates to the code whenever they are made.

## The Game
A straightforward matching game for memories.  To see if two cards—images of memes—match, the user clicks them.  The cards vanish from the board if there is a match.  The cards are turned back to their blank side so that the user can try again if there isn't a match.

The game uses JavaScript, CSS, and HTML.

Suggestions for extra features:
- A system for scoring - A timer - More cards
- The ability to play with others so you may compare scores 


## The Deployment Environment
The code will be deployed and hosted in S3.

## The Deployment Pipeline
The pipeline is created using AWS Code Pipeline.  The pipeline pulls the code from GitHub, and deploys it to S3 whenever a change is detected in the code.

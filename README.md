# UnrealEngineAIProject

 Artificial Intelligence Game -Project.
 
This assignment invokes the use of AI behavioural tree with the use of Unreal Engine by Epic
Games in fulfilment of ​Artificial Intelligence for Games ​in Tallinn University, Estonia.

The development team entails.

● Alper Üste

● Gözde Keser

● Oluwafiyikewa Aigbovbioise Alawode

Open with UE4 Editor; Version 4.24

AI Behavioural Traits

This exercise entails 5 AI-controlled characters (bots). They go through six different behaviours based on 4 stages on the game

● Running along a specific set path in a circular motion.

● Collecting objects (represented as coins) randomly generated in the level area

● Running up to behind each other to try landing a sneak/back attack

● Grouping with teammates at safety points


Stage 0 - Before the game start

In this stage, its like the waiting zones in multiplayer games. Before the real game (Stage 1) start, the AI characters chasing the player as long as they see.

Stage 1 - Run, Forest, Run!

This is the first or initial stage when the programme starts, the AI characters are places along a set spline which is circular in this project, and are expected to run laps around the spline. While that point is the active target and they're running towards it, they are also actively searching for the next waypoint to move to after and the cycle continues.

Stage 2 - Collect Coins

Here, 9 coins are spawned randomly on the ground at intervals. The AI characters are required to use their site perception (included in UE4) to seek the objective.
In human fashion, if they can’t get any coin within their view, they turn 180 to look behind to seek the objective. The nearer a coin is to the bot the likelihood the EQS kicks in and the higher the score it receives. The AI then chooses the coin with the highest score.

Stage 3 - Sneak Attack

The AI bots, at this junction, are expected to creep behind other bots and hit them - simulating a sneak attack from the back. The main functionality is similar to the objective sim, with a few exceptions:

 The bot can sneak behind another but once; this is to avoid having it stuck behind one enemy and not moving away so long as the stage is active

Although the character can turn around (like in the objective sim).

The bots need to tun tow commands in the EQS, instead of the one in the coin collection.

● First, it needs to be able to see an enemy in front of it.

● Second, the other bot must be ahead of the attacking bot -. Without this rule, the attack
will be head-on, it would void the attack.

Stage 4 - Retreat with your Ally

This is the last state of the simulation, 2 characters (including the player, making it 6 characters) are assigned a team with matching colours. The bot is expected to choose one of the platforms (savepoint) and stand on it with the corresponding teammate.

To do this, each character first finds their teammate, then they find the nearest End Point to both of them and run to that point. Once they get there, they stand and the points are awarded.

Acknowledgements

AI for Games video playlist by Roman Gorislavski

Note: AI-related blueprints and Behaviour Tree are commented within the project as well.

Video of the project: https://youtu.be/ZWMGwfObRYo

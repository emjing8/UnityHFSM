This project was focused on creating a high-performance AI with a modular (and therefore scalable) hierarchical finite state machine, which also incorporates an A* pathing algorithm using Unity’s navmesh for the movement of the AI itself. In this case, the AI acts as a neutral objective within a game that the player can fight, and the HFSM controls the behavior of the AI and lets it interact dynamically with the player.

The implementation of the HFSM was in C# Unity, including the base class for the states which takes in the state machine and factory as references, classes for all of the states and substates (Aggro, NoAggro, Idle, Return, Move, Attack, Melee Attack, Special Attack) which all handle behavior and transitions within the class itself. 

The A* pathing allows the NPC to keep up with player movement and other dynamic map changes, and it minimizes performance costs for pathing calculations.

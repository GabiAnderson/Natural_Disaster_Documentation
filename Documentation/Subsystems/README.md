# Subsystems Overview

Table of Contents

- [Natural Disaster Subsystems](#natural-disaster-subsystems)
  - [Game Instance](#game-instance)
  - [World](#world)

- [Additional Resources](#additional-resources)

<br>



## Natural Disaster Subsystems

### Game Instance

Subsystems that extend from `UGameInstanceSubsystem` are initialized when the game is launched, and uninitialized when the game is closed.

| Name                                                         | Description                                                  |
| ------------------------------------------------------------ | ------------------------------------------------------------ |
| [Cosmetics Subsystem](./Cosmetics_Subsystem/CosmeticsSubsystem.md) | Subsystem that keeps track of the cosmetic items worn by the butterfly. |

<br>

### World

Subsystems that extend from `UWorldSubsystem` are initialized when a level is loaded, and uninitialized when a level is exited.

| Name                                                         | Description                                                  |
| ------------------------------------------------------------ | ------------------------------------------------------------ |
| [Interaction Subsystem](./Interaction_Subsystem/InteractionSubsystem.md) | Subsystem for keeping track of active interactables.         |
| [Scene Subsystem](./Scene_Subsystem/SceneSubsystem.md)       | Subsystem that keeps track of the current scene & handles scene change events. |

<br>

## Additional Resources

- [Programming Subsystems | Unreal Engine Documentation](https://docs.unrealengine.com/4.27/en-US/ProgrammingAndScripting/Subsystems/)


# Interaction Subsystem

Table of Contents

- [File Details](#file-details)
- [Blueprint Functions](#functions)
  - [Actor Registration](#actor-registration)
  - [Closest Interactable](#closest-interactable)



<br>



## File Details

| Attribute     | Description                                                  |
| ------------- | ------------------------------------------------------------ |
| Files         | `InteractionSubsystem.h`<br />`InteractionSubsystem.cpp`     |
| Source Folder | `/Source/NaturalDisaster/Pubilc/Interaction/`<br />`/Source/NaturalDisaster/Private/Interaction/` |
| Extends       | `UWorldSubsystem`                                            |

<br>

## Blueprint Functions



### Actor Registration

| Signature                                                    | Usage Example                                     |
| ------------------------------------------------------------ | ------------------------------------------------- |
| `void RegisterInteractable(AActor* InteractableActor)`<br /><br />Adds the given actor to the list of active interactables. | ![](images/InteractionSubsystem_Registration.png) |
| `void DeregisterInteractable(AActor* InteractableActor)`<br /><br />Removes the given actor from the list of active interactables. | See above image.                                  |



### Closest Interactable

| Signature                                                    | Usage Example                                        |
| ------------------------------------------------------------ | ---------------------------------------------------- |
| `AActor* GetClosestInteractable(FVector Position)`<br /><br />Returns the actor in the active interactables list that is closest to the given world position. | ![](images/InteractionSubsystem_ClosestActor.png)    |
| `float GetClosestInteractableDistance(FVector Position)`<br /><br />Finds the actor in the active interactables list that is closest to the given world position, and returns the distance between that actor and the given position. | ![](images/InteractionSubsystem_ClosestDistance.png) |






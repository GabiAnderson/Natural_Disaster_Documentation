# Interact Component

[File Details](#file-details)

[Editor Variables](#editor-variables)

[Linking Interact Effects](#linking-interact-effects)



### File Details

| Attribute            | Description                                                  |
| -------------------- | ------------------------------------------------------------ |
| File Name            | `AC_InteractComponent`                                       |
| Containing Folder    | `/Content/Core/Interaction/`                                 |
| Type                 | `Actor Component`                                            |
| Implements           | `BPI_Lockable`, `BPI_Interact_Listener`                      |
| Special Requirements | 1. The actor that owns this component must have a collision component (of any shape). <br> 2. If the Interact Type is `AutoWhenLanded` or `ButtonWhenLanded`, then the parent actor must have a <u>Landing Point Component</u>. |



### Editor Variables

Category: _Interact Settings_

| Name                 | Type            | Description                                                  |
| -------------------- | --------------- | ------------------------------------------------------------ |
| Interact Type        | `EInteractType` | See [Interaction Types](./InteractionTypes.md)               |
| One Time Interaction | `Bool`          | If true, then the component will essentially enter a permanent 'locked' state after it has been triggered once. <br> If false, then the interaction will be able to be triggered multiple times (with no cooldown). |
| Hidden               | `Bool`          | If true, the object will initially be invisible in game, have no collision, and have tick events disabled. |
| Locked               | `Bool`          | If true, the object will initially be unable to be interacted with. |



Category: _Debug_

| Name                                   | Type   | Description                                                  |
| -------------------------------------- | ------ | ------------------------------------------------------------ |
| Debug Print Pawn Overlap               | `Bool` | If true, then will print a line to the screen when a pawn triggers either the BeginOverlap or EndOverlap event in the actor that owns the component. |
| Debug Print Triggered Interact Effects | `Bool` | If true, then will print a line to the screen for each <u>InteractEffect</u> that is triggered when the component is interacted with. |



### Linking Interact Effects

- When the player successfully triggers an interaction, then this component will activate all sibling <u>Interact Effects</u> owned by the parent actor.


# Interact Component

Table of Contents

- [File Details](#file-details)
- [Editor Variables](#editor-variables)
- [Linking Interact Effects](#linking-interact-effects)

<br>

## File Details

| Attribute         | Description                  |
| ----------------- | ---------------------------- |
| File Name         | `AC_LandingPointComponent`   |
| Containing Folder | `/Content/Core/Interaction/` |
| Type              | `Actor Component`            |

<br>

### Usage

- The component will appear in the editor as a translucent pink butterfly - this acts as a preview of where the butterfly will try to land in game.
- You can move, rotate, and scale the component just like any other actor in the editor.
- When landing on the Landing Point, the butterfly pawn will attempt to match the component's location, rotation, and scale directly. 
- A single actor can own more than one landing point component.

<br>

### Triggering Interactions

- If the parent actor contains an [Interact Component](../Interaction_System/InteractComponent.md) with its [Interaction Type](../Interaction_System/InteractionTypes.md) set to either `AutoWhenLand` or `ButtonWhenLand`, then any landing point component on the parent actor can be used to activate the interaction for that object.

<br>
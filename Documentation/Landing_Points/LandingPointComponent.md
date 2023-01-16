# Landing Point Component

Table of Contents

- [File Details](#file-details)
- [Usage](#usage)
- [Triggering Interactions](#triggering-interactions)

<br>

## File Details

| Attribute         | Description                  |
| ----------------- | ---------------------------- |
| File Name         | `AC_LandingPointComponent`   |
| Containing Folder | `/Content/Core/Interaction/` |
| Extends           | `Static Mesh Component`      |

<br>

### Usage

*For a step-by-step walkthrough, see the guide [**Using Landing Points**](../../Guides/LandingPoints/UsingLandingPoints.md).*



Landing Point Components can be added to any actor via the details panel of the editor.


- The component will appear in the editor as a translucent pink butterfly - this acts as a preview of where the butterfly will try to land in game.
- You can move, rotate, and scale the component just like any other actor in the editor.
- When landing on the Landing Point, the butterfly pawn will attempt to match the component's location, rotation, and scale directly. 
- A single actor can own more than one landing point component.

<br>

### Triggering Interactions

- If the parent actor contains an [Interact Component](../Interaction_System/InteractComponent.md) with its [Interaction Type](../Interaction_System/InteractionTypes.md) set to `AutoWhenLand`, then any landing point connected to that same actor can be used to trigger the interaction.

<br>



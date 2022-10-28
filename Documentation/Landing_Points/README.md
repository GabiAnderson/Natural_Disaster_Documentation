# Landing Points

Table of Contents

- [How it Works](#how-it-works)
- [Modules](#modules)

<br>

## How it Works

The landing point system works by adding one or more [Landing Point Components](./LandingPointComponent.md) to any given actor. Once added, the component's preview butterfly can be moved, rotated, and scaled in order to configure where the player pawn will land in game. 

Landing points can also be used as a way to activate [Interact Components](../Interaction_System/IneractComponent.md) that have an [Interact Type](../Interaction_System/InteractionTypes.md) of `AutoWhenLand` or `ButtonWhenLand`.

<br>

## Modules

| Name                                                  | Description                                                |
| ----------------------------------------------------- | ---------------------------------------------------------- |
| [Landing Point Component](./LandingPointComponent.md) | Component used to mark landing points on the owning actor. |
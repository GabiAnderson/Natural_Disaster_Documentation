# Interaction System

Table of Contents

- [How it Works](#how-it-works)

- [Modules](#modules)





## How it Works

The interaction system works primarily through adding actor components to any given actor. First, add an [Interact Component](./InteractComponent.md) to an actor to make it interactable and configure how the interaction should be triggered, then customize what happens as a result of that interaction by adding one or more <u>Interact Effect</u> components to the same actor.



## Modules

| Name | Description |
| ------------- |-------------|
| [Interact Component](./InteractComponent.md) | Component used to make an actor interactable. |
| <u>Interact Effects</u> | A group of components used to specify what should happen as a result of an interaction. |
| [Interaction Types](./InteractionTypes.md) | Enum values that specify how an interaction should be triggered. |

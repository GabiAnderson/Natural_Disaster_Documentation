# List of Pages


- <b>[Landing Points](./Landing_Points/README.md)</b>
  - [Landing Point Component](./Landing_Points/LandingPointComponent.md)
- <b>[Interaction System](./Interaction_System/README.md)</b>
  - [Interact Component](./Interaction_System/InteractComponent.md)
  - [Interaction Types](./Interaction_System/InteractionTypes.md)
- <b>[Subsystems Overview](./Subsystems/README.md)</b>
  - [Cosmetics Subsystem](./Subsystems/Cosmetics_Subsystem/CosmeticsSubsystem.md)
  - [Interaction Subsystem](./Subsystems/Interaction_Subsystem/InteractionSubsystem.md)
  - [Scene Subsystem](./Subsystems/Scene_Subsystem/SceneSubsystem.md)
 


<br>

# Template
When adding documentation for a new feature or updating documentation of an existing feature, please keep this template in mind.

## Step 1 - Create the folders and files
- Create a folder labled `Feature Name`
- Create subfolders within `Feature Name` for sub features labeled `Sub Feature Name`
- Create .md files for each UE file required for the feature (labeled `UEFileX.md`)
- Place these files in the Feature or Sub Feature folder(s) - where they make the most sense
- Create a `README.md` file in the `Feature Name` folder

## Step 2 - Explain the General Flow
Within the `Feature.md` file:
- Briefly explain how the feature works
- List all the files required for this feature with both their UE path and the GitHub path
- Breifly explain the flow the code goes through
- Create diagram/visual way of showing how all the files connect/interact

## Step 3 - Explain Each File
Within each `UEFileX.md` file:
 - Provide what this singular file does
 - Provide what information this files gets from other files
 - Provde what information this file sends to other files
 - Explain any variables used for this file
 - Provide multiple screenshots of the blueprint(s) with an explanation of what each section does

## Step 4 - Show Result
Within the `README.md` file:
- Create a section entintled *Results*
- Post screenshots/videos/gifs of the feature in action

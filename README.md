# DIalogueBoxes
Create Dialogue Boxes in minutes!

# How to implement:
1) Import the DialogueBoxes.unitypackage in your Unity project
2) Create an empty GameObject and add the DialogueSystem.cs script to it
3) Create another empty GameObject as a child of this GameObject.
4) Add the graphics of the dialogue box and the text as a child of the second GameObject.
5) Assign the target Text in the Dialogue Text field in the inspector.
6) Assign the second empty GameObject to the Panel field in the inspector
7) Done!

# How to use:
- You can start using the Dialogue Box System after referencing the DialogueSystem script component in your manager script.
There are many methods you can use.
- You can start adding dialogues:
```csharp
myDialogueSystem.AddDialogue("Hello World!"); // Does not yet display.
myDialogueSystem.AddDialogue("How are you?"); // Does not yet display.
```
- You can then start showing the dialogues one at a time:
```csharp
myDialogueSystem.Show(); // Will open the dialogue box and show "Hello World!"
myDialogueSystem.Show(); // Will open the dialogue box and show "How are you?" after the player clicks the last one.
```
- You can also show all the dialogues you have added:
```csharp
myDialogueSystem.ShowAll(); // Shows all dialogues.
```
- In case you want to stop showing all dialogues you can:
```CSharp
myDialogueSystem.StopShowingAll();
```

# Notes:
- There is an example scene called ExampleScene.unity located inside the Example folder of the package.
- The dialogue box will close if no other dialogues exist.

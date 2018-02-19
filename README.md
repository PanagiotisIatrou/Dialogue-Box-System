# DIalogueBoxes
Create Dialogue Boxes in minutes!

# How to implement:
1) Import the DialogueBoxes.unitypackage in your Unity project
2) Drag the BlackFaderManager prefab to ONLY one scene (usually the first that's loaded)
3) Done!
4) Create an empty gameObject and add the DialogueSystem.cs script to it
5) Create another empty gameObject as a child of this gameObject.
6) Add the graphics of the dialogue box and the text as a child of the second gameObject.
7) Assign the target Text in the Dialogue Text field in the inspector.
8) Assign the second empty gameObject to the Panel field in the inspector
9) Done!

# How to use:
- You can start using the Dialogue Box System after referencing the DialogueSystem script component in your manager script.
There are many methods you can use.
- You can start adding dialogues:
```CSharp
myDialogueSystem.AddDialogue("Hello World!"); // Does not yet display.
myDialogueSystem.AddDialogue("How are you?"); // Does not yet display.
```
- You can then start showing the dialogues one at a time:
```CSharp
myDialogueSystem.Show(); // Will open the dialogue box and show "Hello World!"
myDialogueSystem.Show(); // Will open the dialogue box and show "How are you?" after the player clicks the last one.
```
- You can also show all the dialogues you have added:
```CSharp
myDialogueSystem.ShowAll(); // Shows all dialogues.
```
- In case you want to stop showing all dialogues you can:
```CSharp
myDialogueSystem.StopShowingAll();
```

# Notes:
- There is an example scene called ExampleScene.unity located inside the Example folder of the package.
- The dialogue box will close if no other dialogues exist.

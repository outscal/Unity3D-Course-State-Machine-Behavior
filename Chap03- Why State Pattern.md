## Why State Pattern

### Problem programmers face:

First, all of our logic is now inside this single class.  Attacking, defending, returning home, and any other state we want to create all need to be added here.  This will lead to a big bloated master class for our AI.  It will also make our code more likely to break since we’re editing the same class for every type of logic. 

### State Pattern: A better approach towards implementation

A better approach is to have each state be its own class, generally with a base ‘state’ class that they inherit from.

This way, the character or object only needs to have a reference to its current state and a call to make that state update.  When we want to add a new state, we just create a new class.

>💡 🚀 **[Join Discord Server](https://discord.gg/J5zDscnzms) → Get your doubts solved by experts instantly**
>

## Fundamentals of State Pattern

“Allow an object to alter its behavior when its internal state changes. The object will appear to change its class.”

To understand this better, consider the following example:

- A script that accepts input for movement logic is attached to an in-game entity.
- This class maintains a current state variable which simply references an instance of a state class.
- The input delegates to this current state which handles it and produces the behavior defined within itself. It also handles the required state transitions.

Thus, due to the different states referenced by the current state variable over time, the same script class will seem to behave differently. This is the essence of the State pattern.

In this project, the aforementioned **Character** class is the one that will behave differently due to the various states. But, you want good behavior only!

![](Images/1.png "Flowchart of state pattern")

In general, there are three key points for every state class which help define the overall behavior of the state:

- ***Entry***: This is where you enter the state and do things you only need to do once when you first enter the state.
- ***Exit***: Similar to the Entry, this is where you do any clean-ups you only need to do once before the state changes.
- ***Update Loop***: This is where the core update logic, which executes in every frame, exists. You can divide this into multiple parts such as a loop for physics updates or a loop for handling input.

![](Images/2.png)

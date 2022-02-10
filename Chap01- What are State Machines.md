# What are State Machines

State machines are a concept in which a container(State) stores the status of something at any given time. Then, given an input, it can provide an output based on the current state, transitioning to a new state in the process

## What is a State Pattern

The state pattern is a behavioral software design pattern that implements a state machine in an object-oriented way. This pattern is used in computer programming to encapsulate varying behavior for the same object based on its internal state.

- A Finite State Machine consists of a finite number of states. At a given time only one such state is active.
- Each state defines which state it’ll transition to as an output, based on the sequence of inputs it receives.
- The output state becomes the new active state. In other words, a state transition occurs.

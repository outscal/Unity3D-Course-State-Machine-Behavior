## Advantages and Disadvantages of State Pattern

Advantages are,

1. This pattern is better than the basic if else/switch-based approach in the way that here you think about decomposing your application process into states & divide behaviors into multiple states
2. A state object handles its own behavior & next possible transitions — multiple responsibilities
3. The State pattern minimizes conditional complexity, eliminating the need for if and switch statements in objects that have different behavior requirements unique to different state transitions

Disadvantages are,

1. As transitions are implicitly handled by states themselves, this method is not scalable & in real life, you might end up violating Open Closed - open for extension & closed for modification principal
2. All the state objects implement common behaviors through the interface which really seems unnecessary & extra work in real-life development

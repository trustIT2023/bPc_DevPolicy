# State

```mermaid
classDiagram
  direction BT
  class Context {
      -state
      +Context(initialState)
      +changeState(state)
      +doThis()
      +doThat()
  }
  class State {
      <<interface>>
      +doThis()
      +doThat()
  }
  class ConcreteStates {
      -context
      +setContext(context)
      +doThis()
      +doThat()
  }
  class Client

  Context o--> State
  ConcreteStates ..|> State
  ConcreteStates --> Context
  Client ..> ConcreteStates
  Client --> Context
```

## 引用文献

[引用1](https://github.com/engineer-taro/mermaid_design_pattern)  
[引用2](https://refactoring.guru/design-patterns)  

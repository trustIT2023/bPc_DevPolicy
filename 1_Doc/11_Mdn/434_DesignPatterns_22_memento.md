# Memento

```mermaid
classDiagram
  direction LR
  class Originator {
      -state
      +save() Memento
      +restore(m: Memento)
  }
  class Memento {
      -state
      -Memento(state)
      -getState()
  }
  class Caretaker {
      -originator
      -history: Memento[]
      +doSomething()
      +undo()
  }

  Originator ..> Memento
  Memento <--o Caretaker
```

## 引用文献

[引用1](https://github.com/engineer-taro/mermaid_design_pattern)  
[引用2](https://refactoring.guru/design-patterns)  

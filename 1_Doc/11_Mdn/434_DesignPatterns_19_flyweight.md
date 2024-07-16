# Flyweight

```mermaid
classDiagram
  direction BT
  class FlyweightFactory {
      -cache: Flyweight[]
      +getFlyweight(repeatingState)
  }
  class Context {
      -uniqueState
      -flyweight
      +Context(repeatingState, uniqueState)
      +operation()
  }
  class Flyweight {
      -repeatingState
      +operation(uniqueState)
  }
  FlyweightFactory o--> Flyweight
  Context --> FlyweightFactory
  Context --> Flyweight
  Client *--> Context
```

## 引用文献

[引用1](https://github.com/engineer-taro/mermaid_design_pattern)
[引用2](https://refactoring.guru/design-patterns)

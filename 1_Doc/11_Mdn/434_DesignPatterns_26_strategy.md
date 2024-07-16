# Strategy

```mermaid
classDiagram
  direction BT
  class Client
  class Context{
    -strategy
    +setStrategy(strategy)
    +doSomething()
  }
  class Strategy{
    <<interface>>
    +execute(data)
  }
  class ConcreteStrategies{
    +execute(data)
  }
  Client --> Context: use
  Client ..> ConcreteStrategies: create
  Context o--> Strategy
  ConcreteStrategies ..|> Strategy
```

## 引用文献

[引用1](https://github.com/engineer-taro/mermaid_design_pattern)  
[引用2](https://refactoring.guru/design-patterns)  

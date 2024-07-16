# Mediator

```mermaid
classDiagram
  direction BT
  class Mediator {
      <<interface>>
      +notify(sender)
  }
  class ConcreteMediator {
      -componentA
      -componentB
      -componentC
      -componentD
      +notify(sender)
      +reactOnA()
      +reactOnB()
      +reactOnC()
      +reactOnD()
  }
  class ComponentA {
      -m: Mediator
      +operationA()
  }
  class ComponentB {
      -m: Mediator
      +operationB()
  }
  class ComponentC {
      -m: Mediator
      +operationC()
  }
  class ComponentD {
      -m: Mediator
      +operationD()
  }
  ComponentA --> Mediator
  ComponentB --> Mediator
  ConcreteMediator ..|> Mediator
  ComponentC --> Mediator
  ComponentD --> Mediator
  ConcreteMediator *--> ComponentA
  ConcreteMediator *--> ComponentB
  ConcreteMediator *--> ComponentC
  ConcreteMediator *--> ComponentD
```

## 引用文献

[引用1](https://github.com/engineer-taro/mermaid_design_pattern)  
[引用2](https://refactoring.guru/design-patterns)  

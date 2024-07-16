# Observer

```mermaid
classDiagram
  direction LR
  class Publisher {
      -subscribers: Subscriber[]
      -mainState
      +subscribe(s: Subscriber)
      +unsubscribe(s: Subscriber)
      +notifySubscribers()
      +mainBusinessLogic()
  }
  class Subscriber {
      <<interface>>
      +upgrade(context)
  }
  class ConcreteSubscribers {
      +update(context)
  }
  class Client

  Publisher o--> Subscriber
  ConcreteSubscribers ..|> Subscriber
  Client --> Publisher
  Client ..> ConcreteSubscribers
```

## 引用文献

[引用1](https://github.com/engineer-taro/mermaid_design_pattern)  
[引用2](https://refactoring.guru/design-patterns)  

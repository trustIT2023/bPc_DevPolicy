# ChainOfResponsibility

```mermaid
classDiagram
  direction BT
  class Handler {
      <<interface>>
      +setNext(h: Handler)
      +handle(request)
  }

  class BaseHandler {
      <<abstract>>
      -next: Handler
      +setNext(h: Handler)
      +handle(request)
  }

  class ConcreteHandlers {
      +handle(request)
  }

  BaseHandler o--> Handler
  BaseHandler ..|> Handler
  ConcreteHandlers --|> BaseHandler
  Client --> Handler
```

## 引用文献

[引用1](https://github.com/engineer-taro/mermaid_design_pattern)  
[引用2](https://refactoring.guru/design-patterns)  

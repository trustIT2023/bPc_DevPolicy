# Proxy

```mermaid
classDiagram
  direction BT
  class ServiceInterface {
    <<interface>>
    +operation()
  }
  class Proxy {
    -realService: Service
    +Proxy(s: Service)
    +checkAccess()
    +operation()
  }
  class Service {
    +operation()
  }
  Client --> ServiceInterface
  Proxy ..|> ServiceInterface
  Service ..|> ServiceInterface
  Proxy o--> Service
```

## 引用文献

[引用1](https://github.com/engineer-taro/mermaid_design_pattern)  
[引用2](https://refactoring.guru/design-patterns)  

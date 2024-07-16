# Adaptor

```mermaid
classDiagram
  direction BT
  class Client
  class ClientInterface {
    <<interface>>
    +method(data)
  }
  class Adapter {
    -adaptee: Service
    +method(data)
  }
  class Service {
    +serviceMethod(specialData)
  }
  
  Client --> ClientInterface: use
  Adapter ..|> ClientInterface
  Adapter o-->Service

```

## 引用文献

[引用1](https://github.com/engineer-taro/mermaid_design_pattern)  
[引用2](https://refactoring.guru/design-patterns)  

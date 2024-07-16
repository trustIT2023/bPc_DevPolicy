# DesignPatterns

```mermaid
classDiagram
  direction LR
  class Client
  class Facade {
    -linksToSubsystemObjects
    -optionalAdditionalFacade
    +subsystemOperation()
  }
  class AdditionalFacade {
    +anotherOperation()
  }
  Client --> Facade
  Facade --> AdditionalFacade
```

## 引用文献

[引用1](https://github.com/engineer-taro/mermaid_design_pattern)  
[引用2](https://refactoring.guru/design-patterns)  

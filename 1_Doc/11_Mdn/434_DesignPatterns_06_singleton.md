# Singleton

```mermaid
classDiagram
    direction LR
    class Singleton {
        -Singleton instance$
        -Singleton()
        +getInstance()$ Singleton
    }

    class Client

    Client --> Singleton : use
    Singleton --> Singleton : create, has
```

## 引用文献

[引用1](https://github.com/engineer-taro/mermaid_design_pattern)  
[引用2](https://refactoring.guru/design-patterns)  

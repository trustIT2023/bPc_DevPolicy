# Protorype

```mermaid
  classDiagram
    direction BT
    class Prototype{
      <<interface>>
      +clone() Prototype
    }

    class ConcretePrototype{
      -field1
      +ConcretePrototype(prototype)
      +clone() Prototype
    }

    class SubclassPrototype{
      -field2
      +SubclassPrototype(prototype)
      +clone() SubclassPrototype
    }
    
    class Client
    SubclassPrototype --|> ConcretePrototype
    ConcretePrototype ..|> Prototype
    Client --> Prototype : use
```

## 引用文献

[引用1](https://github.com/engineer-taro/mermaid_design_pattern)  
[引用2](https://refactoring.guru/design-patterns)  

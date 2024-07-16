# Builder

```mermaid
classDiagram
    direction BT
    class Builder {
        <<interface>>
        +reset()
        +buildStepA()
        +buildStepB()
        +buildStepC()
    }

    class ConcreteBuilder1 {
        -Product1 result
        +reset()
        +buildStepA()
        +buildStepB()
        +buildStepC()
        +getResult() Product1
    }

    class ConcreteBuilder2 {
        -Product2 result
        +reset()
        +buildStepA()
        +buildStepB()
        +buildStepC()
        +getResult() Product2
    }

    class Director {
        -Builder builder
        +Director(builder)
        +changeBuilder(builder)
        +make(type)
    }

    class Product1
    class Product2

    Product1 <-- ConcreteBuilder1: create
    Product2 <-- ConcreteBuilder2: create
    ConcreteBuilder1 ..|> Builder
    ConcreteBuilder2 ..|> Builder
    Director o--> Builder
```

## 引用文献

[引用1](https://github.com/engineer-taro/mermaid_design_pattern)  
[引用2](https://refactoring.guru/design-patterns)  

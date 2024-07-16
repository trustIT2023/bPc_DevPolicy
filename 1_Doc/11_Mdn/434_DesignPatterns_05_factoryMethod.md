# FactoryMethod

```mermaid
classDiagram
  direction BT
  class Creator{
    <<abstract>>
    +someOperation()
    +createProduct()* Product
  }
  class Product{
    <<interface>>
    +doStuff()
  }
  class ConcreteCreatorA{
    +createProduct() Product
  }
  class ConcreteCreatorB{
    +createProduct() Product
  }
  class ConcreteProductA{
  }
  class ConcreteProductB{
  }
  
  ConcreteCreatorA --|> Creator
  ConcreteCreatorB --|> Creator
  Creator --> Product : Create 
  ConcreteProductA ..|> Product
  ConcreteProductB ..|> Product
```

## 引用文献

[引用1](https://github.com/engineer-taro/mermaid_design_pattern)  
[引用2](https://refactoring.guru/design-patterns)  

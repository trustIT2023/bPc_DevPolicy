# TemplateMethod

```mermaid
classDiagram
  direction BT
  class AbstractClass{
    <<abstract>>
    +templateMethod()
    +step1()
    +step2()
    +step3()*
    +step4()*
  }
  class ConcreteClass1{
    +step3()
    +step4()
  }
  class ConcreteClass2{
    +step1()
    +step2()
    +step3()
    +step4()
  }
  ConcreteClass1 --|> AbstractClass
  ConcreteClass2 --|> AbstractClass
```

## 引用文献

[引用1](https://github.com/engineer-taro/mermaid_design_pattern)  
[引用2](https://refactoring.guru/design-patterns)  

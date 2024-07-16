# Composite

```mermaid
classDiagram
  direction BT
  class Client
  class Component {
    <<interface>>
    +execute()
  }
  class Leaf {
    +execute()
  }
  class Composite {
    -children: Component[]
    +add(c: Component)
    +remove(c: Component)
    +getChildren() Component[]
    +execute()
  }
  Client --> Component: use
  Leaf ..|> Component
  Composite ..|> Component
  Composite o--> Component 
```

## 引用文献

[引用1](https://github.com/engineer-taro/mermaid_design_pattern)  
[引用2](https://refactoring.guru/design-patterns)  

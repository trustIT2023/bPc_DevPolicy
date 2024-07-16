# Iterator

```mermaid
classDiagram
    direction BT
    class Client
    class Iterator {
        <<interface>>
        +getNext()
        +hasMore() bool
    }
    class IterableCollection {
        <<interface>>
        +createIterator() Iterator
    }
    class ConcreteIterator {
        -collection: ConcreteCollection
        -iterationState
        +ConcreteIterator(c: ConcreteCollection)
        +getNext()
        +hasMore() bool
    }
    class ConcreteCollection {
        +createIterator() Iterator
    }
    Iterator <-- Client: use
    IterableCollection <-- Client: use
    ConcreteIterator ..|> Iterator
    ConcreteCollection ..|> IterableCollection
    ConcreteIterator <--> ConcreteCollection
```

## 引用文献

[引用1](https://github.com/engineer-taro/mermaid_design_pattern)  
[引用2](https://refactoring.guru/design-patterns)  

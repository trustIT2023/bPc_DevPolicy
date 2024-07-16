# Interpreter

```mermaid
classDiagram
  direction LR
  class Client
  class AbstractExpression {
      <<abstract>>
      interpret()*
  }
  class TerminalExpression {
      interpret()
  }
  class NonterminalExpression {
      childExpression
      interpret()
  }
  class Context {
      getInfoToInterpret()
  }

  Client o--> Context
  Client --> AbstractExpression
  NonterminalExpression --|> AbstractExpression
  TerminalExpression --|> AbstractExpression
  NonterminalExpression o--> AbstractExpression
```

## 引用文献

[引用1](https://github.com/engineer-taro/mermaid_design_pattern)
[引用2](https://refactoring.guru/design-patterns)

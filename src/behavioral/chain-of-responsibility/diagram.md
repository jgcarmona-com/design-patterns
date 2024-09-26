```mermaid
classDiagram
    class Handler {
        +Handler nextHandler
        +handleRequest()
    }

    class ConcreteHandler1 {
        +handleRequest()
    }

    class ConcreteHandler2 {
        +handleRequest()
    }

    Handler <|-- ConcreteHandler1
    Handler <|-- ConcreteHandler2
    Handler --> Handler : next
```
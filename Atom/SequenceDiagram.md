https://shd101wyy.github.io/markdown-preview-enhanced/#/diagrams

```mermaid
sequenceDiagram

participant A as Alice
participant J as John
participant B as Bob


A->>J: Hello John, how are you?
loop Healthcheck
    J->>J: Fight against hypochondria
end
Note right of J: Rational thoughts!
Note over A: Check the
J-->>A: Great!
J->>B: How about you?
B-->>J: Jolly good!
```


---



```plantuml

participant participant as Foo
actor       actor       as Foo1
boundary    boundary    as Foo2
control     control     as Foo3
entity      entity      as Foo4
database    database    as Foo5
collections collections as Foo6
queue       queue       as Foo7

participant A as Alice
participant J as John
participant B as Bob

A->>J: Hello John, how are you?
loop Healthcheck
    J->>J: Fight against hypochondria
end
Note right of J: Rational thoughts!
Note over A: Check the
J-->>A: Great!
J->>B: How about you?
B-->>J: Jolly good!
```

---



```mermaid
sequenceDiagram

participant U as Application
participant P as Mod
participant S as Service

Note over U: User initiated a PIS payment
rect rgb(222, 222, 222)
    U->>+P: start( )
        P->>S: hello(credit)
        P->>S: sup(/v2)
        P->>S: Tata(/v3)
        P-->>-U: Adios
    Note over U: Adios
end

```
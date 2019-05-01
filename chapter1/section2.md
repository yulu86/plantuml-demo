## 1.2 声明参与者

- 关键字`participant`用于改变参与者的先后顺序。
- 也可以使用其他关键字来声明参与者：
  - actor
  - boundary
  - control
  - entity
  - database
  - collections

```
@startuml
actor Foo1
boundary Foo2
control Foo3
entity Foo4
database Foo5
collections Foo6

Foo1 -> Foo2 : To bundary
Foo1 -> Foo3 : To control
Foo1 -> Foo4 : To entity
Foo1 -> Foo5 : To database
Foo1 -> Foo6 : To collections
@enduml
```

![](http://www.plantuml.com/plantuml/png/JSwz3G8n3CNntbDu0GhkumeAIYPW0IUNugJ8JygPWksHCKWk__b9Vf5g6Fm0hbJmqbt6sskY2hM1xZ5JKpli2mljObBaR5uhLVJUgXtGqnys8h_5bxlNn3T-WalSpJA7_4QoB26nc64D-CzdseBINpu0)

- 关键字`as`用于重命名参与者
- 可以使用RGB或颜色名修改actor或者参与者的颜色

```
@startuml
actor Bob #red
participant Alice
participant "I have a really\nlong name" as L #99FF99

Alice -> Bob : Authentiation Request
Bob -> Alice : Authentication Response
Bob -> L : Log transaction
@enduml
```

![](http://www.plantuml.com/plantuml/png/LSon2i9040JG_hvYI6e_u2p4M0I4LDOswxaa1vUzUBiH_7kJG43RcJTpLgDYyvWS1Si5b_n0NVZf9YeMGvn834sAWV-Iweg1tWn2OKhfSvUKfOVGo1L8qQ7slcszTsuRut3QhezePXjOB9B5BBZnQsOrjtGhsUmF2hlIAOlophg5TBc75HAbi9el)

- 可以使用关键字`order`自定义顺序来打印参与者

```
@startuml
participant Last order 30
participant Middle order 20
participant First order 10
@enduml
```

![](http://www.plantuml.com/plantuml/png/AqWiAibCpYn8p2jHy4aiBb78Bqf9BL8mDk12bl7DJ4d9IONA6Q7AkMKMmRKP6W00)
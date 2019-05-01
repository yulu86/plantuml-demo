# 1. 时序图

## 1.1 简单示例

-  可以使用`->`绘制参与者之间传递的消息。    
*也可以使用`-->`绘制虚线箭头。此外还能使用`<-`和`<--`，提高可读性。*
```plantuml
@startuml
Bob -> Alice : Authentication Request
Alice --> Bob : Authentication Response

Bob -> Alice : Another Authentication Request
Bob <-- Alice : Another Authetication Response
@enduml
```

![](http://www.plantuml.com/plantuml/png/SyfFKj2rKt3CoKnELR1IS2mjoKZDAybCJYp9pCzJ24ejB4qjBk62IEi25GBLOrDMN92VLvpAnOLkN5u-K64H3cF1gcrqTR4hnp0T0000)

## 1.2 声明参与者

- 关键字`participant`用于改变参与者的先后顺序。
- 也可以使用其他关键字来声明参与者：
  - actor
  - boundary
  - control
  - entity
  - database
  - collections

```plantuml
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


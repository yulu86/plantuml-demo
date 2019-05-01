# 1. 时序图

# 1.1 简单示例

-  可以使用`->`绘制参与者之间传递的消息。    
*也可以使用`-->`绘制虚线箭头。此外还能使用`<-`和`<--`，提高可读性。*
```
@startuml
Bob -> Alice : Authentication Request
Alice --> Bob : Authentication Response

Bob -> Alice : Another Authentication Request
Bob <-- Alice : Another Authetication Response
@enduml
```

![](http://www.plantuml.com/plantuml/png/SyfFKj2rKt3CoKnELR1IS2mjoKZDAybCJYp9pCzJ24ejB4qjBk62IEi25GBLOrDMN92VLvpAnOLkN5u-K64H3cF1gcrqTR4hnp0T0000)


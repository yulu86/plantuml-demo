## 3.1 类之间的关系
- 类之间的关系通过下面的符号定义：
![](symbol.png)

- 使用`..`来代替`--`可以得到点线

```plantuml
@startuml
Class01 <|-- Class02
Class03 *-- Class04
Class05 o-- Class06
Class07 .. Class08
Class09 -- Class10
@enduml
```


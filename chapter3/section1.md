## 3.1 类之间的关系
- 类之间的关系通过下面的符号定义：

![](symbol.png)
*注：组合是强关联；聚集是弱关联。*

- 使用`..`来代替`--`可以得到点线

```
@startuml
Class01 <|-- Class02
Class03 *-- Class04
Class05 o-- Class06
Class07 .. Class08
Class09 -- Class10
@enduml
```

![](http://www.plantuml.com/plantuml/png/SoWkIImgAStDuNBEIImkDZ1KiAdHrLM0S8oWWiOAMd0n4wYOgK8-NCmCAcQkeAS75RA02bagm5GP6d0vfEQb0Aq20000)

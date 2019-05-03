## 1.22 进入和发出消息
- 如果只想关注部分图示，可以使用进入和发出的箭头。
- 使用方括号`[`和`]`表示图示的左、右两侧。

```
@startuml
[-> A: DoWork
activate A

A -> A: Interval Call
activate A

A ->]: Request Created
deactivate A

[<- A: Done
deactivate A
@enduml
```

![](http://www.plantuml.com/plantuml/png/SoWkIImgAStDuOhMjLDmj59moG_FByhcIamkoInBB4bLSEJYSbI0I7dcbQGMbINcA3WdvkHWg8YrKWXABInDBIvHS2vA1KgaSAMa8YkAjj65M92NYYhZa9gN0dG10000)
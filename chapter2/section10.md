## 2.10 从左向右方向
- 默认*从上往下*构建图示

```
@startuml
user1 --> (Usecase 1)
user2 --> (Usecase 2)
@enduml
```

![](http://www.plantuml.com/plantuml/png/SoWkIImgAStDuIejJYqoLD3LjLFG22rEJKuiJbKmr0IB6g6A6cboEQJcfG3r0000)

- 可以用`left to right direction`命令改变图示的方向

```
@startuml
left to right direction
user1 --> (Usecase 1)
user2 --> (usecase 2)
@enduml
```

![](http://www.plantuml.com/plantuml/png/SoWkIImgAStDuSf9JIjHACbNACfCpoXHICaiIaqkoSpFuoejJYqoLD3LjLFG22rEJKuiJbKmr0IB6a54Iw6YHffS3gbvAK2p0000)
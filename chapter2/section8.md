## 2.8 改变箭头方向
- 默认连接是垂直方向的，用`--`表示，可以用一个*横杠*或*点*来表示水平连接

```
@startuml
:user: --> (Use case 1)
:user: -> (Use case 2)
@enduml
```

![](http://www.plantuml.com/plantuml/png/SoWkIImgAStDuR8gBKujibBGrRLJq0WjJbL8JWGIXfemSHHX8qqkXzIy5A0s0000)

- 也可以通过翻转箭头来改变方向

```
@startuml
(Use case 1) <.. :user:
(Use case 2) <- :user:
@enduml
```

![](http://www.plantuml.com/plantuml/png/SoWkIImgAStDuT88BKvLI4u44eQQ2ZPwUWfMfSMfHLP8uaP0SLsOi4DgNWfG6m00)

- 还可以通过给箭头添加`left`，`right`，`up`，`down`等关键字改变方向

```
@startuml
:user: -left-> (dummyLeft)
:user: -right-> (dummyRight)
:user: -up-> (dummyUp)
:user: -down-> (dummyDown)
@enduml
```

![](http://www.plantuml.com/plantuml/png/SoWkIImgAStDuR8gBKujibBGpKbDAz6rKz18AStDhVG1SZJXKaMPwHa8kI0G3o5PMW2N2Ir02AVab-V19Lo074qkXzGy82y70000)
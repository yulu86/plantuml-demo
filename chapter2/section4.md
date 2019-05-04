## 2.4 基础示例
- 用箭头`-->`连接角色和用例
- 横杠`-`越多，箭头越长
- 通过在箭头定义后面加一个冒号即文字的方式来添加标签

```
@startuml
User -> (Start)
User --> (Use the application) : A small label
:Main Admin: ---> (Use the application) : This is\nyet another\nlable
@enduml
```

![](http://www.plantuml.com/plantuml/png/VSin3i8m38NXFQTu8nrwWGoeFG0Ji7LngQLOSjmgTWTk3v6OsTxxf7_oe1PdrVHqRXYlkDox3B_VuRiGXK77eVAYaDq6PCpmIgfGMbbJlf4OvgsAPOp_kaSHX_XYRmwGxL6uBQQqAgU9RJkhVW00)
## 1.3 在参与者中使用非字母符号

-  可以使用引号定义参与者
-  可以使用`as`给参与者定义别名

```
@startuml
Alice -> "Bob()" : hello
"Bob()" -> "This is very\nlong" as Long #FFFF00
Long --> "Bob()" : ok
@enduml
```

![](http://www.plantuml.com/plantuml/png/SoWkIImgAStDuNBCoKnELT2rKr1ooa_Iq5HIi5B8ICt9oUU2yi5I8HcPnGf0L9PQL1cJbvEVbwwaa5Yiu0DaA2Yx0O610HUOeujYK7usbqDgNWhG6W00)
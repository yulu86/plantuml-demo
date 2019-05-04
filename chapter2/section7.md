## 2.7 构造类型
- 使用`<<`和`>>`来定义角色或者用例的构造类型

```
@startuml
User << Human >>
:Main Database: as MySql << Application >>
(Start) << One Shot >>
(Use the application) as (Use) << Main >>

User -> (Start)
User --> (Use)

MySql --> (Use)
@enduml
```

![](http://www.plantuml.com/plantuml/png/HOv12eCm54JtESKiww8N40aMkkX6kWWzm6yRC12ZDTz5RwyJ1PT_vl7cjrbbrcM8vfNzZAR1OnaamLfJTn8IxgBobknhI4RtTxz8w3PDCNn4mrZGYwEbOlDC7guVjSIR4zfxo8bNzB0eD2T8xkjNYyDqt0o86hCldq7hqtVxUWK0)
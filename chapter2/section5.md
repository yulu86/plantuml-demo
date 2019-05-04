## 2.5 继承
- 如果一个角色或者用例继承于另一个，可以用`<|--`表示

```
@startuml
:Main Admin: as Admin
(Use the application) as (Use)

User <|-- Admin
(Start) <|-- (Use)
@enduml
```

![](http://www.plantuml.com/plantuml/png/SoWkIImgAStDuRBoJSpCKt1CoStCir98B8Qmk3H2YrCLIZ9I5H8B2d8oanDBClFpD47I80bDBYuWMQHWKwEh2rCV339F4om4LUEGcfS2j000)
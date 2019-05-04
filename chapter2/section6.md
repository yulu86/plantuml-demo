## 2.6 使用注释
- 可以使用以下关键字给一个对象添加注释：
    - `note left of`
    - `note right of`
    - `note top of`
    - `note bottom of`
- 注释还可以通过`note`关键字来定义，然后用`...`连接其他对象。

```
@startuml
:Main Admin: as Admin
(Use the application) as (Use)

User -> (Start)
User --> (Use)
Admin ---> (Use)

note right of Admin: This is an example.
note right of (Use)
    A note can also
    be on serveral lines
end note

note "This note is connection\nto serveral objects." as N2
(Start) .. N2
N2 .. (Use)
@enduml
```

![](http://www.plantuml.com/plantuml/png/LL2nKWGX3EtvYZTNtHPIN7c5S_S1NgDsDZaskZXiiWFe-Fa6H9rZ64ZUI_9ud4gbN3_Mv8uF50NdUOro19MVoEsV2wCk3Dgs50FLg38rkX6JStPctDrZ_zZcJ2DlGEVx4Cl_02TQ6Jc-BHNw-YltjCG2soJWBrgtnFwsS7J3rXcT2LPBgMZ7hWmLcFGdPqf8KRWubhcN3irT5-cXtK55E3GtBrBrlrMlxmONlsiUBmStVC7xbbqE5eotd6o-_Tit)
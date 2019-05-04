## 2.2 角色
- 角色用两个冒号包裹起来
- 也可以用`actor`来定义角色，用`as`来定义别名

```
@startuml
:First Actor:
:Another\nactor: as Men2
actor Men3
actor :Last actor: as Men4
@enduml
```

![](http://www.plantuml.com/plantuml/png/SoWkIImgAStDuR9ooomgBb5mJ2x9BxBYidBCoo_9I2sAoKi42oWa5YlufkOPSO6v8AOnb6dbamZKXgBAXCiXDIy5Q2W0)
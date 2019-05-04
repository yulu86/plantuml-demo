## 2.11 显示参数
- 用`skinparam`改变字体和颜色
- 可以在如下场景中使用：
    - 在图示的定义中
    - 在引入的文件中
    - 在命令行或者ANT任务提供的配置文件中
- 也可以给构造的角色和用例指定特殊颜色和字体

```
@startuml
skinparam handwritten ture
skinparam usecase {
    BackgroundColor DarkSeaGreen
    BorderColor DarkSlateGray

    BackgroundColor<< Main >> YellowGreen
    BorderColor<< Main >> YellowGreen

    ArrowColor Olive
    ActorBorderColor black
    ActorFontName Courier

    ActorBackgroundColor<< Human >> Gold
}

User << Human >>
:Main Database: as MySql << Application >>
(Start) << One Shot >>
(Use the application) as (Use) << Main >>

User -> (Start)
User --> (Use)

MySql --> (Use)
@enduml
```

![](http://www.plantuml.com/plantuml/png/VP31JeD048Rl-nHpb8Clq3IajOrugJqG3nwdC94DomxEpaeQuxlR1H98QZpoVn__FzbTK1IDdJEXjRv7mGuQzFKWLfKyQ1HQeHYema3mRG00dh1gFuIZhm_iME28qfQ4XH3vIM2fILRGeL8XU3L__R_TmWcjXpo7TtAEXxkYVwnHsulmCCsTdVsYAQoKPNt9nTrs5_JCNb-n8pXm54jY5dH_u4liSDmksDNcnvYtG08hO3RZTKTKl62W3M20qxNyT4dQzxsp5QhbKNqe5KMpHCwUe6nOn_ZM2TeGuA9dgIU139O7cDSVSvYRvkyK9DMOQNa9TkJhsBbV)
## 1.25 包裹参与者
- 可以使用`box`和`end box`画一个盒子将参与者包裹起来。
- 还可以在`box`关键字后添加标题或者背景颜色。

```
@startuml
box "Internal Service" #009900
participant Bob
participant Alice
end box
participant Other

Bob -> Alice: hello
Alice -> Other: hello
@enduml
```

![](http://www.plantuml.com/plantuml/png/SoWkIImgAStDuKhAhr1GyimhIItAIynH24ujAijCJbLIK3OmiBGqCE0g02hBJCuiICmhKN3AJqBXE-O0bNAbvgKe00r1aV4loKWjuk82Qb3GjOEeirB8ICt9oUS2Su2Y43KmKGUWAK3N0000)
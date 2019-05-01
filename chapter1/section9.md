## 1.9 分割示意图
- 关键字`newpage`用于把一张图分割成多张
- 在`newpage`后添加文字，作为新的示意图的标题

```
@startuml
Alice -> Bob : message 1
Alice -> Bob : message 2

newpage

Alice -> Bob : message 3
Alice -> Bob : message 4

newpage A title for the\nlast page

Alice -> Bob : message 5
Alice -> Bob : message 6
@enduml
```

![](http://www.plantuml.com/plantuml/png/SoWkIImgAStDuNBCoKnELT2rKt3AJrAmKiXDBIvEJ4zLCCGbOSJ5bPTQNW1aSk5IOenBmWIkLy5HeIIp92TL8Is_IA4a8pKcBoUnk4G1hx6ck2JCk1nIyrA0dW40)
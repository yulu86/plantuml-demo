## 1.23 构造类型和圈点
- 可以使用`<<`和`>>`给参与者添加构造类型.
- 在构造类型中，可以使用`(X, Color)`格式的语法添加一个圆圈圈起来的字符。

```
@startuml
participant "Famous Bob" as Bob << Generated >>
participant Alice << (C, #ADD1B2) Testable >>

Bob -> Alice: First Message
@enduml
```

![](http://www.plantuml.com/plantuml/png/SoWkIImgAStDuIe0qfd9cGM9UIKAIcw9kVcbnGfE-KbA2ebWMi76Hi4zDI-rAB4aDKN1pWv5lMDEPd8gI8M6iuw2igEBYw6JaQP2I2hGyAISL91gBf0HkdOGbLOARfb5nIKAlgd5nOdfgLmEgNafG2S00000)
## 1.27 外观参数
- 用`skinparam`改变字体和颜色。
- 可以在如下场景中使用：
    - 在图示的定义中
    - 在引入的文件中
    - 在命令行或者ANT任务提供的配置文件中
- 也可以修改其他渲染元素

```
@startuml
skinparam sequenceArrowThickness 2
skinparam roundcorner 20
skinparam maxmessagesize 20
skinparam sequenceParticipant underline
skinparam handwritten true

actor User
participant "First Class" as A
participant "Second Class" as B
participant "Last Class" as C

User -> A: DoWork
activate A

A -> B: Create Request
activate B

B -> C: DoWork
activate C
C --> B: WorkDone
destroy C

B --> A: Request Created
deactivate B

A --> User: Done
deactivate A
@enduml
```

![](http://www.plantuml.com/plantuml/png/POy_JmCn3CLtVmghUoNKiGDgxYec1iGVCLk9HQFUESNEKU3JSuPAvDGrlzzxBzvP9QtJE80Tivn8QKJZzuabSb0jv-T3ZaTXCzmqYfP9KYmghBYvQS18d-CiqnjR_cPdrxqFf3N7V2AfEDUm3bcuyGuawQovLXQiEZ40nLeKNumLJaruTPVLAlO3cQsG3CCIFt4iaXhUBVazBT8zW4_W-XR35lVbjUZHf_C7LSO041nrM-oL_UNHxx7whtG0dIlzTRg77jT_QGVx8Wnf3clvyjtEeQzUEYyJQNRQzl2h-ITzGRZ50NOiQHg77m00)
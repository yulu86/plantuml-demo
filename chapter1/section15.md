## 1.15 分隔符
- 可以通过`==`关键字来将图表分割多个步骤
```
@startuml
== Initialization ==
Alice -> Bob: Authentication Request
Bob --> Alice: Authentication Response

== Repetition ==
Alice -> Bob: Another Authentication Request
Bob -> Alice: Another Authentication Response

@enduml
```

![](http://www.plantuml.com/plantuml/png/VOz13i9024NtSmekq0kOO5ftRht1M4aa6Q6MFnjFBz4ODzObUGzU60DrHR-rman7KsXj-gXGDs8kKzDPQDZJmSyxcZgkOj3vpKzoxn8eoMX8voN_i69n2obPo64HwCPryrnS_rQ-aItv4nl5BldM4m00)
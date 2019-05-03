## 1.28 填充区设置
- 可以设置填充区的参数设置。

```
@startuml
skinparam ParticipantPadding 20
skinparam BoxPadding 10

box "Foo1"
participant Alice1
participant Alice2
end box

box "Foo2"
participant Bob1
participant Bob2
end box

Alice1 -> Bob1: hello
Alice1 -> Out: out
@enduml
```

![](http://www.plantuml.com/plantuml/png/PSon3e8m4CRn_PxYmcv2Ep8OP72LLoYqqSPhhu5hmkFRQ0nLrl_Tx-jNCOlaGB0-VKncCG77Klpiauao6cjzlADkg_l0sxUh5c3Y3PihiseWxH8lv6UdZac3YnOBsgN-bGDFwZzKwZECf_FxiSE78-Agth9qo5cWBoG7UW40)
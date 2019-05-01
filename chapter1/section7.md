## 1.7 对消息序列编号
- 关键字`autonumber`用于自动对消息编号

```
@startuml
autonumber
Bob -> Alice : Authentication Request
Alice --> Bob : Authentication Reqsponse
@enduml
```

![](http://www.plantuml.com/plantuml/png/SoWkIImgAStDuKeiBSdFAyrDIYtYSifFKj2rKt3CoKnELR1IS2mjoKZDAybCJYp9pCzJ24ejB4qjBk62IEi25GBLOrLMN92VLvpAvP2QbmAq0G00)

- `autonumber` *start*用于指定编号的初始值
- `autonumber` *start* *increment*可以同时指定编号的初始值和每次增加的值

```
@startuml
autonumber
Bob -> Alice : Authentication Request
Alice --> Bob : Authentication Reqsponse

autonumber 15
Bob -> Alice : Another Authentication Request
Alice --> Bob : Another Authentication Reqsponse

autonumber 40 10
Bob -> Alice : Yet Another Authentication Request
Alice --> Bob : Yet Another Authentication Reqsponse
@enduml
```

![](http://www.plantuml.com/plantuml/png/SoWkIImgAStDuKeiBSdFAyrDIYtYSifFKj2rKt3CoKnELR1IS2mjoKZDAybCJYp9pCzJ24ejB4qjBk62IEi25GBLOrLMN92VLvpAXMIqWg4fXkbv-K1zHKJRWb1Es3OJ0mL30tGB8rDBIB8KeeMmnGwfUId0W0G0)

- 可以在双引号内指定编号的格式
*编号是由java的`DecimalFormat`类实现的，也可以使用HTML标签来指定格式*

```
@startuml
autonumber "<b>[000]"
Bob -> Alice : Authentication Request
Alice --> Bob : Authentication Reqsponse

autonumber 15 "<b>(<u>##</u>)"
Bob -> Alice : Another Authentication Request
Alice --> Bob : Another Authentication Reqsponse

autonumber 40 10 "<font color=red><b>Message 0 "
Bob -> Alice : Yet Another Authentication Request
Alice --> Bob : Yet Another Authentication Reqsponse
@enduml
```

![](http://www.plantuml.com/plantuml/png/bOun2y9034Rt-nMXNNGeNa4NgGTrTt4JSMXhr8DwqRla_nli8bImpddvtck4ASYznGXPrRgZjVQKcIsrK3YeUzyXhA4Mlc5WtpNiAS0UduA9pN0k55J-AvOU518Qys4fLs_Hh1ANvzL2t7oi2wH3SR9smAVfbnPAgmKN2WmTzHGt4SzEYtQOKdD5i30AEY3_6wKlFyDU)

- 可以使用`autonumber stop`和`autonumber resume` *increment* *format* 来表示暂停或继续使用自动编号
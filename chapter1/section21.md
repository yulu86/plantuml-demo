## 1.21 创建参与者
- 可以把`create`放在第一次收到消息前，以强调本次消息实际上是在创建新的对象。
*即对象的生命周期是从new开始的。*

```
@startuml
Bob -> Alice : hello

create Other
Alice -> Other: new

create control String
Alice -> String
note right: You can also put notes!

Alice --> Bob : ok
@enduml
```

![](http://www.plantuml.com/plantuml/png/FOv1hi8m34JtFiNy0_mBP84A5s31YcK8LXjXREGuuleqbThbQDwJtjGYU_ItqCKU-3_XBBKm4XOMCQBYd8DnZOMTjcz0sqnG_Xv4CGqtmIsywdoW-rOBXjTvYOIxTPIioD8CdnuOP_kZNLgj4PDWBvfOdslT3m00)
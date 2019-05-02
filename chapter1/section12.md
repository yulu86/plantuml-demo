## 1.12 其他注释
- 可以使用以下关键字在节点相应位置放置注释:
  - `note left of`
  - `note right of`
  - `note over`
- 可以通过修改背景色来高亮显示注释

```
@startuml
participant Alice
participant Bob
note left of Alice #aqua 
This is displayed
left of Alice.
end note

note right of Alice: This is displayed right of Alice
note over Alice: This is displayed over Alice.
note over Alice, Bob #FFAAAA: This is displayed\n over Bob and Alice.

note over Alice, Bob
This is yet another
example of 
a long note.
end note
@enduml
```

![](http://www.plantuml.com/plantuml/png/TOz1he8m48RtSuf9sBvmWBS25vp0fPkH3j1aQ6ifHcvlcqOHH4BIflDzV-Qlfa0-pAE0YwTkjICJi1RTykRbPAzWR60KxWBQBYDOq6qcXFEW9uo_qfCJMbZ11Yk1ZSAaGmxnkX_MyJz--JiYM_RE_hUnJiiz_fVMnw9fwlWTk1UJuKIHKQ-KmvXtruK3KYG6zi0F6frmsXS8nPe-jVtiNSNRFCeJ)
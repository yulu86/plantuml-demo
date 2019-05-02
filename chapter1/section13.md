## 1.13 改变备注框的形状
- 可以使用`hnote`和`rnote`关键字来修改备注框的形状

```
@startuml
caller -> server : conReq
hnote over caller: idle
caller -> server: conConf
rnote over server
  "r" as rectangle
  "h" as hexagon
endnote
@enduml
```

![](http://www.plantuml.com/plantuml/png/POun3i8m34Ltd-AhEnVeW2fn0suGfPy6oTZ22OZZaxG30zlJiv_qbzfIjDT39ITL1avdLCQxqupiTkLJYdaZVBZZQSPzLVuLUt1nkqdyYkCam1GJKaKmjsIRSgYogy9Fsjo4jevEbWvzqHS0)
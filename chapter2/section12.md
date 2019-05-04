## 2.12 一个完整的例子

```
@startuml
left to right direction
skinparam packageStyle rectangle
actor customer
actor clerk
rectangle checkout {
    customer -- (checkout)
    (checkout) .> (payment) : include
    (help) .> (checkout) : extends
    (checkout) -- clerk
}
@enduml
```

![](http://www.plantuml.com/plantuml/png/NOzD2i8m44RtESMth8jwW2waT_04Gpgs8Jy9oGGiujsDbhRWyl4UypCMeIpLE-Nu8P28REP5C9dCMamCgbWJ4cNoIAGjpNoNrJ6-ciBiM96McA5haUWvx-WuMtL4q0jh6wlWfG0SDVeUtUukFtKYhZTqYLRFeS404xIh4s_LmYvjnTaFuATmcCh_eBPbE-YjnkRRkny0)
## 1.16 引用
- 使用`ref over`关键字来实现引用

```
@startuml
participant Alice
actor Bob

ref over Alice, Bob: init
ref over Bob
    this can be on
    serveral lines
end ref
@enduml
```

![](http://www.plantuml.com/plantuml/png/HOt13G9124NlLF4Bi09Fgvsm8qQI4JQ0rY-Z1q-GznvXo-AertFIqLE77co5ozGXnACySFMTAEGEVqlyp6d1CzIq_cPr050FJGmsx0AtBqg9BdXYgacIs0rzHbil_Va3)
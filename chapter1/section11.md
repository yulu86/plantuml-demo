## 1.11 给消息添加注释
- 通过在消息后面增加`note left`或者`note right`关键字来给消息增加注释
- 也可以通过`end note`添加多行注释

```
@startuml
Alice -> Bob : hello
note left: this is a first note

Bob -> Alice : ok
note right: this is another note

Bob -> Bob: I'm thinking
note left
a note
can also be defined
on serveral lines
end note
@enduml
```

![](http://www.plantuml.com/plantuml/png/LOyn3i8m34Ltd-9lJ5mW0ofi72DjtIQgwqY9uVmuoW18bcnzloVBKxDOxNKAtIKlZEiDZp8Z8B588It64Duim59ky8hOScs6lYBgi3j33YZ7K6hUqw_ZOUBwxtWBU5xEJkcHTVzUepZG9IgYj8APiVAMbLSgYiRrpJKAn9D6hEl09v_ybGy0)
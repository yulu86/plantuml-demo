## 1.17 延迟
- 使用`...`关键字来表示延迟，并且可以添加注释

```
@startuml
Bob -> Alice: Authentication Request
...
Alice -> Bob: Authentication Response
...5 minutes later...
Bob -> Alice: Bye
@enduml
```

![](http://www.plantuml.com/plantuml/png/SoWkIImgAStDuNBAJrBGjLDmpCbCJhLIS2mjoKZDAybCJYp9pCzJ24ejB4qjBk7IqzFZ0gi0AGNgmAAmk20_hpWLfD9K8JSphxGajLWX9x4ajGWeWcQ9KsKgbqDgNWhGUW00)
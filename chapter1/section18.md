## 1.18 空间
- 可以使用`|||`增加空间
- 还可以指定空间的像素

```
@startuml
Bob -> Alice: Authentication Request
Alice -> Bob: Authentication Response
|||
Bob -> Alice: Another Authentication Request
Alice -> Bob: Another Authentication Response
||45||
Bob -> Alice: Yet Another Authentication Request
Alice -> Bob: Yet Another Authentication Response
@enduml
```

![](http://www.plantuml.com/plantuml/png/SoWkIImgAStDuNBAJrBGjLDmpCbCJhLIS2mjoKZDAybCJYp9pCzJ24ejB4qjBk42ouAK0LLZKLHSa9zNdCfLKrE3RbnUFb1f4J76mXNZCTx45CE6oDGIKcm1Qo1eaqDgNWemR000)
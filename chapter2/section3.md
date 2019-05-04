## 2.3 用例描述
- 如果想定义跨越多行的用例描述，可以用双引号将其包裹起来。
- 还可以使用分隔符:
    - `--`
    - `..`
    - `==`
    - `__`
*注：可以在分隔符中间放置标题。*

```
@startuml
usecase UC1 as "You can use
several lines to define your usecase.
You can also use separators.
--
Several separators are possible.
==
And you can add titles:
..Conclusion..
This allows large description."
@enduml
```

![](http://www.plantuml.com/plantuml/png/HOz1IWOn34RtESN7lv-2Ms5WP8wWBbp6DceXDaFIAjxU3eou2o-y1zyMdRsFJwKHaZa4p_iTE71xiO7C3PDJo9SuAxGs2NH3aRTvuiU6un8J_HciOIT5oC7EtJmIBGizNfL_37R1OH7rLMTWNUcXbLczEgMWrwuIzvJIRYthY6ej9Nhwg5DMjU-0ihyBYaJsUlJpVwDDMfcZVW40)
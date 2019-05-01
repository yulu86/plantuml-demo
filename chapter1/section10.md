## 1.10 组合消息
- 可以通过以下关键字组合消息：
    - alt/else
    - opt
    - loop
    - par
    - break
    - critical
    - group, 后面紧跟着消息内容
- 可在`header`添加需要显示的文字
  关键字`end`用来结束分组
  *注意：分组可以嵌套使用*

```
@startuml
Alice -> Bob : Authentication Request

alt Successful case

Bob -> Alice : Authentication Accepted

else Some kind of failures

Bob -> Alice : Authentication Failure

group My own label
Alice -> Log : Log attack start
    loop 1000 times
        Alice -> Bob : DNS attack
    end
Alice -> Log : Log attack end
end

else Another type of failure
    Bob -> Alice : Please request
end
@enduml
```

![](http://www.plantuml.com/plantuml/png/XP11JiGm34NtFiM_05BPia1JX5W1GlG4cTGTed7ZaZX2StlIqCMe266ftlI_BxySihbaPHRg9NZ6pJqUz8WxzCK-E5hmpe96lFDduMn4JWn3yPvpdeh0kyn4ArB9Ll6RxMjwCHw9M39Zq9bn3d64JfXSa98u_zVnz9CZEYKj2rukqAy8SKU-klnPJvLSjpDp_emcHwWZgWjkkww3XPapOPkTzUFhiB4jmN7ykxtzhT-crKUj5oVOPU4hizQpStiJTfL8svkk7OUwoYpV)
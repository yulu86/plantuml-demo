# 1. 时序图

## 1.1 简单示例

-  可以使用`->`绘制参与者之间传递的消息。    
*也可以使用`-->`绘制虚线箭头。此外还能使用`<-`和`<--`，提高可读性。*
```
@startuml
Bob -> Alice : Authentication Request
Alice --> Bob : Authentication Response

Bob -> Alice : Another Authentication Request
Bob <-- Alice : Another Authetication Response
@enduml
```

![](http://www.plantuml.com/plantuml/png/SyfFKj2rKt3CoKnELR1IS2mjoKZDAybCJYp9pCzJ24ejB4qjBk62IEi25GBLOrDMN92VLvpAnOLkN5u-K64H3cF1gcrqTR4hnp0T0000)

## 1.2 声明参与者

- 关键字`participant`用于改变参与者的先后顺序。
- 也可以使用其他关键字来声明参与者：
  - actor
  - boundary
  - control
  - entity
  - database
  - collections

```
@startuml
actor Foo1
boundary Foo2
control Foo3
entity Foo4
database Foo5
collections Foo6

Foo1 -> Foo2 : To bundary
Foo1 -> Foo3 : To control
Foo1 -> Foo4 : To entity
Foo1 -> Foo5 : To database
Foo1 -> Foo6 : To collections
@enduml
```

![](http://www.plantuml.com/plantuml/png/JSwz3G8n3CNntbDu0GhkumeAIYPW0IUNugJ8JygPWksHCKWk__b9Vf5g6Fm0hbJmqbt6sskY2hM1xZ5JKpli2mljObBaR5uhLVJUgXtGqnys8h_5bxlNn3T-WalSpJA7_4QoB26nc64D-CzdseBINpu0)

- 关键字`as`用于重命名参与者
- 可以使用RGB或颜色名修改actor或者参与者的颜色

```
@startuml
actor Bob #red
participant Alice
participant "I have a really\nlong name" as L #99FF99

Alice -> Bob : Authentiation Request
Bob -> Alice : Authentication Response
Bob -> L : Log transaction
@enduml
```

![](http://www.plantuml.com/plantuml/png/LSon2i9040JG_hvYI6e_u2p4M0I4LDOswxaa1vUzUBiH_7kJG43RcJTpLgDYyvWS1Si5b_n0NVZf9YeMGvn834sAWV-Iweg1tWn2OKhfSvUKfOVGo1L8qQ7slcszTsuRut3QhezePXjOB9B5BBZnQsOrjtGhsUmF2hlIAOlophg5TBc75HAbi9el)

- 可以使用关键字`order`自定义顺序来打印参与者

```
@startuml
participant Last order 30
participant Middle order 20
participant First order 10
@enduml
```

![](http://www.plantuml.com/plantuml/png/AqWiAibCpYn8p2jHy4aiBb78Bqf9BL8mDk12bl7DJ4d9IONA6Q7AkMKMmRKP6W00)

## 1.3 在参与者中使用非字母符号

-  可以使用引号定义参与者
-  可以使用`as`给参与者定义别名

```
@startuml
Alice -> "Bob()" : hello
"Bob()" -> "This is very\nlong" as Long #FFFF00
Long --> "Bob()" : ok
@enduml
```

![](http://www.plantuml.com/plantuml/png/SoWkIImgAStDuNBCoKnELT2rKr1ooa_Iq5HIi5B8ICt9oUU2yi5I8HcPnGf0L9PQL1cJbvEVbwwaa5Yiu0DaA2Yx0O610HUOeujYK7usbqDgNWhG6W00)

## 1.4 给自己发消息

- 参与者可以给自己发消息
- 消息文字可以用`\n`来换行

```
@startuml
Alice -> Alice :  "This is a signal to myself.\nIt also demostrates\nmultiline\ntext"
@enduml
```

![](http://www.plantuml.com/plantuml/png/9Son2i9G38NXlKznwAuFu21rT7UyIx1H0qakDAUWR--5mZ_yqxSKPUCUFjtSdehJ5STSWFdniS98KFPESR0ZVgN-EhUy4-BLiMhquYRKQXcxqznIMrA_dAT5Sntw7m00)

## 1.5 修改箭头样式
有以下几种方式：
 - 一条丢失的消息：末尾加`x`
 - 箭头只有上半部分或下半部分：将`<`和`>`替换成`\`或者`/`
 - 细箭头：将箭头标记写两次，如`>>`或`//`
 - 虚线箭头：用`--`替代`-`
 - 箭头末尾加圈：`->o`
 - 双向箭头：`<->`

 ```
 @startuml
 Bob ->x Alice
 Bob -> Alice
 Bob ->> Alice
 Bob -\ Alice
 Bob \\- Alice
 Bob //-- Alice
 Bob ->o Alice
 Bob o\\-- Alice
 Bob <-> Alice
 Bob <->o Alice
 @enduml
 ```

 ![](http://www.plantuml.com/plantuml/png/Kt3AJrBGjQjGSCp9J4xbWd9HUQZS66HUJ8mkCbTVNrSNLMy-CZS_9WPLtWRLAXiazGwfUIcbkJa0)

 ## 1.6 修改箭头颜色
- 可以用以下记号修改箭头颜色：

```
@startuml
Bob -[#red]> Alice : hello
Alice -[#0000ff]-> Bob : ok
@enduml
```

![](http://www.plantuml.com/plantuml/png/SoWkIImgAStDuNBAJrBGZLOkIas9jLDmpCbCJbMmKiX8pSd9vmBpG986G92M5gjhfm1K3PJEp-PoICrB0Me70000)

## 1.7 对消息序列编号
- 关键字`autonumber`用于自动对消息编号

```
@startuml
autonumber
Bob -> Alice : Authentication Request
Alice --> Bob : Authentication Reqsponse
@enduml
```

![](http://www.plantuml.com/plantuml/png/SoWkIImgAStDuKeiBSdFAyrDIYtYSifFKj2rKt3CoKnELR1IS2mjoKZDAybCJYp9pCzJ24ejB4qjBk62IEi25GBLOrLMN92VLvpAvP2QbmAq0G00)

- `autonumber` *start*用于指定编号的初始值
- `autonumber` *start* *increment*可以同时指定编号的初始值和每次增加的值

```
@startuml
autonumber
Bob -> Alice : Authentication Request
Alice --> Bob : Authentication Reqsponse

autonumber 15
Bob -> Alice : Another Authentication Request
Alice --> Bob : Another Authentication Reqsponse

autonumber 40 10
Bob -> Alice : Yet Another Authentication Request
Alice --> Bob : Yet Another Authentication Reqsponse
@enduml
```

![](http://www.plantuml.com/plantuml/png/SoWkIImgAStDuKeiBSdFAyrDIYtYSifFKj2rKt3CoKnELR1IS2mjoKZDAybCJYp9pCzJ24ejB4qjBk62IEi25GBLOrLMN92VLvpAXMIqWg4fXkbv-K1zHKJRWb1Es3OJ0mL30tGB8rDBIB8KeeMmnGwfUId0W0G0)

- 可以在双引号内指定编号的格式
*编号是由java的`DecimalFormat`类实现的，也可以使用HTML标签来指定格式*

```
@startuml
autonumber "<b>[000]"
Bob -> Alice : Authentication Request
Alice --> Bob : Authentication Reqsponse

autonumber 15 "<b>(<u>##</u>)"
Bob -> Alice : Another Authentication Request
Alice --> Bob : Another Authentication Reqsponse

autonumber 40 10 "<font color=red><b>Message 0 "
Bob -> Alice : Yet Another Authentication Request
Alice --> Bob : Yet Another Authentication Reqsponse
@enduml
```

![](http://www.plantuml.com/plantuml/png/bOun2y9034Rt-nMXNNGeNa4NgGTrTt4JSMXhr8DwqRla_nli8bImpddvtck4ASYznGXPrRgZjVQKcIsrK3YeUzyXhA4Mlc5WtpNiAS0UduA9pN0k55J-AvOU518Qys4fLs_Hh1ANvzL2t7oi2wH3SR9smAVfbnPAgmKN2WmTzHGt4SzEYtQOKdD5i30AEY3_6wKlFyDU)

- 可以使用`autonumber stop`和`autonumber resume` *increment* *format* 来表示暂停或继续使用自动编号

## 1.8 页面标题、页眉和页脚
- 使用`title`关键字增加页面标题
- 使用`header`和`footer`关键字增加页眉和页脚

```
@startuml
header 这是页眉
footer 图 %page% of %lastpage%

title Example title

Alice -> Bob : message 1
Bob -> Alice : message 2
@enduml
```

![](http://www.plantuml.com/plantuml/png/SoWkIImgAStDuSf8JKn9BL9uiN_cindhNoxS-dnE9rTQVdu9KEpfx7qAgWM9wQcg2lbf2gevYSKbO1uNLqbcIKwgWcj5Ocu1a0RpkBWSSpAJKnLqxHISyfCKh1HoKukBWQeL3Bc0V90mH1uXOSJba9gN0dG30000)

## 1.9 分割示意图
- 关键字`newpage`用于把一张图分割成多张
- 在`newpage`后添加文字，作为新的示意图的标题

```
@startuml
Alice -> Bob : message 1
Alice -> Bob : message 2

newpage

Alice -> Bob : message 3
Alice -> Bob : message 4

newpage A title for the\nlast page

Alice -> Bob : message 5
Alice -> Bob : message 6
@enduml
```

![](http://www.plantuml.com/plantuml/png/SoWkIImgAStDuNBCoKnELT2rKt3AJrAmKiXDBIvEJ4zLCCGbOSJ5bPTQNW1aSk5IOenBmWIkLy5HeIIp92TL8Is_IA4a8pKcBoUnk4G1hx6ck2JCk1nIyrA0dW40)

## 1.9 组合消息
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

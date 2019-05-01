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
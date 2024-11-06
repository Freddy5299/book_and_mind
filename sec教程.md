## sec基本

- 深度优先 和广度优先
- 可扩展性，可以使用自定义的apps和相应的property
- unit level simulation
  - high rtl to designers
- 死代码 cdc 计数器溢出 fsm活锁死锁
- 可以关闭lighting



## 基本命令

- clean -all
- analyze -sv12 rtl.v
- elaborate -top arch -parameter WIDTH 4 -create_related_covers {precondition witness}
- clock clk
- reset rst

- debug功能
  - window
    - Visualize Window
      - Reset Analysis
  - 双击波形可以调出源码
  - 双击源码可以遍历源码
  - 可以点击源码
    - 找到需要分析的端口，点击Visualize下的Visualize
      - 波形分析，点击Highlight Relevant Logic
  - 运行下几个时钟周期
  - 信号添加，可以直接点放大镜旁边那个键，使用通配符搜索
  - 当我们一个信号的链路比较长的花，可以点击modify value
  - quite trace
    - 减少了信号活动，对于不熟悉设计代码的人很有用
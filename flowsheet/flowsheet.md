
#Flowsheet架构

> 功能目的制作Web的flowsheet 需求提出方 圣泰 附件（模型、例题）
>
> 文档编写负责人 Long, Huilong 修订 Rev 发布时间 修订内容 1 2016.12.9 讲述了flowsheet的架构 2


#### **Flowsheet Demo**
![DEMO](../images/001.jpg)

>Flowsheet有两种模式，一种是添加模式，另一种是拖拽模式。

` `
** 添加模式：**
* 可以添加stream，block	
* 添加一个block后，进入拖拽模式
* Stream添加后依然是添加模式

` `
** 拖拽模式：**
* 拽stream进行重新连接block
* 拖动stream和block
* 对stream的局部线条进行位置调整
* 移动block的时候，会移动连接的stream。

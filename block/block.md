##Block
###Port
**类型：**

* 入口: 物流线的终点箭头连接的port，当物流连接到port上时，箭头是从外指向block的。
* 出口：物流线的起始箭头连接的port，当物流连接到port上时，箭头变成了直线。

**方向：**

` `从上到下，从下到上，从左到右，从右到左，以block为中心。
可见的port和隐藏的port：

` `当需要连接block的outlet port时，显示可见的outlet port，它应该显示在hidden port的下面，但因为hidden port是透明的，所以给用户一个错觉，认为物流连接的是visible port，其实连接的hidden port。当需要连接block的inlet port时，也是一样。
###移动
` `当鼠标在block按下时，在block上创建一个svg的矩形，这个矩形会覆盖原来的block，但因为这个矩形是透明的，会给用户一个错觉，认为是在block上加了一个外边框。当鼠标移动时，矩形会按照鼠标的位置不断的进行重绘。当鼠标松开时，会重新绘制block，并且绘制block连接的所有物流。
###水平翻转
水平翻转时，hidden port和image桶是翻转，与它连接的线也要做翻转。它的visible port在显示的时候，需要按照翻转后的位置重新计算。
###垂直翻转
水平翻转。
###旋转90度
` `当用户点击旋转按钮时，block会进行顺时针90度的旋转，它的hidden port也会随着旋转。它连接的stream需要重绘，以及visible port的位置需要按照旋转后的位置进行计算。

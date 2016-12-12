##Stream与Block的连接
###删除Stream
` `当删除stream时，会把原来的stream设置为空，但并不把它移除。
###删除Block
` `删除block时，把block设置为空，并不是把它移除。
##软件架构(Controller-ModelView)
` `可以把flowsheet分成3个controller，一个flowsheetcontroller，来控制整个flowsheet的事件，同时记录当前block，stream，以及他们的连接信息。一个flowsheetblockcontroller，主要控制所有block，以及block的添加、删除。一个flowsheetstreamcontroller，主要控制所有的stream， 添加，拖动，拽动，移动，删除。

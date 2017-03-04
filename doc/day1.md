#position css属性选择用于定位元素的替代规则，被设计为对动画效果有用
#top,right,bottom,left属性确定定位元素的位置
#static 该关键字指定元素使用正常的布局行为，即元素在文档流中当前的布局位置。此时 top, right, bottom, left 和 z-index 属性无效。
#relative 相对定位 该关键字下，元素先放置在未添加定位时的位置，再在不改变页面布局的前提下调整元素位置（因此会在此元素未添加定位时所在位置留下空白）。position:relative 未定义对 table-*-group, table-row, table-column, table-cell, table-caption 元素应用的效果。
#absolute 绝对定位 不为元素预留空间，通过指定元素相对于最近的非 static 定位祖先元素的偏移，来确定元素位置。绝对定位的元素可以设置外边距（margins），且不会与其他边距合并。
#fixed 固定定位 不为元素预留空间，而是通过指定元素相对于屏幕视口（viewport）的位置来指定元素位置。元素的位置在屏幕滚动时不会改变。打印时，元素会出现在的每页的固定位置。fixed 属性会创建新的栈上下文。当元素祖先的 transform  属性非 none 时，容器由视口改为该祖先。
#绝对定位 相对定位的元素并未脱离文档流，而绝对定位的元素则脱离了文档流。在布置文档流中其它元素时，绝对定位元素不占据空间。绝对定位元素相对于最近的非 static 祖先元素定位。当这样的祖先元素不存在时，则相对于根级容器定位。

.clearfix {  overflow: auto;}  清除浮动
.clearfix {  overflow: auto;  zoom: 1;} 兼容IE6 清除
display 是CSS中最重要的用于控制布局的属性。每个元素都有一个默认的 display 值，这与元素的类型有关。对于大多数元素它们的默认值通常是 block 或 inline 。一个 block 元素通常被叫做块级元素。一个 inline 元素通常被叫做行内元素。
#div 是一个标准的块级元素。一个块级元素会新开始一行并且尽可能撑满容器。其他常用的块级元素包括 p 、 form 和HTML5中的新元素： header 、 footer 、 section 等等。
inline span 是一个标准的行内元素。一个行内元素可以在段落中 <span> 像这样 </span> 包裹一些文字而不会打乱段落的布局。 a 元素是最常用的行内元素，它可以被用作链接。
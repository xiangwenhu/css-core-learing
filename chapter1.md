## 遇见未知的CSS

* 浏览器五种样式来源
  * 属性style
  * 标签style
  * link
  * 浏览器用户自定义样式
  * 浏览器默认样式
优先级
1. 浏览器默认样式
2. 浏览器用户自定义一般样式
3. 一般样式
4. 一般样式 !important
5. 浏览器用户自定义样式 !important
6. 权重比较
7. 权重相同，后面的优先   
[
CSS样式的五种来源及浏览器默认样式](https://blog.csdn.net/u013778905/article/details/52886938)

* CSS命名，按照用意命名
```css

size-10{
    font-size:10px //X
}

size-small{
    font-size:10px //ok
}
```

* pointer-events 穿透   
  
元素永远不会成为鼠标事件的target。但是，当其后代元素的pointer-events属性指定其他值时，鼠标事件可以指向后代元素，在这种情况下，鼠标事件将在捕获或冒泡阶触发父元素的事件侦听器。
说明：只能屏蔽鼠标事件，不能屏蔽键盘事件例如tab和enter，屏蔽事件也不是永久，后代指定属性时可能在冒泡时会有影响。

demo
<iframe height="265" style="width: 100%;" scrolling="no" title="pointer-events 穿透" src="//codepen.io/xiangwenhu/embed/MLbYBR/?height=265&theme-id=0&default-tab=js,result" frameborder="no" allowtransparency="true" allowfullscreen="true">
  See the Pen <a href='https://codepen.io/xiangwenhu/pen/MLbYBR/'>pointer-events 穿透</a> by dirge
  (<a href='https://codepen.io/xiangwenhu'>@xiangwenhu</a>) on <a href='https://codepen.io'>CodePen</a>.
</iframe>

[pointer-events|MDN](https://developer.mozilla.org/zh-CN/docs/Web/CSS/pointer-events)  
[pointer-events: none 的两个应用场景](https://www.cnblogs.com/zichi/p/9068481.html)      


* 利用padding实现等比例缩放
  

* calc函数
运算符可以是 + - * /， 但需要注意运算符前后保留一个空格。
* 隐藏元素
* 设置width:0, height:0, 必要时设置font-size:0, background-color
* opacity
* 移出屏幕, 例如position:absolute, left: -9999px
* text-indent
* z-index, 必要时background-color
* overflow:hidden隐藏溢出部分
* visibility
* display:none
* backgound-color:transparent; font-size:0
* tranform:ranslate
* tranform:scale
* tranform:skew
* margin-left负值
* clip-path
  
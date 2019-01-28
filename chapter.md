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

[pointer-events: none 的两个应用场景](https://www.cnblogs.com/zichi/p/9068481.html)
# 基于 HTML Canvas 的简单画板
#### 1. 基于: HTML5 + JavaScript.

#### 2. 功能: 五种颜色(红黄蓝绿黑) 五种画笔(1 2 4 8 16px) 橡皮擦以及另存为.

#### 3. 参考: 
- csdn博客: [【JavaScript】基于H5 canvas实现的画板绘图工具](https://blog.csdn.net/a727911438/article/details/71037450?utm_source=itdadao&utm_medium=referral)  (参考了 画线 部分)
- github: [linhongbijkm/canvasPainter](https://github.com/linhongbijkm/canvasPainter) (copy了 另存为 部分) 
> ps 同一个作者的不同代码.

#### 4. 说明: 
- 学习html第二天做的小项目,功能是后面一项一项加上去的,代码显得有些凌乱.没有CSS,后续学习了会来补充.
- 已知bug: 鼠标不放开的时候点击清空画布失效.
- IE和Eage并不支持download标签,在这两个浏览器上不能使用另存为功能.
- 只测试了Firefox.

#### 5. 笔记
- 创建button可以使用&lt;button&gt;标签也可以使用&lt;input type="button"&gt;
- &lt;select>标签可以用onchange来指定变化方法,&lt;option&gt;可以使用selected="selected"来指定默认值.
- canvas 的 lineCap 设置或返回线条末端线帽的样式.
- canvas 的 lineJoin 属性设置或返回当两条线交汇时所创建边角的类型.
- canvas 可以使用 clearRect(x,y,width,height) 方法来清空画布.

|类型 | 基于 |
|:---:|:---:|
|event.clientX | 鼠标相对于浏览器窗口可视区域的X，Y坐标 |
|event.pageX | 同e.clientX 但使用的是文档坐标而非窗口坐标(非标准属性) |
|event.offsetX | 鼠标相对于事件源元素（srcElement）的X,Y坐标 |
|event.screenX | 鼠标相对于用户显示器屏幕左上角的X,Y坐标 |

图解:![pic](https://images2015.cnblogs.com/blog/1009007/201702/1009007-20170223112832882-336762012.png)


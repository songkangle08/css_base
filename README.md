## svg
- svg指可伸缩矢量图形（Scalable Vector Graphics）
- SVG用来定义网络的基于矢量的图形
- SVG使用XML格式定义图形
- SVG图像在放大或改变尺寸的情况下器图形质量不会有所损失（这个是重点）
- SVG是万维网联盟的标准

### SVG的优势
- SVG图像可通过文本编辑器来创建和修改
- SVG图像可悲搜索，索引，脚本化或压缩
- SVG是可伸缩的
- SVG图像可在任何的分辨率下被高质量的打印
- SVG可在图像质量不下降的情况下被放大
### 浏览器支持
- ie9以上


## background
### linear-gradient线性渐变
- linear-gradient()函数用于创建一个表示两种或多种颜色性渐变的图片
```css
body{
    background：linear-gradient(color-stop1,color-stop2,...);
    background: linear-gradient(direction,color-stop1,color-stop2,...);     // 方向
    background: linear-gradient(angle,color-stop1,color-stop2,...);         // 角度
}
```

### radial-gradient径向渐变
- radial-gradient()函数创建来一个图片，其由一个原单辐射开的在两个或多个颜色之前的渐变组成。
```css
body{
    background：radial-gradient(color-stop1,color-stop2,...);
    background：radial-gradient(closest-side,color-stop1,color-stop2,...);
    background：radial-gradient(circle at 100%,color-stop1,color-stop2,...);
    background：radial-gradient(ellipse at top,color-stop1,transparent),
                radial-gradient(circle at bottom,color-stop1,transparent)
}
```

### background-size 背景尺寸
- 检索或设置对象的背景图像的尺寸大小
- 该属性提供2个参数值（特性值cover和contain）
- 如果提供两个，第一个用于定义背景图像的宽度，第二个用于定于背景图像的高度
- 如果只提供一个，该值用于定义背景图像的宽度，第2个值默认为auto，即高度为auto，此时的背景图以提供的宽度作为参照来进行等比缩放
- 取值情况：length，percentage（百分比），auto，cover，contain

#### cover，contain的区别
- cover： 宽高同时等比例缩放，可能会出现裁剪
- contain：高度或宽度一个达到盒子的100%就停止缩放，可能会出现留白的状态。
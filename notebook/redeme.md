# 介绍

关于本人

    笔者系大四学生，此笔记是笔者在学习前端的时候的一些知识点  
    就此开始内容吧
# 内容
## HTML
### 1. 什么是HTML？

    HTML的全称为超文本标记语言，是一种标记语言。它包括一系列标签．通过这些标签可以将网络上的文档格式统一，使分散的Internet资源连接为一个逻辑整体。HTML文本是由HTML命令组成的描述性文本，HTML命令可以说明文字，图形、动画、声音、表格、链接等。

### 2. html语言的语法
   
      <标签>实体内容</标签>
   
      <标签 属性="属性的值">实体内容</标签>
   
      <标签 属性1="属性1的值" 属性2="属性2的值">实体内容</标签>
   
      备注：属性的值外面可以使用双引号，可以使用单引号，也可以不使用引号。规范是使用双引号

### 3. HTML标签的嵌套
   
      <标签1>
      <标签2></标签2>
      </标签1>

### 4. 特殊的标签

   单标签，就是不成对的标签

   <标签 />

  整体框架标签:

    <!doctype html>     
    html    规定，所有html的内容都必须写在该标签内
    head    头部标签，规定了文档的一些规范和页面显示内容无关的内容
        title 页面标题标签，为了给SEO优化做准备，其中他是整个页面对SEO优化效果最强的部分
        <meta charset="UTF-8" />   字符集编码格式
            UTF-8   国际字符集编码格式
            GBK     国家标准扩展包
            GB2312  国家2312标准
        <meta name="description" content="">   网站描述
    body    身体标签，所有页面显示内容都应该写在body中
        文本标签类型：
            文本/文章标题标签    h1-h6
                1. 从h1-h6字体逐渐变小
 
                2. 每个h标签独占一行
 
                3. 每个h标签之间存在一个间隙
 
                4. 一般情况下，使用的时候，一个页面只能有一个h1标签
 
                5. h4-h6一般不使用，在汉语还是英语的语法结构中，不存在4级标题
 
                6. h标签是加粗状态的
 
            段落标签  p
                1. 每个p标签独占一行
 
                2. p标签不会前面空两个
 
                3. 每个p标签之间存在间隙
 
            粗体标签   b
                1. b标签不会独占一行
 
                2. b标签没有专门的SEO效果
 
            粗体标签(SEO) strong
                1. strong不会独占一行
 
                2. 他对SEO有优化效果
 
            斜体标签    i
                1. i标签不会独占一行
 
                2. 他对SEO没有优化效果
 
            斜体标签(SEO) cite
                1. cite不会独占一行
 
                2. 他对SEO有优化效果
 
            斜体标签(SEO) em
                1. em不会独占一行
 
                2. 他对SEO有优化效果
 
            居中标签   center
            字体标签   font
                size   设置字体大小
                    取值范围是1-7的整数
                color   设置字体颜色
        列表标签
            无序列表   ul
                需要配合li进行使用
            有序列表   ol
                配合li进行使用
            自定义列表  dl
                配合dt和dd标签进行使用，具体定义某个事物的标签
        表格标签     table
            border  设置表格边框的属性，一般使用1。在不同的浏览器中，颜色和外形不同
            align   设置表格的水平对齐方式
                center  
                left
                right
            bgcolor 设置表格的背景颜色
        表头标签   th
        行标签     tr
        单元格标签  td
        表单标签    
            form    表单标签本身
                action  设置表单的url地址，用户数据向哪里提交
                method  设置表单提交的方式，一般是GET/POST
                    GET提交方式，数据是通过地址栏进行提交的，是可见的
                    POST提交方式，数据无法从地址栏看到
            input   输入框标签
                type    设置输入框的类型
                    text    文本输入框
                    password    密码输入框
                    radio   单选输入框，如果要实现单选，每个输入框的name属性必须一致
                    email   邮箱输入框
                    color   颜色输入框
                    time    时间输入框
                    datetime-local    日期输入框
                    checkbox    多选输入框
                    number  数字输入框
                        step    跳步属性，设置点击箭头数字如何变化
                value   设置input框的值
                name    设置和后台提交的时候的字段名称
                placeholder 设置input标签的提示信息
                required    设置input标签必须填写的属性，没有属性值
                maxlength   设置input标签的最大输入长度
            select  下拉菜单
                需要配合option标签进行使用
            textarea    文本域标签
        br      换行
        hr      水平线
        图片标签   img
            src     资源属性，用来指引图片所在的地址
            alt     图片描述属性(IE中alt可以起到title的作用)
            title   图片描述属性
            备注：在工作中，更多图片需要配合懒加载进行使用
        超链接标签(锚点) a
            href    设置超链接跳转的地址
            target  设置a标签连接的页面的打开方式
                _blank  重新打开一个新的标签，显示页面
                _self   覆盖当前页面 

### 5. HTML的颜色制式
```   
   1. 英文单词模式:red,blue,cyan,gray

   2. rgb()模式:  rgb(红色值，绿色值，蓝色值)

      每种颜色的取值范围是0-255
   3. rgba()模式： rgba(红色值，绿色值，蓝色值，透明度/亮度/色彩饱和度)

      亮度的取值范围是0-1的小数
   4. #红色值绿色值蓝色值，十六进制颜色表示方式，HEX模式

      每种颜色的取值范围仍然是0-255，但是需要用16进制进行表示
      rgba(255,0,100,0.8)   -> #FF0064
```
## CSS
### 1. 在head标签中使用css
```
    <style>
        css代码
    </style>
```

### 2. 使用link标签，从外部引入css文件
``` 
   <link rel="stylesheet" href="css文件地址">
 ```

### 3. 在标签中间，使用style属性，书写css
```
   <p style="font-size:50px" >123</p>
```
### 4.选择器
```
就是给页面上的哪个标签添加样式

1. element 元素选择器

   element就代表一个标签名称，你可以使用该选择器选中页面上的所有的该标签

2. *   通用选择器

选中页面上的所有元素，添加样式

一般用来重置浏览器样式的

3. class(类)选择器

   首先，在标签中，使用class="类名"的方式，添加属性

   然后，在css部分，可以使用.类名的形式，添加样式

4. id选择器

   首先，在标签中，使用id="id名"的方式，添加属性

   然后，在css部分，可以使用#类名的形式，添加样式

5. element element  关系选择器

   外部元素 内部元素的方式，选中内部元素

6. element,element  组合选择器

   同时选中好几个元素，添加样式

7.  :hover  伪类选择器

    鼠标移入的时候，发生什么情况
```
### css属性
#### background 背景属性

    background-color    设置元素的背景颜色
    
    background-image    设置元素的背景图片
    
        background-image:url("图片地址");
    
    background-repeat   设置元素的背景图片的重复方式
    
        no-repeat   不重复
     
        repeat-x    横向重复
     
        repeat-y    纵向重复
    
    background-position 设置元素的背景图片的位置属性
    
        属性值是: 横向坐标 纵向坐标
    
    background-size   设置元素的背景图片的大小
    
        属性值是：宽度 高度
    
    background-attachment   背景图片绑定属性
    
        fixed   把背景图片绑定在网页的相对高度上
    
    background  背景综合属性
    
        可以把color,image,position,repeat这四个属性写在一起
#### 字体属性

    font-size   设置字体大小
    
        属性值为长度单位
        px  像素
        em  一个汉字的大小(具体需要根据该标签的字体大小来设置)
        %   百分比
        rem 通过JS进行设置的相对单位，一般指一个汉字的大小
        ex  一个英文字母x的大小
        color   设置字体的颜色
    
        只能设置单纯的颜色值，而不能设置线性渐变
        font-weight 设置字体的粗细
    
        bold    字体加粗
        800     字体加粗
        normal  正常
        font-style  设置字体风格
    
        italic  斜体
        oblique 斜体
        normal  正常
        font-family 设置字体类型:黑体，宋体等等
#### 文本属性
    
    text-align  设置文本的水平对齐方式
    
        center  居中对齐
     
        left    靠左对齐
     
        right   靠右对齐
    
    line-height 设置文本的一行的高度
    
        属性值是长度单位
     
        备注：该属性是设置字体垂直居中的，然后不对图片生效
    
    text-decoration 设置文本修饰属性
    
        none    没有修饰
     
        underline   下划线
     
        overline    上划线
     
        line-through    删除线
    
    text-indent 设置首行缩进属性
    
        属性值是长度单位，这里可以使用em
    
    text-shadow 设置文本阴影
    
        四个属性值，用空格分隔：横向位移 纵向位移 模糊程度 颜色
#### 边框属性

    border  设置元素的边框
    
        border-style    设置边框的风格
     
            solid   单实线
     
            double  双实线
     
            dashed  虚线
     
        border-color    设置边框的颜色
     
        border-width    设置边框的宽度
    
    border-radius   设置边框的圆角属性
    
    outline 设置元素的轮廓线
#### transition 过渡属性

    一共有四个属性值：过度的属性，过渡的时间，过渡的方式，延迟的时间
    
    过渡方式:
    
        linear  线性过渡
        ease    平滑过渡
        ease-in 由快到慢
        ease-out    由慢到快

#### transform 变换属性

    rotate()    旋转
    
        括号里面填入角度值，deg代表度数，rad代表弧度
    
    translate(横向坐标，纵向坐标) 平移
    
    scale()     缩放
    
    skew(横向扭曲角度,纵向扭曲角度)      扭曲
    
    如果要想让页面拥有Z轴，那么需要给页面一个深度
    
    perspective 透视属性
    
    如果元素参与变换，那么会被强制转化回2D效果，如果要保持3D效果，需要给该元素的父元素添加:
    
    transform-style:preserve-3d;
    
    opacity    设置元素的透明度，0-1的一个小数
#### margin 外间距
    
    就是设置元素之间的距离的属性
    
    margin-top
    
    margin-bottom
    
    margin-left
    
    margin-right
    
    margin可以设置多个值：
    
    当margin有一个值的时候，四个方向是一个值
    
    当margin有两个值的时候，第一个值是上下方向，第二个值是左右方向
    
        对于独占一行的元素，可以使用margin:上下值 auto的方式让他水平居中
    
    当margin有三个值的时候，第一个值是上方，第二个值是左右方向，第三个值是下方
    
    当margin有四个值的时候，按照顺时针方向，分别为上右下左
#### HTML元素的分类
    
    独占一行的元素:div,h1,p,li等等，这一类的标签一般称之为块状元素，可以设置宽度和高度，如果没有设置宽度和高度，那么宽度自动为100%，高度为0。内部元素会自动撑开他的高度
    
    不会独占一行的元素:a,span,b,i等等，这一类的标签一般称之为行内元素，不可以设置宽度和高度，他的宽高是由里面的文字撑起来的
#### padding 内间距
    
    不是用来调整位置的，而是用来填充元素，使其面基扩大的
    
    padding-top
    
    padding-bottom
    
    padding-left
    
    padding-right
    
    padding可以设置多个值：
    
    当padding有一个值的时候，四个方向是一个值
    
    当padding有两个值的时候，第一个值是上下方向，第二个值是左右方向
    
    当padding有三个值的时候，第一个值是上方，第二个值是左右方向，第三个值是下方
    
    当padding有四个值的时候，按照顺时针方向，分别为上右下左
#### flex 弹性盒子
    
    display 设置元素的显示方式
    
        none    元素不显示
        block   将元素转化为块状元素
        inline  将元素转化为行内元素
        flex    将元素转化为弹性盒子
    justify-content 设置弹性盒子内部元素的水平排列方式
    
        flex-start  元素从左到右排列
        flex-end    元素从右向左排列
        center      所有元素居中排列
        space-between   两端对齐
        space-around    平均分布
    flex-wrap   设置弹性盒子内部元素是否可以换行
    
        nowrap  不允许元素换行
        wrap    元素可以换行
    flex-direction  设置弹性盒子内部元素的排列方式
    
        row 横向排列
        row-reverse 反向横向排列
        column   纵向排列
        column-reverse  反向纵向排列
    align-items 设置弹性盒子内部元素的垂直排列方式
    
        flex-start  靠上排列
        flex-end    靠下排列
        center  居中排列
        baseline    水平线排列
    order   设置弹性盒子内部元素的顺序
#### 渐变属性
##### 线性渐变
    这是一个属性值，兼容性不太好
    
    linear-gradient(方向,第一个颜色,第二个颜色 位置,第三个颜色 位置.....)
    
    需要添加浏览器实验性前缀
    
        -webkit-   谷歌/苹果浏览器(360浏览器和QQ浏览器的极速模式)
        -ms-       微软浏览器(IE不一定支持)
        -o-        欧朋浏览器
        -moz-      火狐浏览器
##### 径向渐变
    
    radial-gradient(形状,第一个颜色，第二个颜色，第三个颜色....)
    
    形状:circle 表示圆形，ellipse 表示椭圆形
#### 动画属性
    
    animation-name  指定动画的名称
    
    animation-duration  动画的播放时间
    
    animation-timing-function   动画播放的方式
    
        linear 线性播放
     
        ease   平滑播放
     
        cubic-bezier(n,n,n,n)   自定义贝塞尔曲线
    
    animation-delay 设置动画的延迟时间
    
    animation-iteration-count   设置动画的播放次数
    
        infinite    无限次
    
    animation-direction     设置动画是否反向
    
        alternate   反向
#### left 浮动

    浮动的元素会脱离标准文档流
    
    clear   可以清除浮动，当前元素不要受到上面元素的浮动的影响
    
        clear:left ,clear:right, clear:both
    
    多页面/pc端页面一般推荐使用浮动进行布局，单页面/手机端页面，推荐使用弹性盒子布局
#### position 定位
    
    static  静态定位
    
    fixed   绑定定位
    
        当元素添加绑定定位之后，原来的位置就不在占有了。这种情况叫做：脱离标准文档流
        坐标点的参考系是按照网页窗口为参考点的
    relative    相对定位
    
        相对定位不会让元素脱离标准文档流
        相对定位的坐标点的参考系是：就是他原来的位置
    absolute    绝对定位
    
        绝对定位会让元素脱离标准文档流
        绝度定位的参考点：首先找他的父级是否有定位属性，如果他的父级有定位属性，那么以他的父级为参考点。如果父级没有定位属性，那么找他的父级的父级是否有定位属性。
        以此类推，直到找到html标签为止，如果都没有定位属性，那么以页面的最左上角为参考点
#### 音视频标签
##### audio 音频标签
    
    如果想在页面上看到音频标签，那么需要添加控制面板属性: controls
    
    autoplay    自动播放属性，该属性在谷歌浏览器中不允许被自动播放，但是该属性只支持谷歌浏览器

[更多内容](https://www.runoob.com/tags/ref-av-dom.html)
##### video 视频标签

    如果需要显示控制面板，需要添加controls属性
    
    autoplay    自动播放属性
    
    poster      设置视频的封面

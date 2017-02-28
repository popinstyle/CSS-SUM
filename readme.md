1.盒模型: 外边距 , 边框 , 内边距 , 元素的内容。
2.全局reset是类似于一下的样式:
body,div,dl,dt,dd,ul,ol,li,h1,h2,h3,h4,h5,h6,pre,code,form,fieldset,legend,input,button,textarea,p,blockquote,th,td{
	margin:0;
	padding:0;
	outline:none;
}
3.元素的总尺寸是指:
	content + padding + border + margin
4.css3的box-sizing属性可以定义需要何种盒模型;
5.外边距叠加:(发生在普通文档流中 块 框垂直外边距才会发生外边距叠加)
	当两个或更多的外边距相遇时,他们将形成一个外边距。这个外边距等于两个发生叠加的外边距的高度中的较大者。(不管是嵌套的还是相邻的元素)

							可视化格式模型
6.p,div,h1-h6都是块级元素。(块框)   span,strong 是行内元素。(行内框)
7.在使用相对定位时，无论元素是否移动，元素仍然占据原来的空间。移动该元素会覆盖其他元素。
8.相对定位相对于元素咋文档流的初始位置,绝对定位相对于距离他最近的已定位的祖先元素。

9.让背景图片垂直居中的方法:
	<div class="background"></div>
	.background{
		width:300px;
		height:50px;
		background:url(images.png) no-repeat center;
	}
10.圆角边框实现有两种办法：border-image,border-radius;
11.实现阴影效果:(photoshop的滤镜和图像)
	(1)	<div class="wrap"><img src=""/></div>
	.wrap{
		background:url(shadow.gif) no-repeat bottom right;
		clear:right;
		float:left;
	}
	.wrap img{
		margin:-5px 5px 5px -5px;
	}
	(2) box-shadow:3px 3px 6px #888;(垂直和水平位移,投影宽度和颜色)
12.:link伪类选择器用来寻找未被访问过的链接
   :visited伪类选择器用来寻找访问过的的链接
   :actived激活发生在链接被单机时
13.属性选择器允许根据特定的属性是否存在或属性值寻找元素(突出所有的外部链接)
   例如:使用[att^=val]属性选择器寻找以文本http:开头的所有链接
14.链接应该只用于GET请求，绝不要用于POST请求。
15.工具提示是当鼠标悬停在具有title属性的元素上时刘拉你弹出的黄色小文本框。
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
9.
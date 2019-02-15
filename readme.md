# <canvas> 元素
<canvas> 是一个替换元素，需要结束标签</canvas>。它只有两个标签：width 和 height，当没有设置宽高，canvas 会默认为宽300px和高150px（使用CSS设置canvas 的宽高会导致画布内容模糊）。
<canvas> 需要通过脚本，它有一个叫getContext() 方法是用来获得 rendering context or painting. 对于2D图像而言，可以使用 CanvasRenderingContext2D。
var canvas=document.getElementById("canvasCtx"); //为元素<canvas>得到DOM对象
var ctx=canvas.getContext("2d"); //使用2d来绘制上下文
绘制形状：方形 rectangularctx.fillRect(x, y, width, height); //绘制一个实心方形
ctx.strokeRect(x, y, width, height); //绘制一个方形边框
ctx.clearRect(x, y, width, height); //清除指定方形区域，变成透明
绘制路径ctx.beginPath(); //开始生成一条路径
ctx.moveTo(x, y); //路径移到指定位置
ctx.lineWidth; //设定路径宽度
ctx.lineTo(x, y); //路径连接指定位置
ctx.lineTo(x, y); //路径连接另一指定位置
ctx.fill(); //填充各连接路径内的区域
onmousedown = "SomeJavaScriptCode" 滑鼠按下会触发的事件
onmousemove = "SomeJavaScriptCode" 滑鼠移动会触发的事件
onmouseup = "SomeJavaScriptCode" 滑鼠松开会触发的事件
document.documentElement.clientWidth 获取页面可见宽度
document.documentElement.clientHeight 获取页面可见高度
window.onresize 获取当前窗口resize事件
element.onclick 返回当前元素的click 的事件

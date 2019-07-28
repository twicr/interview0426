# interview
# 每日三问——0426
> [github项目](https://github.com/haizlin/fe-interview?utm_source=ZHShareTargetIDMore&utm_medium=social&utm_oi=750848792785354752) 问题解答
# HTML
### viewport常见设置都有哪些？
viewport时用户可视窗口，pc端为显示区域，移动端的显示区域可能超出屏幕大小，可能出现滚动条,常用设置
* width(width=device-width)
* initial-scale(初始缩放值)
* maximum-scale(最大缩放值)
* minxmum-scale(最小缩放值)
* user-scale(是否手动缩放)
# CSS
### 对比下px、em、rem有什么不同？
* px：绝对固定的值
* em：相对父元素的倍数关系
* rem：相对根元素(html)的倍数关系(一般浏览器默认字体大小为16px)
# JS
### 简要描述下什么是回调函数并写一个例子出来
将A函数以参数的形式传入B函数，当B函数满足某个条件时再调用A函数，此时A函数为回调函数
```javascript
function main(callBack){
	callBack();
	console.log("主函数");
}
function callBack(){
	setTimeout(() => {console.log('回调函数')}, 2000);
}
```
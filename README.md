# until

## 记录一些常用的方法

// 	h5底部输入框被键盘遮挡问题：
//  当输入框在最底部，点击软键盘后输入框会被遮挡。可采用如下方式解决

	var oHeight = $(document).height(); //浏览器当前的高度

	$(window).resize(function(){

		if($(document).height() < oHeight){

			$("#footer").css("position","static");

		}else{

			$("#footer").css("position","absolute");

		}

	})

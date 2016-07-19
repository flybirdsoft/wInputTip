# wInputTip
适用于Mobile端或PC端输入框提示组件

# 调用方式示例一：

	var t = new wInputTip({
		id:"input",
		tip:"请输入手机号",
		label:{
			offsetX:5,
			offsetY:0,
			type:"custom",                 /* 使用自定义方式呈现 */
			onfocus:function(input,label){ /* 自定义方式处理     */
				label.style.top="-30px";
				label.style.fontSize="10px";
			},
			onblur:function(input,label){  /* 自定义方式处理     */
				if(input.value=="")
				{
					label.style.top="0";
					label.style.fontSize="1em";
				}
			}
		}
	});
	
# 调用方式示例二（简单）：

		var t3 = new wInputTip({
		id:"input3",
		tip:"年龄",
		label:{        /*提示信息在文本框里的位置信息的位置*/
			offsetX:10,
			offsetY:0
		}
	});
	
	

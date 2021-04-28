# vue-countTo
vue-countTo的使用
```html
1.安装依赖：
npm install vue-count-to -D
2.示例：
http://panjiachen.github.io/countTo/demo/
<template>
  <countTo :startVal='startVal' :endVal='endVal' :duration='3000'></countTo>
</template>

<script>
  import countTo from 'vue-count-to';
  export default {
    components: { countTo },
    data () {
      return {
        startVal: 0,
        endVal: 2020
      }
    }
  }
</script>
```
```table
3.参数
属性	           描述               类型	      默认
startVal	      开始值	           Number	       0
endVal	        结束值	           Number	      2017
duration	 持续时间，以毫秒为单位  Number	     3000
autoplay	    自动播放	          Boolean	     true
decimals	  要显示的小数位数	     Number	       0
decimal	    十进制分割            String	       .
separator	    分隔符	            String	       ,
prefix	      前缀	             String	       ''
suffix	      后缀	             String	       ''
useEasing	  使用缓和功能	       Boolean	     true
easingFn	   缓和回调

4.功能
属性	描述
mountedCallback	挂载以后返回回调
start	开始计数
pause	暂停计数
reset	重置countTo
```

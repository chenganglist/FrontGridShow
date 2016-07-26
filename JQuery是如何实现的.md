##JQuery是如何实现的
###$是自定义函数，只是看起来特殊一些，和一般的function没区别,比如
function $(param){
  alert(param);
}

$('$ now becomes an alert function');

	function $(e, n, r) {
		if (r === t && 1 === e.nodeType) {
			var i = "data-" + n.replace(P, "-$1").toLowerCase();
			if (r = e.getAttribute(i), "string" == typeof r) {
				try {
					r = "true" === r ? !0 : "false" === r ? !1 : "null" === r ? null : +r + "" === r ? +r : B.test(r) ? x.parseJSON(r) : r
				} catch (o) {}

				x.data(e, n, r)
			} else
				r = t
		}
		return r
	}

###本质
JSON格式的定义--匿名函数     
基本的JS语法   
JS面向对象的做法（通过函数返回一个特定的JSON格式的变量。   
JSON变量的Key：Value，Value可以是具体的函数）          


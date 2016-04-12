title: 正则的方法test
date: 2016-01-03 23:43:50
tags: JavaScript
categories: JavaScript
---

test : 正则去匹配字符串，如果匹配成功就返回真，如果匹配失败就返回假

test的写法 : 正则.test(字符串)
{% codeblock %}
var str = 'abcdef';
var re = /b/;
alert( re.test(str) );	//弹出true
{% endcodeblock %}
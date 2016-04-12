title: 利用rem进行弹性布局
date: 2015-12-30 22:35:47
tags: CSS3
categories: CSS3
---

现在在做移动端项目中都是用了rem进行了弹性布局，顺便聊下rem的那些事。

所谓rem，rem是css3新增的一个单位。在W3C官网上是这样描述rem的——“font size of the root element” 。

rem的大小是根据<html>的“font-size”为基准，我们来看一个简单的代码实例：

{% codeblock %}
 html{
        font-size: 10px;
 }
 div{
        width: 1.5rem;
        height: 1.5rem;
 }
{% endcodeblock %}

 那么div的宽度就是15px，高度也是15px，也就是1.5*10=10，计算公式：(根节点的字体大小) 乘以 (本身rem的大小)，为了在做项目中计算方便，可以设置html:font-size为100px，最好不要设置10px（谷歌浏览器不支持12px以下的字体）。

 当然，在做移动端项目的时候，最好能通过屏幕的宽度，按照比例进行动态设置html:font-size的大小。可以通过js，或者media都可以的。

 对于PC端，IE6-8不支持rem，所以最好在移动端上用。
title: 初步认识AngularJS
date: 2016-01-01 16:20:15
tags: AngularJS
categories: AngularJS
---

什么是angularJs？
    angularJs基于javascript开发的客户端应用框架，使我们可以更加快捷，简单的开发web应用。诞生于2009年，后来被google收购，用在了很多项目中。适用于CRUD应用或者SPA单页面网站的开发。
    angularJs是为了克服HTML在构建应用上的不足而设计的。HTML是一门很好的为静态文本展示设计的声明式语言，但要构建WEB应用的话它就显得乏力了。所以我做了一些工作（你也可以觉得是小花招）来让浏览器做我想要的事。


五大特性：
	1、良好的应用程序结构
	2、双向数据绑定
	3、指令
	4、HTML 模板
	5、可嵌入、注入和测试


优点：
	1、模板功能强大丰富，并且是声明式的，自带了丰富的 Angular 指令
	2、是一个比较完善的前端MV*框架，包含模板，数据双向绑定，路由，模块化，服务，依赖注入等所有功能
	3、自定义 Directive，比 jQuery 插件还灵活，但是需要深入了解 Directive 的一些特性，简单的封装容易，复杂一点官方没有提供详细的介绍文档，我们可以通过阅读源代码来找到某些我们需要的东西，如：在 directive 使用 $parse
	4、ng模块化比较大胆的引入了Java的一些东西（依赖注入），能够很容易的写出可复用的代码，对于敏捷开发的团队来说非常有帮助，我们的项目从上线到目前，UI变化很大，在摸索中迭代产品，但是js的代码基本上很少改动


缺点：
	1、验证功能错误信息显示比较薄弱，需要写很多模板标签，没有JQuery Validate方便，所以我们自己封装了验证的错误信息提示
	2、ngView只能有一个，不能嵌套多个视图
	3、对于特别复杂的应用场景，貌似性能有点问题，特别是在Windows下使用chrome浏览器，不知道是内存泄漏了还是什么其他问题，没有找到好的解决方案，奇怪的是在IE10下反而很快，对此还在观察中
	4、这次从1.0.X升级到1.2.X，貌似有比较大的调整，没有完美兼容低版本，升级之后可能会导致一个兼容性的BUG，具体详细信息参考官方文档 AngularJS
	5、ng提倡在控制器里面不要有操作DOM的代码，对于一些JQuery 插件的使用，如果想不破坏代码的整洁性，需要写一些directive去封装一下JQ插件，但是现在有很多插件的版本已经支持Angular了
	6、Angular 太笨重了，没有让用户选择一个轻量级的版本，当然1.2.X后，Angular也在做一些更改，比如把route，animate等模块独立出去，让用户自己去选择
	7、兼容性不是很好
	8、SEO不是很理想


angularJs资源
	1、http://www.angularjs.org/
	2、https://www.github.com/angular/
	3、http://www.angularjs.cn/
	4、http://www.ngnice.com/
	5、http://woxx.sinaapp.com/

# 一个漂亮的所见即所得(WYSIWYG)富文本编辑器:Froala

本文翻译来自[wysiwyg-editor](https://github.com/froala/wysiwyg-editor)，大家想看原文可以点击此链接或文章下面的【阅读原文】

## 介绍

[WYSIWYG HTML编辑器](https://www.froala.com/wysiwyg-editor)是一款有史以来最强大的JavaScript富文本编辑器之一。它采用了最新的技术，并利用jQuery和HTML5的巨大优势，创造了出色的编辑体验。拥有非常多的示例让你轻松集成，让你的用户爱上它清晰的设计。它能和Ruby On Rails，Django，Angular.js，Meteor，Symgony.CakePHP等集成，具有如下特点。

- 微小 - 只需添加您需要的插件([30+ 官方插件](https://www.froala.com/wysiwyg-editor/docs/plugins))
- [客户端框架集成](https://www.froala.com/wysiwyg-editor/docs/framework-plugins/)
- 可以向如 [PHP](https://www.froala.com/wysiwyg-editor/docs/sdks/php), [Node.JS](https://www.froala.com/wysiwyg-editor/docs/sdks/nodejs),  [.NET](https://www.froala.com/wysiwyg-editor/docs/sdks/dotnet), [Java](https://www.froala.com/wysiwyg-editor/docs/sdks/java), 和 [Python](https://www.froala.com/wysiwyg-editor/docs/sdks/python)提供服务端开发工具包
- 代码注释精美
- [在线文档更新](https://www.froala.com/wysiwyg-editor/docs)
- 简单可扩展- 良好的插件注释使你更容易使用和开发自己的插件
- 良好的维护 - [持续更新](https://www.froala.com/wysiwyg-editor/changelog)
- 很好的支持 - [帮助中心](https://wysiwyg-editor.froala.help)

![WYSIWYG HTML Editor](https://raw.githubusercontent.com/froala/wysiwyg-editor/master/editor.jpg)​​

## 演示

- **基本演示**: https://www.froala.com/wysiwyg-editor
- **在线演示**: https://www.froala.com/wysiwyg-editor/inline
- **完整列表**: https://www.froala.com/wysiwyg-editor/examples
​
## 开始使用

### 初始化编辑器

Froala WYSIWYG HTML编辑器是一个易于集成和易于使用的插件。它需要[jQuery](http://jquery.com/) 1.11.0或更高版本，以及名为[Font Awesome](http://fortawesome.github.io/Font-Awesome/) 4.4.0的图标字体。你也可以使用旧版本的Font Awesome，但是某些编辑器的图标将不会出现。

下面是如何在textarea上初始化编辑器的基本示例。

```
<!DOCTYPE html>
<html>
  <head>
    <meta charset="utf-8">
 
    <!-- Include external CSS. -->
    <link href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/4.4.0/css/font-awesome.min.css" rel="stylesheet" type="text/css" />
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/codemirror/5.25.0/codemirror.min.css">
 
    <!-- Include Editor style. -->
    <link href="https://cdnjs.cloudflare.com/ajax/libs/froala-editor/2.6.0/css/froala_editor.pkgd.min.css" rel="stylesheet" type="text/css" />
    <link href="https://cdnjs.cloudflare.com/ajax/libs/froala-editor/2.6.0/css/froala_style.min.css" rel="stylesheet" type="text/css" />
  </head>
 
  <body>
    <!-- Create a tag that we will use as the editable area. -->
    <!-- You can use a div tag as well. -->
    <textarea></textarea>
 
    <!-- Include external JS libs. -->
    <script type="text/javascript" src="https://cdnjs.cloudflare.com/ajax/libs/jquery/1.11.0/jquery.min.js"></script>
    <script type="text/javascript" src="https://cdnjs.cloudflare.com/ajax/libs/codemirror/5.25.0/codemirror.min.js"></script>
    <script type="text/javascript" src="https://cdnjs.cloudflare.com/ajax/libs/codemirror/5.25.0/mode/xml/xml.min.js"></script>
 
    <!-- Include Editor JS files. -->
    <script type="text/javascript" src="https://cdnjs.cloudflare.com/ajax/libs/froala-editor/2.6.0/js/froala_editor.pkgd.min.js"></script>
 
    <!-- Initialize the editor. -->
    <script>
 		$(function() { 
			$('textarea').froalaEditor() 
		}); 
	</script>

  </body>
</html>
```

### 显示编辑内容

要在富文本编辑器之外保留编辑过的HTML的样式，你必须引入以下CSS文件。

```
<!-- CSS rules for styling the element inside the editor such as p, h1, h2, etc. -->
<link href="../css/froala_style.min.css" rel="stylesheet" type="text/css" />
```

此外，你应该确保将编辑的内容放在类名为fr-view元素中。

```
<div class="fr-view">
  Here comes the HTML edited with the Froala rich text editor.
</div>
```
### 举个栗子

在此富文本编辑器中，你可以在块级元素之间随意拖动图片，具体代码如下。

HTML

```
<div id="froala-editor">
  <h3>Click here to edit the content</h3>
  <p><img id="edit" class="fr-fil fr-dib" src="/assets/editor/docs/photo14.jpg" alt="Old Clock" width="300"/></p>
  <p>The image can be dragged only between blocks and not inside them.</p>
</div>
```

JAVASCRIPT

```
<script>
  $(function() {
    $('div#froala-editor').froalaEditor({
      dragInline: false,
      toolbarButtons: ['bold', 'italic', 'underline', 'insertImage', 'insertLink', 'undo', 'redo'],
      pluginsEnabled: ['image', 'link', 'draggable']
    })
  });
</script>
```

效果图如下所示。

![WYSIWYG HTML Editor](https://cloud.githubusercontent.com/assets/20238205/26573912/09b7c2ce-4552-11e7-9687-2e0f5b8080ba.gif)

有关自定义编辑器的详细信息，请查看编辑器[文档](https://www.froala.com/wysiwyg-editor/docs)。
​​​   
## 相关下载

- npm: `npm install froala-editor`
- bower: `bower install froala-wysiwyg-editor`
- CDN: https://cdnjs.com/libraries/froala-editor
- Angular JS: https://github.com/froala/angular-froala
- Angular 2: https://github.com/froala/angular2-froala-wysiwyg
- Aurelia: https://github.com/froala/aurelia-froala-editor
- CakePHP: https://github.com/froala/wysiwyg-cake
- Django: https://github.com/froala/django-froala-editor
- Ember: https://github.com/froala/ember-froala-editor
- Knockout: https://github.com/froala/knockout-froala
- Meteor: https://github.com/froala/meteor-froala
- Ruby on Rails: https://github.com/froala/wysiwyg-rails
- React JS: https://github.com/froala/react-froala-wysiwyg/
- Reactive: https://github.com/froala/froala-reactive
- Symfony: https://github.com/froala/KMSFroalaEditorBundle
- Vue JS: https://github.com/froala/vue-froala-wysiwyg/
- Yii2: https://github.com/froala/yii2-froala-editor
- Wordpress: https://github.com/froala/wordpress-froala-wysiwyg
​
## 浏览器支持

我们正在积极测试编辑器在所有主要浏览器兼容性。在下面列出的浏览器中，如有任何问题请当作bug反馈到我们的GitHub库。

- Internet Explorer 10+
- Safari 6+
- Firefox (Current - 1) and Current versions
- Chrome (Current - 1) and Current versions
- Opera (Current - 1) and Current versions
- iOS 7.0+
- Android 4.0+

## 资源

- 演示： [www.froala.com/wysiwyg-editor](http://www.froala.com/wysiwyg-editor)
- 下载页面：[www.froala.com/wysiwyg-editor/download](https://www.froala.com/wysiwyg-editor/download)
- 文档： [froala.com/wysiwyg-editor/docs](https://www.froala.com/wysiwyg-editor/docs)
- 授权协议： [www.froala.com/wysiwyg-editor/terms](https://www.froala.com/wysiwyg-editor/terms)
- 帮助： [wysiwyg-editor.froala.help](https://wysiwyg-editor.froala.help/hc/en-us)
- 问题：[Repo guidelines](https://github.com/highcharts/highcharts/blob/master/repo-guidelines.md)
​
## 问题报告

我们使用GitHub中的问题作为Froala WYSIWYG HTML编辑器的官方错误跟踪器，以下是我们希望报告问题的用户的一些建议：

1. 确保您使用的是最新版本的Froala WYSIWYG Editor。 您即将报告的问题可能已在最新的主分支版本中已经修复：https：//github.com/froala/froala-wysiwyg/tree/master/js。

2. 为问题提供可复写的步骤将会缩短解决时间。[JSFiddle](https://jsfiddle.net)总是受欢迎的。 
3. 某些问题可能是浏览器特定的，因此在您遇到问题中指定浏览器可能会有所帮助。

## 技术支持或问题

如果您有任何问题或需要帮助，请与我们[联系](https://www.froala.com/wysiwyg-editor/contact)。

## 许可

为了使用Froala编辑器，您必须根据需求购买以下许可证之一。 您可以在我们的网站上的[定价计划页面](https://www.froala.com/wysiwyg-editor/pricing)找到更多信息。


## 文章回顾

[ECMAScript modules in browsers](http://mp.weixin.qq.com/s/PVL8kuXBwirbgm6MCpnl5A)

[SQL已经43岁了：盘点8大我们还在使用的理由](https://mp.weixin.qq.com/s/BsL8aWUqr3z2zSYbRtP75Q)

[大公司里怎样开发和部署前端代码？](https://mp.weixin.qq.com/s/Mq6Gd8QXuNbN0pPIFuIxPA)

如对其他文章感兴趣，可以关注大前端工程师</br>

![weixinhao](https://cloud.githubusercontent.com/assets/20238205/26142454/2d2b04bc-3b13-11e7-85d4-cf6d5277722c.png)

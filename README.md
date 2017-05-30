基于HTML5技术的漂亮的富文本编译器WYSIWYG
https:/www.froala.com/wysiwyg-editor

![WYSIWYG HTML Editor](https://cdn0.froala.com/assets/editor/pages/B/tour/tour-3cf16a0c5b3471ef2b56ad7d1aa2d747.svg)
​

# [Froala Editor](https://www.froala.com/wysiwyg-editor) 

Froala WYSIWYG HTML 编辑器是一款有史以来最强大的JavaScript富文本编辑器。

- 微小 - 只需添加您需要的插件([30+ 官方插件](https://www.froala.com/wysiwyg-editor/docs/plugins))
- [客户端框架集成](https://www.froala.com/wysiwyg-editor/docs/framework-plugins/)
- 可以向如 [PHP](https://www.froala.com/wysiwyg-editor/docs/sdks/php), [Node.JS](https://www.froala.com/wysiwyg-editor/docs/sdks/nodejs),  [.NET](https://www.froala.com/wysiwyg-editor/docs/sdks/dotnet), [Java](https://www.froala.com/wysiwyg-editor/docs/sdks/java), 和 [Python](https://www.froala.com/wysiwyg-editor/docs/sdks/python)提供服务端开发工具包
- 代码注释精美
- [在线文档更新](https://www.froala.com/wysiwyg-editor/docs)
- 简单可扩展- 良好的插件注释使你更容易使用和开发自己的插件
- 良好的维护 - [持续更新](https://www.froala.com/wysiwyg-editor/changelog)
- 很好的支持 - [帮助中心](https://wysiwyg-editor.froala.help)
​

## 演示

- **基本演示**: https://www.froala.com/wysiwyg-editor
- **在线演示**: https://www.froala.com/wysiwyg-editor/inline
- **完整列表**: https://www.froala.com/wysiwyg-editor/examples
​
## 开始使用

Froala WYSIWYG HTML编辑器需要[jQuery](http://jquery.com/) 1.11.0或更高版本，以及名为[Font Awesome](http://fortawesome.github.io/Font-Awesome/) 4.4.0的图标字体。您也可以使用旧版本的Font Awesome，但是某些编辑器的图标不会出现。 

```html
<!-- Include CSS for icons. -->
<link href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/4.4.0/css/font-awesome.min.css" rel="stylesheet" type="text/css" />

<!-- Include Editor style. -->
<link href="https://cdnjs.cloudflare.com/ajax/libs/froala-editor/2.5.1/css/froala_editor.pkgd.min.css" rel="stylesheet" type="text/css" />
<link href="https://cdnjs.cloudflare.com/ajax/libs/froala-editor/2.5.1/css/froala_style.min.css" rel="stylesheet" type="text/css" />

<!-- Create a tag that we will use as the editable area. -->
<!-- You can use a div tag as well. -->
<textarea></textarea>

<!-- Include jQuery lib. -->
<script type="text/javascript" src="https://cdnjs.cloudflare.com/ajax/libs/jquery/1.11.0/jquery.min.js"></script>

<!-- Include Editor JS files. -->
<script type="text/javascript" src="https://cdnjs.cloudflare.com/ajax/libs/froala-editor/2.5.1//js/froala_editor.pkgd.min.js"></script>

<!-- Initialize the editor. -->
<script> 
  $(function() { 
    $('textarea').froalaEditor() 
  }); 
</script>
```
有关自定义编辑器的详细信息，请查看编辑器[文档](https://www.froala.com/wysiwyg-editor/docs)。​
    
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
- ​
## 浏览器支持

At present, we officially aim to support the last two versions of the following browsers:

- Chrome
- Edge
- Firefox
- Safari
- Opera
- Internet Explorer 10+
- Safari iOS
- Chrome, Firefox and Default Browser Android
- 
## 资源

- 演示： [www.froala.com/wysiwyg-editor](http://www.froala.com/wysiwyg-editor)
- 下载页面：[www.froala.com/wysiwyg-editor/download](https://www.froala.com/wysiwyg-editor/download)
- 文档： [froala.com/wysiwyg-editor/docs](https://www.froala.com/wysiwyg-editor/docs)
- 授权协议： [www.froala.com/wysiwyg-editor/terms](https://www.froala.com/wysiwyg-editor/terms)
- 帮助： [wysiwyg-editor.froala.help](https://wysiwyg-editor.froala.help/hc/en-us)
- 问题：[Repo guidelines](https://github.com/highcharts/highcharts/blob/master/repo-guidelines.md)
​
## 问题报告

我们使用GitHub中的问题作为Froala WYSIWYG HTML编辑器的官方错误跟踪器。 以下是我们希望报告问题的用户的一些建议：

1. 确保您使用的是最新版本的Froala WYSIWYG Editor。 您即将报告的问题可能已在最新的主分支版本中修复：https：//github.com/froala/froala-wysiwyg/tree/master/js。

2. 为问题提供可复写的步骤将会缩短解决时间。[JSFiddle](https://jsfiddle.net)总是受欢迎的。 
3. 某些问题可能是浏览器特定的，因此在您遇到问题中指定浏览器可能会有所帮助。

## 技术支持或问题

如果您有任何问题或需要帮助，请与我们[联系](https://www.froala.com/wysiwyg-editor/contact) ，而不是空着问题。

## 许可
为了使用Froala编辑器，您必须根据需要购买以下许可证之一。 您可以在我们的网站上的[定价计划页面](https://www.froala.com/wysiwyg-editor/pricing)上找到更多信息

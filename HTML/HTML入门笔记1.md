
# HTML
##  调试代码用  
 1) [js.jirengu.com](https://js.jirengu.com/)  
 2) 代码沙盒 [codesandbox](https://note.youdao.com/).io
 
 ## HTML简介
HTML 的全名是“超文本标记语言”（HyperText Markup Language），由蒂姆·伯纳斯-李（Tim Berners-Lee）发明
 
## HTML起手

```
<!DOCTYPE html> //<!DOCTYPE html>文档类型 
<html lang="en">
  <head>
  <!--<meta charset='UTF-8'> 文件的字符编码,可以改成zh-CN中文-->
    <meta charset="UTF-8" /> 
    <!--禁用缩放 兼容手机-->
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <!--告诉ie使用最新内核-->
    <meta http-equiv='X-UA-Compatible' content="ie=edge">
    <!--标题-->
    <title>Document</title>
  </head>
  <body>
    <img id="xxx" src="./photo.png" />
  </body>
</html>

 head里面一般是看不见的元素
```
VS Code内可以使用快捷键 ！+ Tab自动生成部分格式，自己检查并修改



##  章节标签
1. 标题h1~h6
2. 章节section
3. 文章article
4. 段落 p
5. 头部 header
6. 尾部 footer
7. 主要内容 main
8. 旁支aside
9. 划分 div

##  全局属性（所有标签都有的属性）
1. class .class(只要含有class都能找到)
2. contenteditable 用户可以直接在页面编辑
3. hidden
4. id 尽量不要用id
5. style: 

```javascript
1) <div style="color:green"></div> //style 的优先级高于css
2) 在js中操作style(优先级最高): XXX.style.border='10px solid green'
```

6. tabindex:控制tab的顺序


<a href="http://www.w3school.com.cn/" tabindex="2">W3School</a>
<a href="http://www.google.com/" tabindex="1">Google</a>
<a href="http://www.microsoft.com/" tabindex="3">Microsoft</a>

tabindex=0 是最后一个
tabindex=-1 永远不到这里来

7. title 
规定关于元素的额外信息。
这些信息通常会在鼠标移到元素上时显示一段工具提示文本（tooltip text）


```
实现限定范围，超出用省略号代替
white-space:nowrap //不要换行
overflow：hidden//溢出就shenglue
text-overflow: ellipsis //省略部分用省略号

<style></style>标签 display:block 可以让style标签被看到
```


##  默认样式 

1. element.style: 自己写的样式
2. user agent:浏览器自带的默认样式
3. css reset：默认样式不符合需求，把默认样式干掉
 
##  内容标签

1. ol+li：ordered list + list item
2. ul+ li: description List + 
3. dl+dt+dd:列表+词+描述内容
4. pre ： 保留空格，回车，tab。<pre></pre>
5. code: <code>把代码包起来</code>  
6. hr: hr分割线 
7. a: <a href="" target=''>链接</a>  target:打开新页面
8. em：强调。默认样式是斜体 语气上的强调
9. strong：加粗 内容本身的强调

strong：粗体强调标签，强调，表示内容的重要性；  

em：斜体强调标签，更强烈的强调，表示内容的强调点，即一个是粗体，一个是斜体，都表示强调。  

10. quote：引用，看不出样式上有什么区别。

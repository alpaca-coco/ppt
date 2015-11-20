title: nodeppt markdown 演示
speaker: Theo Wang
url: https://github.com/ksky521/nodePPT
transition: move
files: /js/demo.js,/css/demo.css,/js/zoom.js
theme: dark
usemathjax: yes

[slide]

# 今日分享
## 使用fis构建你的前端开发环境  gitflow工作流实践
<small>分享者：朱其聪</small>

[slide]

![](/images/zb.jpg)

##请注意！在下要开始装逼了！！！！

[slide]
## 什么是fis？

fis是解决前端开发中以下的问题工具
----
* 自动化工具 {:&.rollIn}
* 性能优化
* 模块化框架
* 开发规范
* 代码部署
* 开发流程



[slide]
## gitflow工作流
----
![](/images/gitflow.png)




[slide]

## 主分支

* master
* developer

## 辅助分支

* feature
* release
* hotfix

[slide]
## master分支
>  master分支上存放的应该是随时可供在生产环境中部署的代码（Production Ready state）。当开发活动告一段落，产生了一份新的可供部署的代码时，master分支上的代码会被更新。同时，每一次更新，最好添加对应的版本号标签（TAG）。

[slide]
## developer分支
>develop分支是保存当前最新开发成果的分支。通常这个分支上的代码也是可进行每日夜间发布的代码（Nightly build）。因此这个分支有时也可以被称作“integration branch”。

>当develop分支上的代码已实现了软件需求说明书中所有的功能，通过了所有的测试后，并且代码已经足够稳定时，就可以将所有的开发成果合并回master分支了。对于master分支上的新提交的代码建议都打上一个新的版本号标签（TAG），供后续代码跟踪使用。

>因此，每次将develop分支上的代码合并回master分支时，我们都可以认为一个新的可供在生产环境中部署的版本就产生了。通常而言，“仅在发布新的可供部署的代码时才更新master分支上的代码”是推荐所有人都遵守的行为准则。基于此，理论上说，每当有代码提交到master分支时，我们可以使用Git Hook触发软件自动测试以及生产环境代码的自动更新工作。这些自动化操作将有利于减少新代码发布之后的一些事务性工作。

[slide]
## 支持.class/#id/自定义属性样式
----

```html
使用：.class{:.class}
使用：#id{:#id}
组合使用：{:.class.class2 width="200px"}
父元素样式使用&：{:&.class}
```

[slide]

## 主页面样式
### ----是上下分界线
----

nodeppt是基于nodejs写的支持 **Markdown!** 语法的网页PPT

nodeppt：https://github.com/ksky521/nodePPT

[slide]

[subslide]
## 这是一个列表
---
* 上下左右方向键翻页
    * 列表支持渐显动画 {:&.moveIn}
    * 支持多级列表
    * 这个动画是moveIn
* 完全基于markdown语法哦
============
## 这是一个subslide页面
---
1. 数字列表 {:&.rollIn}
2. 数字列表
3. 数字列表，这是一个subslide页面
[/subslide]

[slide]
## 列表渐显动画：fadeIn
----
* 列表支持渐显动画哦 {:&.fadeIn}
    * 使用方法
    * markdown列表第一条加上：{:&.动画类型}
* 动画类型
    * fadeIn
    * rollIn
    * bounceIn
    * moveIn
    * zoomIn

[slide]
## 列表渐显动画：zoomIn
----
* 列表支持渐显动画哦 {:&.zoomIn}
* 动画类型
    * fadeIn
    * rollIn
    * bounceIn
    * moveIn
    * zoomIn

[slide]
## 列表渐显动画：bounceIn
----
* 列表支持渐显动画哦 {:&.bounceIn}
* 动画类型
    * fadeIn
    * rollIn
    * bounceIn
    * moveIn
    * zoomIn



[slide]
## 表格示例
### 市面上主要的css预处理器：Less\Sass\Stylus
---
| Less | Sass | Stylus
:-------|:------:|-------:|--------
环境 |js/nodejs | Ruby(这列右对齐) | nodejs(高亮) {:.highlight}
扩展名 | .less | .scss/.sass | .styl
特点 | 老牌，用户多，支持js解析 | 功能全，有成型框架，发展快 | 语法多样，小众
案例/框架 | [Bootstrap](http://getbootstrap.com/) | [Compass](http://beta.compass-style.org) [Bootstrap](http://getbootstrap.com/css/#sass) [Foundation](http://foundation.zurb.com/) [Bourbon](http://bourbon.io) [Base.Sass](https://github.com/jsw0528/base.sass) |


[slide]
## text
-----

<span class="text-danger">.text-danger</span> <span class="text-success">.text-sucess</span><span class="text-primary">.text-primary</span>

<span class="text-warning">.text-warning</span><span class="text-info">.text-info</span><span class="text-white">.text-white</span><span class="text-dark">.text-dark</span>


<span class="blue">.blue</span><span class="blue2">.blue2</span><span class="blue3">.blue3</span><span class="gray">.gray</span><span class="gray2">.gray2</span><span class="gray3">.gray3</span>

<span class="red">.red</span><span class="red2">.red2</span><span class="red3">.red3</span>

<span class="yellow">.yellow</span><span class="yellow2">.yellow2</span><span class="yellow3">.yellow3</span><span class="green">.green</span><span class="green2">.green2</span><span class="green3">.green3</span>

[slide]
## label and link
<span class="label label-primary">.label.label-primary</span><span class="label label-warning">.label.label-warning</span><span class="label label-danger">.label.label-danger</span><span class="label label-default">.label.label-default</span><span class="label label-success">.label.label-success</span><span class="label label-info">.label.label-info</span>

<a href="#">link style</a> <mark>mark</mark>

[slide]
## blockquote
----

> nodeppt可能是迄今为止最好用的web presentation <small>三水清</small>


下面是另外一种样式

> 这是一个class是：pull-right的blockquote <small>small一下</small> {:&.pull-right}

[slide]
## buttons
----

<button class="btn btn-default">.btn .btn-default</button>  <button class="btn btn-primary">.btn.btn-lg.btn-primary</button> <button class="btn btn-warning">.btn.btn-waring</button> <button class="btn btn-success">.btn.btn-success</button> <button class="btn btn-danger">.btn.btn-danger</button>



<button class="btn btn-lg btn-default">.btn.btn-lg.btn-default</button> <button class="btn btn-xs btn-success">.btn.btn-xs.btn-success</button> <button class="btn btn-sm btn-primary">.btn.btn-sm.btn-primary</button> <button class="btn btn-rounded btn-warning">.btn.btn-rounded.btn-waring</button>  <button class="btn btn-danger" disabled="disabled">disabled.btn.btn-danger</button>


<button class="btn btn-success"><i class="fa fa-share mr5"></i></button>

[slide]
## icons: Font Awesome
------

<i class="fa fa-apple"></i>
<i class="fa fa-android"></i>
<i class="fa fa-github"></i>
<i class="fa fa-google"></i>
<i class="fa fa-linux"></i>
<i class="fa fa-css3"></i>
<i class="fa fa-html5"></i>
<i class="fa fa-usd"></i>
<i class="fa fa-pie-chart"></i>
<i class="fa fa-file-video-o"></i>
<i class="fa fa-cog"></i>


[slide]

## 代码格式化
### 使用 `highlightjs` 进行语法高亮
----
<div class="columns-2">
    <pre><code class="javascript">(function(window, document){
    var a = 1;
    var test = function(){
        var b = 1;
        alert(b);
    };
    //泛数组转换为数组
    function toArray(arrayLike) {
        return [].slice.call(arrayLike);
    }
}(window, document));
    </code></pre>
    <pre><code class="javascript">(function(window, document){
    var a = 1;
    var test = function(){
        var b = 1;
        alert(b);
    };
    //泛数组转换为数组
    function toArray(arrayLike) {
        return [].slice.call(arrayLike);
    }
}(window, document));
    </code></pre>
</div>



[slide]
## 支持多种皮肤
----

[colors](/)-[moon](?theme=moon)-[blue](?theme=blue)-[dark](?theme=dark)-[green](?theme=green)-[light](?theme=light)


[slide data-incallback="testScriptTag"]
## 支持 HTML 和 markdown 语法混编
----

<div class="file-setting">
    <p>这是html</p>
</div>
<p id="css-demo">这是css样式</p>
<p>将html代码直接混编到**markdown**文件中即可</p>

我是js控制的颜色 black {:#testScriptTag}

<script>
    function testScriptTag(){
        document.getElementById('testScriptTag').style.color = 'black';
    }

</script>
<style>
#css-demo{
    color: red;
}
</style>


[slide]
## iframe效果
----
<iframe data-src="http://www.baidu.com" src="about:blank;"></iframe>

[slide]
## 动画样式强调
----

这段话里面的**加粗**和*em*字体会动画哦~

按下【H】键查看效果


[slide]
## 支持zoom.js
----

增加了zoom.js的支持，在演示过程中使用`alt`+鼠标点击，则点击的地方就开始放大，再次`alt+click`则回复原状

[slide]

## 图片，点击全屏
----

![小萝莉](/girl.jpg "小萝莉")


[slide]
[note]
##这里是note

使用n键，才能显示
[/note]
## 使用note笔记
### note笔记是多窗口，或者自己做一些笔记用的
---
按下键盘【N】键测试下note，

markdown语法如下：
```markdown
[note]
这里是note，{ 要换成中括号啊！！
{/note]
```
[slide]

## 使用画笔
### 使用画笔做标记哦~你也可以随便作画啊！
---
按下键盘【P】键：按下鼠标左键，在此处乱花下看看效果。

按下键盘【B/Y/R/G/M】：更换颜色，按下【1~4】：更换粗细

按下键盘【C】键：清空画板


[slide]

## 宽度不够？？
---
按下键盘【W】键，切换到更宽的页面看效果，第二次按键返回

 |less| sass | stylus
:-------|:------:|-------:|--------
环境 |js/nodejs | Ruby(这列右对齐) | nodejs(高亮) {:.highlight}
扩展名 | .less | .sass/.scss | .styl
特点 | 老牌，用户多，支持js解析 | 功能全，有成型框架，发展快 | 语法多样，小众
案例/框架 | [Bootstrap](http://getbootstrap.com/) | [compass](http://compass-style.org) [bourbon](http://bourbon.io) |

[slide]
## 使用overview模式
---
按下键盘【O】键。看下效果。

在overview模式下，方向键下一页，【enter】键进入选中页

或者按下键盘【O】键，退出overview模式

[slide]

## 多窗口演示
## 双屏演示不out！
---
本页面网址改成 [url?_multiscreen=1](?_multiscreen=1)，支持多屏演示哦！

跟powderpoint一样的双屏功能，带有备注信息。

[slide]
## 20种转场动画随心换
----
 * <a href="?transition=slide">slide</a>/<a href="?transition=slide2">slide2</a>/<a href="?transition=slide3">slide3</a>
 * [newspaper](?transition=newspaper)
 * [glue](?transition=glue)
 * [kontext](?transition=kontext)/[vkontext](?transition=vkontext)
 * [move](?transition=move)/[circle](?transition=circle)
 * [horizontal](?transition=horizontal)/[horizontal3d](?transition=horizontal3d)
 * [vertical3d](?transition=vertical3d)
 * [zoomin](?transition=zoomin)/[zoomout](?transition=zoomout)
 * [cards](?transition=cards)
 * [earthquake](?transition=earthquake)/[pulse](?transition=pulse)/[stick](?transition=stick)...


[slide data-transition="glue"]

## 这是一个glue的动画
----
使用方法（全局设置） 1：

> transition: glue


[slide data-transition="glue"]

## 这是一个glue的动画
----
使用方法 2：

&#91;slide data-transition="glue"&#93;

[slide data-transition="zoomin"]

## 这是一个zoomin的动画
----
使用方法：

&#91;slide data-transition="zoomin"&#93;

[slide data-transition="vertical3d"]

## 这是一个vertical3d的动画
----
使用方法：

&#91;slide data-transition="vertical3d"&#93;

[slide data-outcallback="outcallback" data-incallback="incallback" ]
## 使用回调
----

* &#91;slide data-outcallback="fnName"&#93;
    * 进入执行回调incallback函数
* &#91;slide data-incallback="fnName"&#93;
    * 退出执行outcallback函数

亦可以组合写：

> &#91;slide data-outcallback="foo" data-incallback="bar"&#93;


<p id="incallback"></p>
<p id="outcallback"></p>

[slide]
## 远程执行函数
----
在多屏和远程模式中，可以使用`proxyFn`来远程执行函数。

```html
<script>
function globalFunc(){
}
</script>
<button onclick="Slide.proxyFn('globalFunc')" class="btn btn-default">远程执行函数</button>
```

<button onclick="Slide.proxyFn('globalFunc','args')" class="btn btn-default">测试远程执行函数</button>
<a href="?_multiscreen=1#33">在多屏中测试远程执行</a>
<script>
    function globalFunc(a){
        alert('proxyFn success: '+a);
    }
</script>


[slide]

## 更多玩法
---
https://github.com/ksky521/nodePPT

什么？这些功能还不够用？

socket远程控制可以在手机上摇一摇换页哦~

查看项目目录ppts获取更多帮助信息

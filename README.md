## Readme

博客是基于Jekyll模版的。可通过fork此工程开始写世强博客

* [中文官方文档](http://jekyll.com.cn/)

### 1 Folder structure

#### 1.1 Template

> Only related to template, won't effect all wrote posts.

##### 1.1.1 Page construct

* `_includes`
* `_layouts`

##### 1.1.2 Static

> no need to explain

* `js`
* `css`

##### 1.1.3 Tag&Category page

* `categories`

	> Category index page

* `tags`

	> Tag index page

#### 1.2 Site related

> different from site to site

* `public`
* `_posts`
* `_tages_page`

	> Collection page for each tag	

### 2 第一次配置

文件:

\* \_config.yml

> 修改所有TODO的地方

\* .gitlab-ci.yml

> 将TODO换为自己的用户名

### 3 写作

在`_post`文件夹下写**markdown**文件。几个要点：

1 文件名：`yyyy-MM-dd-name_no_space`

> 名字四部分：年，月，日，名字。名字中不能有`-`号和空格，否则不能被识别

2 每篇头信息很重要

> [中文官方文档-头信息](http://jekyll.com.cn/docs/frontmatter/)。例子`_posts/hello/2016-10-24-hello_world.md`

3 （可自定义修改）写作以h3为顶级标题

> 因为目录插件的**配置**支持h3,h4,h5。可**自定义**修改配置，在js/tocUse.js中。[官方链接](https://github.com/ghiculescu/jekyll-table-of-contents)

### 本地调试

需要先安装ruby和gem，然后通过gem安装jekyll和jekyll-paginate。

通过`ruby -v`和`jekyll -v`验证安装

在文件根目录`jekyll serve`运行，通过`127.0.0.1:4000/{{根目录,默认TODO}}`访问

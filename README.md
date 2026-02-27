# xf_blog
[github 线路](https://lm-xiao-fen.github.io)　[cloudflare 线路](/404)　[edgeone 线路](/404)
## 一点点介绍
这是我拿 github 官方主题 primer 改的，这个主题本身是给项目仓做库介绍网页做的，但我改成了博客

所以我称它为……

<h1 align="center">primer for blog</h1>

###### 好中二啊

## 怎么使用
在 **_posts** 和 **_note** 下新建格式为 **YYYY-MM-DD-title.md** 的文件

在 **_posts** 和 **_note** 下的文件内容开头必须有下面这段内容

```yaml
---
layout: post
title: "title"
date: YYYY-MM-DD
---
```

## 怎么部署
这是我的自用博客，并没有开放一个模板
如果你要使用你可以按照以下方法

### 直接fork
点击仓库顶部的 **fork** 或者直接[点击此处](https://github.com/lm-xiao-fen/lm-xiao-fen.github.io/fork)

将 **_posts** 和 **_note** 里的所有文件删除

### git 下来
在你的 github 创建好一个一个仓库

将这个仓库克隆到本地

```shell
git clone https://github.com/lm-xiao-fen/lm-xiao-fen.github.io.git  # 克隆该项目
cd lm-xiao-fen.github.io  # 进入项目文件
```

将 **_posts** 和 **_note** 里的所有文件删除

```shell
rm -i ./_posts/*  # 删除 /_posts 下的所有文件
rm -i ./_note/*  # 删除 /_note 下的所有文件
```

打开你创建的仓库网页，点击添加文件，上传项目文件中的所有文件和文件夹

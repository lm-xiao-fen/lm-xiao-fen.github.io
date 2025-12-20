---
title: "Cloudflare Workers + KV 数据库 = 一个虚拟备案系统"      
date: 2025-12-20
layout: post
---

# cloudflare workers + kv 数据库 = 一个虚拟备案系统

我闲的78疼时，我就想做个玩具玩玩 VICP虚拟备案系统应运而生

## 先看看长啥样
![预览](https://lm-xiao-fen.github.io/image/%E8%99%9A%E6%8B%9F%E5%A4%87%E6%A1%88%20(20.12.2025%2020_41).png)
源码到时候放github上了，这只是教程 [lm-xiao-fen/VICP](https://github.com/lm-xiao-fen/VICP)

## 需要什么
- **一个域名**(付费免费都可以)，并且托管至你自己的cloudflare账号上
- **cloudflare账号**

## 怎么部署

### 复制源码
- 打开 [lm-xiao-fen/VICP](https://github.com/lm-xiao-fen/VICP) 复制worker.js的源码

### 部署到cloudflare
- 打开cloudflare
- 侧边栏点击>**计算和AI**>**workers和pages**
- 右上角点击**新建应用程序**>选择**从hello world！开始**
- 给项目取个名字>点击**部署**
- 部署好后点击>右上角三个点>**编辑代码**
- 把hello world！的代码删掉，换成VICP的代码
- 最好点击**部署**

### 绑定kv数据
- 侧边栏点击>**数据与存储库**~~如果我没记错叫什么的话~~>**kv数据库**
- 右上角点击>**新建数据库**>匿名为下面的名称

```text
RECORD_KV
```

- 返回创建的workers，点击>**绑定**>**添加绑定**
- 弹出的窗口点击>**kv数据库**>**绑定**
- 出现俩个输入框都填**RECORD_KV**，点击**绑定**

### 绑定自定义域
- 打开创建的workers，点击>**设置**>**添加自定义域**>**自定义域**>填写你的域名或子域名 例如:

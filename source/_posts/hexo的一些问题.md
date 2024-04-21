---
title: Hexo的一些问题
date: 2024-04-21 10:55:31
categories: 
- 教程
tags:
- Hexo
---

记录下使用Hexo的一些问题

一、文章加密
---
使用hexo插件

1.博客目录运行命令:
```bash
npm install hexo-blog-encrypt --save
```

2.在文章信息头里添加：
```bash
password: xxx
abstract: 需要密码
message: 请输入密码
wrong_pass_message: 密码错误
```

3.重新生成文件即可。其他的详细信息可到插件文件里查看。

二、更新错误
---
在上传更新的时候报错:
```
ERROR Deployer not found: git
```
可能是没有部署git的插件

1.在博客目录里安装插件:
```bash
npm install hexo-deployer-git --save
```

2.重新生成文件上传即可。
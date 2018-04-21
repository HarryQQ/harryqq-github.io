---
title: Hexo使用
date: 2018-04-19 21:00:28
tags:
---
对比过jekyll和hexo，在windows 10下jekyll需要安装ruby环境，官方也不推荐在windows上使用，而hexo是node环境就可以，所以选择hexo。

[hexo官网](https://hexo.io/zh-cn/docs/)

#### 常用命令

    hexo new 新文章名 // 意文章
    hexo s // server开启本地调试
    hexo g -d // 生成并发布

#### 更换主题

git clone ${主题git地址} themes/${主题名}

如： git clone git@github.com:theme-next/hexo-theme-next.git themes/next

修改_config.yml文件为：

    theme: next

#### 插入图片
[参考](http://51world.win/)

配置文件开启

post_asset_folder: true
> hexo new 一个新文章，会有一个同名文件存放资源，如图片

我在[Hexo使用]文件夹存放了 baobao.jpg

    {% asset_img baobao.jpg xx %}

     <img src="baobao.jpg" height="80" width="100" />

 <img src="baobao.jpg" height="80" width="100" />


另外可以直接引用网络图片

     <img src="https://www.zoivi.cn/image/5.jpg" width="100" height="70" />

 <img src="https://www.zoivi.cn/image/5.jpg" width="100" height="70" />

#### 点击放大预览


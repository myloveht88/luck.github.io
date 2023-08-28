---
title: 更换hexo主题
tags: hexo
categories: tools
---

> **1、进入Hexo官网https://hexo.io/themes/ 选择喜欢的主题**

![](https://pic2.zhimg.com/80/v2-e3930f5c1a91cec058f8092f524e1b89_720w.webp)

> 2、在hexo目录下的themes文件夹下打开git bash，输入以下命令，下载主题:
<!-- more -->

```console
git clone 复制主题的网址

例如：D:\blog>git clone https://github.com/litten/hexo-theme-yilia.git themes/yilia
```


> 3、配置_config.yml文件
打开hexo目录下的_config.yml文件，修改theme，注意冒号之后的空格

因为刚刚已经下载过主题，打开hexo目录下的themes文件夹会看到新生成的主题文件夹，将他的名字复制到_config.yml里并保存，如图（ps：注意hexo和themes的主题文件夹里各有一个_config.yml文件，不要搞混了，后续增加各种效果还需要用到的）
> 4、在hexo目录下，打开git bash，输入以下命令，清除缓存，生成静态文件，查看效果
```git
hexo clean
hexo g
hexo s
```
感觉效果满意就可以部署到GitHub上了

5、在hexo目录下，打开git bash，输入以下命令，清除缓存，将内容部署到GitHub
```git
hexo clean
hexo g -d
```
配置完成，打开网址查看效果

![](https://pic2.zhimg.com/80/v2-e4bfa4ed074072927c3a407080bd2c75_720w.webp)
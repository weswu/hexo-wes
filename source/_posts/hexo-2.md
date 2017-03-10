---
title: hexo 认识
date: 2017-03-02 23:05:17
categories: hexo
header-img: https://hexo.io/hexo-theme-landscape/assets/wallpaper-2572384.jpg
tags: hexo
---
![zespia](https://zespia.tw/blog/2015/11/21/redux-1-to-3/53131016.png)
<!--more-->
## _config.yml
### 语言:
```
language: zh-CN
```
### 分页
```
per_page: 2
```
### 推广页面
```
plugins:
  hexo-generator-feed:
  hexo-generator-baidu-sitemap:

# sitemap
baidusitemap:
  path: baidusitemap.xm
```

```
$ npm install hexo-generator-feed --save
$ npm install hexo-generator-baidu-sitemap --save

```


### 创建文章
```
$ hexo new "文章名"
```

### 创建页面
```
$ hexo new page "book"
$ hexo new page "book-1"
menu:
  Home: /
  Archives: /archives
  Book: /book
```



### 多标签
```
tags: [hexo,git]
```
End
# hexo-wes
[![Build Status](https://img.shields.io/badge/build-passing-brightgreen.svg)](https://github.com/weswu/hexo-wes)
[![Hexo](https://img.shields.io/badge/hexo-3.2.0+-blue.svg)](https://github.com/hexojs/hexo)

一个简单博客的[hexo](https://hexo.io/themes/)主题

Demo: [landscape](http://hexo.io/hexo-theme-landscape)

## 外观

![电脑界面](http://om1ci69wa.bkt.clouddn.com/hexo-theme-wes-pc.png)
![手机界面](http://om1ci69wa.bkt.clouddn.com/hexo-theme-wes-mobile.png)

## 功能

 - 简单快速开发
 - 自由评论
 - 分享功能
 - 个性页面,值得拥有

## 安装 

  1. 电脑基本配置 
  
  node git
  
  2. 安装博客后台 
  
  ```
  $ git clone https://github.com/weswu/hexo-wes
  ```
  
  3. 安装node_modles插件
  
  ```
  $ npm install
  ```
  
# 主题配置

## 配置文件 

`_config.yml` `theme/landscape/_config.yml`

### 图标: 

`favicon: /favicon.ico`

### seo:

`keywords: Hexo, Gruntjs, Nodejs, Reactjs, Vuejs`

### 社交: 

`facebook, twitter, weibo, wechat, github, stackoverflow, linkin, email, segmentfault, flickr, zhihu, disqus`

### 个性域名: 

修改自己的二级域名 `source/CNAME` 

博客目录存入,新建远程项目(有300M空间) `用户名.github.io` 
 
```
deploy:
    type: git
    repository: git@github.com:用户名/用户名.github.io.git
    branch: master
```

### 评论

([多说](http://duoshuo.com/)): 

```
duoshuo:
  enable: true
  siteName: ueibo
```  

### 版权: 

```
copyright:
  record: false
  hexo: true
  laughing: true
```

## 运行

 1. 初始化本地项目
 
 ```
 $ hexo g
 ```
 
 2. 打开本地页面 [localhost:400](htts://localhost:4000)
 
 ```
 $ hexo s
 ```
 
 3. 初始化git项目并自动 `push`
 
 ```
 $ hexo d
 ```
 
## 参考
 
 - [MarkDown](http://www.markdown.cn/)

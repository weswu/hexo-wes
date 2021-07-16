# hexo-wes
[![Build Status](https://img.shields.io/badge/build-passing-brightgreen.svg)](https://github.com/weswu/hexo-wes)
[![Hexo](https://img.shields.io/badge/hexo-3.2.0+-blue.svg)](https://github.com/hexojs/hexo)

一个简单博客的[hexo](https://hexo.io/themes/)主题

Demo: [在线地址](http://www.weizai.party/)

## 外观

![电脑界面](http://om1ci69wa.bkt.clouddn.com/hexo-theme-wes-pc.png)
![手机界面](http://om1ci69wa.bkt.clouddn.com/hexo-theme-wes-mobile.png)


### 安装并运行
```
npm install -g hexo-cli
hexo init website-hexo
npm install
```
1. 本地服务器
```
hexo server         #运行本地服务器 localhost:4000
hexo generate       #自动根据当前目录下文件,生成静态网页
```
2. 发布到github
```
npm install hexo-deployer-git --save
hexo deploy    #生成.deploy_git文件
```

#### 配置 _config.yml
1. 自定义域名:把CNAME文件放到当前目录source文件下
2. 更新到远程
```
deploy:  
    type: git
    repository: git@github.com:weswu/weswu.github.io.git
    branch: master
```
3. 推广页面 
```
npm install hexo-generator-feed --save  # 安装插件
npm install hexo-generator-baidu-sitemap --save
```
```
plugins: 
  hexo-generator-feed:
  hexo-generator-baidu-sitemap:
# sitemap
baidusitemap:
  path: baidusitemap.xm
```

	
### 创建文章与页面
```
hexo new "文章名"
hexo new page "book"
hexo new page "book-1"
menu:
  Home: /
  Archives: /archives
  Book: /book
  	
tags: [hexo,git]
```



## 目录

<pre>
.
├── .deploy_git         // 网站代码
├── public              // 网站代码
├── scaffolds           // 模板
├── source              // 博客文章
├── themes/landscape    // 皮肤
│   ├── languages       // 语言包
│   ├── layout          // 各种组件
│   ├── scripts         // js
│   ├── source          // 静态文件
│   ├── _config.yml     // 皮肤配置文件
│   ├── Gruntfile.js    // 皮肤打包
│   .
├── _config.yml         // 配置文件
├── .gitignore          // 忽略的文件
├── .gitmodules         // 皮肤git项目地址
├── db.json             // json数据
├── gruntfile.js        // 打包
├── package.json        // 项目配置文件
├── README.md           // 说明
</pre>



## 皮肤主题

### 滚动向上

插件[material-scrolltop](https://github.com/bartholomej/material-scrolltop)



## 参考

 - [写作-MarkDown](http://www.markdown.cn/)
 - [皮肤-landscape](http://hexo.io/hexo-theme-landscape)
 - [图片-七牛云](https://www.qiniu.com/)

 - [huxpro博客](https://github.com/Huxpro/huxpro.github.io)

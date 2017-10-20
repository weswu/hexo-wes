# hexo-wes
[![Build Status](https://img.shields.io/badge/build-passing-brightgreen.svg)](https://github.com/weswu/hexo-wes)
[![Hexo](https://img.shields.io/badge/hexo-3.2.0+-blue.svg)](https://github.com/hexojs/hexo)

一个简单博客的[hexo](https://hexo.io/themes/)主题

Demo: [在线地址](http://www.weizai.party/)

## 外观

![电脑界面](http://om1ci69wa.bkt.clouddn.com/hexo-theme-wes-pc.png)
![手机界面](http://om1ci69wa.bkt.clouddn.com/hexo-theme-wes-mobile.png)


## 安装和运行

  1. 安装依赖

  ```
  $ npm install
  ```

  2. 启动本地服务器 [localhost:400](htts://localhost:4000)

  ```
  $ hexo s
  ```

  3. 初始化本地项目

  ```
  $ hexo g
  ```

  4. 初始化远程项目

  ```
  $ hexo d
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

### 个性域名:

修改自己的二级域名 `source/CNAME`

博客目录存入,新建远程项目(有300M空间) `用户名.github.io`

```
deploy:
    type: git
    repository: git@github.com:用户名/用户名.github.io.git
    branch: master
```


## 参考

 - [写作-MarkDown](http://www.markdown.cn/)
 - [皮肤-landscape](http://hexo.io/hexo-theme-landscape)
 - [图片-七牛云](https://www.qiniu.com/)

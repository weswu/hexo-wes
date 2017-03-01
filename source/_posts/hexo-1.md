---
title: 用hexo写博客
date: 2017-02-27 20:36:34
tags: hexo
---

  很早之前就想写一个博客，可是一直找不到好的tool。
  用Wordpress搭建过，感觉page不好搞，数据库也不是mysql，后来... 直到reship system。
  今天就用github pages搭建，github真是好东西，大家都知道。

### 一.hexo
本地安装Node
1.安装 hexo

```
$ npm install -g hexo-cli
```

2.建立一个博客文件夹，并初始化博客
```
$ hexo init 文件名
$ cd 文件名
```

3.安装依赖包,生成node_modules文件夹
```
$ npm install
```


### 二.github
github账号
1.新建项目   用户名.github.io

![wes](http://om1ci69wa.bkt.clouddn.com/git_pages1.png)

2.设置

![wes](http://om1ci69wa.bkt.clouddn.com/git_pages2.png)
![wes](http://om1ci69wa.bkt.clouddn.com/git_pages3.png)

3.自定义二级域名
新建CNAME文件,内容域名

![wes](http://om1ci69wa.bkt.clouddn.com/git_pages4.png)
![wes](http://om1ci69wa.bkt.clouddn.com/git_pages5.png)

4.域名服务商 设置域名解析地址

![wes](http://om1ci69wa.bkt.clouddn.com/git_pages6.png)



### 三.生成博客
1.本地服务器

```
$ hexo generate       #自动根据当前目录下文件,生成静态网页
$ hexo server         #运行本地服务
```

打开 [localhost:4000](http://localhost:4000)

2.更新到远程
修改_config.yml 
自定义域名:把CNAME文件放到当前目录source文件下

```
deploy:
    type: git
    repository: git@github.com:weswu/weswu.github.io.git
    branch: master
```

发布到github

```
$ npm install hexo-deployer-git --save
$ hexo deploy          #生成.deploy_git文件
```


# 前言

本书为个人学习计算机相关知识的笔记书，希望借由编写此书的过程中，为自己建立相对系统的计算机知识体系

书中记录相关知识来源于读书笔记、博客、个人思考等所得，在此对开源事业与知识传播者表示由衷的敬意！

## 安装Gitbook

安装`node.js`，针对Linux Deb系

```bash
$ sudo apt-get install nodejs
$ sudo apt-get install npm
```

安装`gitbook-cli`

```bash
$ sudo npm i gitbook-cli -g
```

## 安装插件

进入书目录，安装`gitbook`插件

```bash
$ gitbook install
```

## 启动服务

两种启动方式

1.  `Gitbook` 自带serve服务，优点：自动编译文本

    ```bash
    $ gitbook serve .
    ```

2.  `Nginx` 静态资源服务器

    书籍目录执行`gitbook build .`生成`_book`目录

    配置`nginx.conf`或`conf.d/default.conf`，监听端口，root定位到书籍所在目录下的_book目录

    启动`Nginx`服务即可。
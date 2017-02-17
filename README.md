# gulp-project

## 本示例目标

这是一份帮助你学习 gulp 的项目示例代码。仅仅是一份参考。请根据自己的项目对其进行修改。详情请戳[「基于 gulp 的前端构建」](https://cobish.github.io/#/post/20)。

## 学习的前提

* 了解 gulp 是做什么用的；
* 了解什么是前端项目的构建，什么是静态文件的打包。

## 构建目标

* 图片优化，雪碧图，图片 hash 戳；
* sass 编译，css 压缩合并，css 文件 hash 戳；
* js 检错，requirejs 打包，js 压缩合并，js 文件 hash 戳。

## 示例依赖

* gulp
* requirejs
* sass

## 目录结构与说明

``` bash
├─ gulp/                  # gulp配置目录
    ├─ tasks              # 任务配置目录
        ├─ image.js       # 图片配置
        ├─ other.js       # 其它配置
        ├─ script.js      # 脚本配置
        ├─ style.js       # 样式配置
        └─ view.js        # 页面配置
    └─ config             # gulp配置文件
├─ src/                   # 开发目录
    ├─ html/              # 存放html的目录
        ├─ app/           # 可提取复用的页面模块
        └─ page/          # 各页面入口文件
    ├─ images/            # 存放图片的目录
        ├─ single/        # 不需要合并的图片
        └─ sprite/        # 需要合并的图片
    ├─ js/                # 存放js的目录
        ├─ app/           # 可提取复用的脚步模块
        ├─ lib/           # 第三方js库
        ├─ page/          # 各页面入口脚本文件
        └─ config.js      # RequireJs的配置文件
    └─ sass/              # 存放sass的目录
        ├─ app/           # 可提取复用的样式模块
        └─ page/          # 各页面入口样式文件
├─ .jshintrc              # jshint参数配置文件
├─ gulpfile.js            # gulp入口配置文件
└─ package.json           # npm包管理文件
```

## 0. 依赖

### 运行环境

- node.js@5.8.0

``` bash
$ node -v
v5.8.0

$ npm -v
3.7.3
```

### 依赖

- gulp@3.9.1

``` bash
$ npm install -g gulp@3.9.1
```

## 1. 安装 NPM

首先，别忘记安装 ``npm``，一切都是基于它之上进行玩转。

``` bash
$ npm install
```

## 2. 运行命令

命令帮助：

``` bash
$ gulp help
```

运行开发命令：

``` bash
$ gulp dev
```

打包上线命令：

``` bash
$ gulp build
```

## 3. 查看源代码

了解该示例如何实现，并根据自身项目需求对其进行更改。

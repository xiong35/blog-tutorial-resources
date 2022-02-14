# 总目标: 完成博客

## Step 1 新建项目

> 前置要求：下载 git，了解 git 使用  
> ref：[廖雪峰 git](https://www.liaoxuefeng.com/wiki/896043488029600)

1. 在 github 上创建项目
2. 将项目克隆下来
3. 添加 ssh 密钥
4. 使用 vim 添加 readme 文件并提交

## Step 2 准备开发工具 - vscode

1. 下载 vscode
2. 安装插件
   1. chinese
   2. prettier
3. 配置自动格式化

## Step 3 编写代码

### 3.1 编写前端静态页面

#### 3.1.0 下载 node.js

#### 3.1.1 初始化一个 React 项目

1. 按 react 官网的指引初始化项目
   1. [beta](https://beta.reactjs.org/)
   2. [稳定版](https://reactjs.org/)
2. 启动项目
3. 随便改改看看

#### 3.1.2 React 项目的基本操作

> 前置要求：基本 html、css、js 语法  
> ref：[【极客学院】Web 前端开发教学](https://www.bilibili.com/video/BV1Mx411m7fd)，有余力可以开倍速，快速
> 上手就行，要想系统学习还得看书和多写，看视频学的还是容易忘  
> tip：下面评论区别人贴的链接都不建议学

1. 认识项目基本结构
2. jsx
3. hook
   1. useState
   2. useEffect
4. 引入样式
5. 使用 scss

#### 3.1.3 使用 React Router 来配置我们的页面

1. 什么是 react router
2. [安装](https://reactrouter.com/)
3. 随便改改试试

#### 3.1.4 开发前端页面（包含交互，不包含和后端通信）

这部分我只是抛砖引玉，样式方面有自己的想法可以不按我的来，但是为了方便后续逻辑一致，整体还是建议和我不要差太多  
建议开倍速，我码字比较慢 hhhh

#### 3.1.4.1 首页

1. 整体布局（响应式）
2. 顶部导航栏
3. 左侧侧边栏
4. 中间主体部分
   1. 博客列表
   2. 翻页器
5. 下方 footer

#### 3.1.4.2 博客详情页

1. 安装 markdown-it
2. 稍加布局

#### 3.1.4.3 管理员登录

1. 封装一下输入框的样式

#### 3.1.4.4 管理员发布

1. 需要进行鉴权，使用 token 的方式
2. 新增 tag 和新增文章

#### 3.1.4.5 【可选】个人介绍页

自由发挥可以

### 3.2 编写接口文档

见接口文档 # TODO

### 3.3 mock 前端数据

见 mock # TODO

### 3.4 根据接口文档编写后端接口

#### 3.4.1 初始化一个 Koa 项目，下载 postman，加入 nodemon

1. 去 [koa.js 官网](https://koajs.com/)找安装教程
2. 编写一个 hello world
3. 下载 [postman](https://www.postman.com/)
4. 测试一下
5. 添加 nodemon

#### 3.4.2 学习 Koa 基本操作，安装插件

1. 中间件、洋葱模型
2. 下载一些会用到的插件
   1. router
   2. body
   3. logger

#### 3.4.3 下载 MongoDB

1. 去[官网](https://www.mongodb.com/)下载
2. 讲讲 mongoDB 的基本操作-增删改查，详见 [api 文档](https://docs.mongodb.com/manual/introduction/)
3. 使用 compass 可视化

#### 3.4.4 连接 Koa 与 MongoDB

1. 下载 [mongoose](https://mongoosejs.com/)
2. 按教程链接数据库
3. 随便改改试试

#### 3.4.5 开发

##### 3.4.5.1 先把处理的空函数写出来，配置路由

1. 博文
   1. 增加
   2. 删除
   3. 修改
   4. 批量查询简略信息
   5. 查询详细信息
2. 标签
   1. 增加

##### 3.4.5.2 写下模型定义

1. 博文
2. 标签

二者是一对多的关系

##### 3.4.5.3 实现上述处理函数

### 3.5 前后端对接

1. 前端改用真实的接口

## Step 4 部署

### 4.1 租一个学生服务器

1. 租台阿里云学生服务器
2. 连接到服务器
3. linux 下基本命令的使用
   1. ls
   2. cd
   3. vim
4. 配置 ssh 登录
5. 配置 vscode 连接服务器

### 4.2 将前后端部署到服务器

1. 准备服务器环境
   1. 下载 node
   2. 下载 mongoDB
2. 将仓库克隆下来
3. 前后端 dev 启动
4. 就可以看到界面啦！

### 4.3 配置 nginx 代理

1. 下载 nginx
2. 配置代理规则
3. 前端编译
4. 后端用 pm2 启动

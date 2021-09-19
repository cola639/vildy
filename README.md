## react + react-router-dom + express + mongoDB

> 跟着MoshIfy视频教学,实现一个简易电影后台管理,下载到本地运行node监听3900端口启动后台服务

- 前后台分离式开发（项目中也包含电影的后台管理系统），为了方便记录后端开发过程，笔者将后端也一起放在同个项目文件夹中。
- 借助于 `Bootstrap`  UI 框架，主打简约风格。
- 具备了电影管理、用户注册与登录、点赞、电影修改的功能...
- 用户权限分离,对游客,注册用户授予不同权限

### 实现功能

- [x] 前台：主页 + 详情页 + 搜索页 + 分类页 
- [x] 后台：电影内容修改
- [x] 用户：站内用户
- [x] 用户可以点赞


### 技术栈

- 前端 （基于 `create-react-app eject` 后的配置）

  - `react ^16.4.1`  + `react-router4` 
  - `bootstrap` + `font-awesome`
  - `webpack` 打包优化
  - `axios` 封装

- 后端 （自构建后台项目）
  - `express` + `cors`
  - `mongoose` + `mongoDB`
  - `jwt` + `bcrypt`
  - `joi`

## 项目结构

### 目录结构

```js

│                            
├─config                // 构建配置
├─public                // html 入口
├─scripts               // 项目脚本
└─server                // 后端
    ├─config            // 项目配置 port、database、github参数 等等
    ├─middlewares       // 中间件
    ├─models            // 数据库模型
    ├─public             //存放静态图片
    ├─routes            // 路由
    ├─startup           // 启动配置
    ├─tests             // 集成测试
    ├─index.js          // 后端主入口文件
    └─...
│
└─src                   // 前端项目源码
   ├─components         // 页面组件
   ├─services           // http网络服务
   ├─utils              // 工具包
   ├─  App.js           // 路由配置
   ├─  index.js         // 主入口文件
   └─...

```



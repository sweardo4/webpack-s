# webpack 简单工作流配置

## 功能说明

1.安装依赖并运行demo

```bash
npm install
npm run dev
```

访问<http://localhost:8080/> 你就可以看到页面了

这里主要是webpack-dev-server 插件在起作用，他们在本地运行一个服务器，默认端口8080 你可以运行以下命令变更端口

```
webpack-dev-server --hot --inline --host 0.0.0.0 --port=端口号
```

2.如何在其他终端上访问
```
webpack-dev-server --public --host 192.168.1.106 --port 8080//把host地址改成本机的ip地址就可以了
```

具体关于webpack-dev-server的资料请[移步](https://github.com/e-cloud/webpack-docs/wiki/webpack-dev-server.cn)

关于其他终端访问的[问题](https://github.com/webpack/webpack-dev-server/issues/882)

3.Demo能干什么？

开发环境下

> - 自动更新编译代码
> - ~~自动刷新页面(待加入)~~
> - sass语法
> - js、css自动载入

打包

> - 编译压缩丑化js文件(webpack -p)
> - 编译sass文件、厂商前缀、压缩css文件
> - 编译html文件载入css、js

打包命令

```
npm run prod
```

## 参考资料

[官方文档](https://webpack.js.org/guides/get-started/)

[webpack 入门教程](https://llp0574.github.io/2016/11/29/getting-started-with-webpack2/)

[webpack 优秀中文文章](https://github.com/webpack-china/awesome-webpack-cn)

[webpack-docs](https://github.com/e-cloud/webpack-docs/wiki/webpack-dev-server.cn)

<http://coolnuanfeng.github.io/webpack>

<http://www.cnblogs.com/haogj/p/5160821.html>

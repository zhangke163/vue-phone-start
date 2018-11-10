我的理解是vue-cli是一个快速构建vue使用环境的一个包，
它不需要我们去安装webpack，再一个一个的手动安装和配置我们需要的基本东西。比如sass、es6等。
当然根据我们开发的项目需要什么我们再手动安装就好。
（安装文档详见npm官网）
1、全局安装
npm install vue-cli -g
2、在自己项目的文件夹安装
vue init webpack my-project



下载后运行npm run dev
手动下载我们还需要的依赖
npm install axios     //发起请求的
移动端的组件库 mint-ui

大致操作步骤
1、main.js中配置axios，给上公共的url
2、App.vue写东西
3、main.js中配置mini-ui
4、App.vue中写上头部和底部的组件
5、components里面写上各个页面的组件
6、router里面配置组件路由
7、App.vue页面监视路由和路由留坑

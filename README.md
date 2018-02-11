# 爱摆摊小程序前端开发规范

> 命令规范

- css类命名统一中杠连接
- js方法命名使用小驼峰命名

> 组件化

- css组件化，在app.wxss中将会多次出现的部分进行组件抽离，例如flex居中盒子布局代码，或者一直的功能按钮样式，保证css的复用性
- js模块化，例如时间格式处理的功能代码，接口请求的功能代码，分别封装成对应的模块，按需引入

> ui框架

- 统一使用小程序weui布局，提高开发效率

> 全局配置

- 接口统一在 根目录app.js中配置globalData中配置
- 用户token也配置globalData中，统一控制用户状态

> 静态资源体积控制

- 小程序总体积最大为2M,所以图片能放到cdn的就进行cdn配置，静态资源文件最后进行压缩，尽量缩减体积

> 其他细节

- 各种请求前的加载动效
- js操作成功失败的提示必须完整
- wxml中的js数据和事件的绑定统一写在控制样式的class之前
# 介绍
wxa是一套完善的微信小程序开发解决方案，通过Decorator增强小程序能力，基于nodejs工程化小程序开发流程，同时支持Vue单文件开发模式和原生小程序开发模式！此外还提供了一套基于wxa开发UI组件。

## 它是如何工作的？
一个`wxa`项目实际上是由`@wxa/core`，`@wxa/cli`以及小程序原生能力驱动的应用。通过cli为小程序和npm仓库搭建了直接沟通的桥梁，使得无数优秀的类库有了直接在小程序上使用的可能。而`@wxa/core`则为小程序开发提供了许多最佳实践。

## 特性
- 原生友好
    - 迁移一个旧项目到wxa只需要几分钟
    - 良好的原生组件开发支持

- 简洁好用的核心类库`@wxa/core`
    - **Decorator** 切面编程，无缝增强
    - **Mixins** 分离逻辑，复用代码，提高可维护性
    - **Plugins** 插件机制
    - **Redux** 全局状态管理方案
    - **Promise** 化小程序api
    - **Eventbus** 自定义事件
    - **Router** 路由跳转

- 功能齐全的命令行工具`@wxa/cli`
    - Npm依赖解析
    - 灵活的编译配置
        - [Tapable](https://github.com/webpack/tapable)插件机制
        - 可拔插的编译器
    - 多开发模式支持
        - 支持小程序原生开发
        - 支持Vue单文件开发模式
    - 组件良好支持
        - 原生组件
        - 第三方原生组件
    - 调用微信开发者工具
        - 上传代码
        - 预览项目

## 初衷
小程序自诞生开始，大家对改进其开发流程都有自己的见解，例如组件化方面有[zanui](https://github.com/youzan/zanui-weapp)，[weui](https://github.com/Tencent/weui-wxss/), 框架方面有[wepy](https://github.com/Tencent/wepy)。过去一年，一直在观望wepy，文档和源码都有拜读了，不得不说思路的确很惊艳，几次都想在项目中应用，又被大量issue吓退了，等到wepy相当稳定的时候，结果官方又支持了自定义组件了，于是一直都是使用自己开发部署流程在工作，的确发现有很多改进的地方，写了wxa希望能把自己的一些想法加进去。

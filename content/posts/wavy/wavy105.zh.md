---
author: ["novrain"]
title: "Wavy, 1.0.5"
date: "2024-01-11"
description: "1.0.5发布在Windows Store."
summary: "基于electron/Vue/Vuetify."
tags: ["Wavy","serial", "electron", "vue", "vuetify", "protocol", "tool", "test"]
categories: ["Code", "Wavy"]
series: ["Wavy"]
ShowToc: true
TocOpen: true
cover:
  image: assets/images/wavy.svg
  hiddenInList: true
params:
  comments: true
---

目标：支持多种连接方式的协议测试工具.

## 功能特性

- 支持Windows/Mac/Linux
- 支持多连接会话
- 支持多种编码：Hex/ASCII/Base64
- 支持仅发送选中的部分指令
- 支持工程管理，便于管理分享测试指令
- 高级命令块：
  - String: 支持长度/补齐/补齐位置/补齐长度/编码等特性
  - Decimal: 支持类型/补齐/补齐位置/补齐长度/编码/字节序等特性
  - Delay：在命令块之间插入延时
- 支持向单个会话或多个会话发送单个命令块或多个命令块
- 支持保存命令与日志为文本
  
<img src="https://raw.githubusercontent.com/novrain/wavy/master/docs/imgs/string-block.png" alt="string-block" width="300"/>
<img src="https://raw.githubusercontent.com/novrain/wavy/master/docs/imgs/decimal-block.png" alt="decimal-block" width="300"/>
<img src="https://raw.githubusercontent.com/novrain/wavy/master/docs/imgs/delay-block.png" alt="delay-block" width="300"/>

- 优化的界面，引入了Lumino, 方便的拖拽功能，改变布局，多连接时更便捷，[vue3-lumino-widget](https://github.com/novrain/vue3-lumino-widget)
- 支持Light/Dark两种主题
- 支持中文/英文

<img src="https://raw.githubusercontent.com/novrain/wavy/master/docs/imgs/dark.png" alt="SimpleBlocks" width="800"/>
<img src="https://raw.githubusercontent.com/novrain/wavy/master/docs/imgs/light.png" alt="SimpleBlocks" width="800"/>

## 安装

- Windows Store

[![windows store](https://cdn.jsdelivr.net/gh/qishibo/img/windows-store-icon182-56.png)](https://www.microsoft.com/store/apps/9PFS4672J8M2)

## 开发

### 版本要求

- Nodejs: 18.18.2
- Electron: 28.1.3

### 构建

#### 安装

```shell
yarn
```

#### 开发调试

```shell
npm run electron:dev
```

#### 构建Release

```shell
npm run vite:build
npm run forge:make
```

## 赞赏

- [A Star⭐](https://github.com/novrain/wavy)
- [给个关注](https://github.com/novrain/wavy/subscription)
- 如果觉得好用，又乐意打赏的话
  
  <img src="https://raw.githubusercontent.com/novrain/wavy/master/docs/imgs/sponsor/wechat.jpg" alt="wechat" width="200"/>

  [PayPal](https://paypal.me/novrainn)

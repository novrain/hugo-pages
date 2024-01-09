---
author: ["novrain"]
title: "Wavy, 支持多种连接方式的协议测试工具，目前仅支持串口"
date: "2023-12-26"
description: "开发一个能编辑并保存数据块、数据帧的工具。"
summary: "基于electron/Vue/Vuetify."
tags: ["serial", "electron", "vue", "vuetify", "protocol", "tool", "test"]
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

## Serial port

### UI

- 引入了Lumino, 方便的拖拽功能，改变布局，多连接时更便捷。[vue3-lumino-widget](https://github.com/novrain/vue3-lumino-widget)
- String/Decimal 命令块定义，方便编辑指令

两个串口间收发数据。

![SimpleBlocks](https://raw.githubusercontent.com/novrain/wavy/master/docs/imgs/SimpleBlocks.png)

## 开发

### 版本要求

- Nodejs: 18.18.2
- Electron: 28.0.0

### 构建

#### 安装

```shell
yarn
```

#### 安装 electron-forge 工具链

```shell
npm exec --package=@electron-forge/cli -c "electron-forge import"
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

---
author: ["novrain"]
title: "Wavy, a simple protocol testing tool that supports various connection types(now serial port only)."
date: "2023-12-26"
description: "I want to build a tool, which can edit and save data blocks and frames."
summary: "A tool build base on electron/Vue/Vuetify."
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

Target: Build a protocol testing tool that supports various connection methods.

## Serial port

### UI

- Using lumino, drag and drop function to change the layout, making it more convenient for multiple connections. [vue3-lumino-widget](https://github.com/novrain/vue3-lumino-widget)
- String/Decimal Command Blocks，easy to build command.

Send and receive data between two serial ports.

![SimpleBlocks](https://raw.githubusercontent.com/novrain/wavy/master/docs/imgs/SimpleBlocks.png)

## Development

### Versions

- Nodejs: 18.18.2
- Electron: 28.0.0

### Build

#### Install npm packages

```shell
yarn
```

#### Install electron-forge tool chains

```shell
npm exec --package=@electron-forge/cli -c "electron-forge import"
```

#### Run dev

```shell
npm run electron:dev
```

#### Build vite project and make release

```shell
npm run vite:build
npm run forge:make
```

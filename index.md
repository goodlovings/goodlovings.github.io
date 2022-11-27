---
layout: default
title: 前言
nav_order: 1
permalink: /
---

# 如何进行源码阅读

# package.json

- 1、从**main**字段确定当前项目的入口，通过入口文件和文件中引入依赖进行源码阅读；
- 2、从**xxxdependencies**字段确定当前项目以来的其他第三方库，可以初步判断该库的规模；
- 3、从**script**字段确定当前项目的执行命名，了解该项目的运行、编译、打包流程和机制；
- 4、···

# index.js

axios 的入口文件`index.js`：

```javascript
module.exports = require("./lib/axios");
```

根据引入，真正执行的文件`./lib/aixos.js`文件;

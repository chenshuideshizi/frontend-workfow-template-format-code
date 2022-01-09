# Frontend Workflow Tmplate


**使用的工具**

- husky：Git hooks 工具<br>
解决了.git文件不会被跟踪并且不会上传至远端仓库的问题


- lint-staged：检测文件插件<br>
只检测**暂存区**的文件，对过滤出的文件执行脚本


- eslint：插件化JavaScript代码检测工具<br>
Js编码规范，检测并提示错误或警告信息


- prettier：代码格式化工具<br>
代码风格管理，更好的代码风格效果


- editorconfig：文件代码规范<br>
保持多人开发一致编码样式


- commitlint：代码提交检测<br>
检测git commit 内容是否符合定义的规范


- commitizen：代码提交内容标准化<br>
提示定义输入标准的git commit 内容

### 增产提效

**1. eslint + vscode**

- 1. 在 vscode 上安装 eslint 插件
- 2. 每次保存的时候根据根目录下 .eslint.js 配置自我修正

文件 > 首选项 > 设置

```js
    "files.autoSave":"off",
    "eslint.validate": [
       "javascript",
       "javascriptreact",
       "html",
       { "language": "vue", "autoFix": true }
     ],
     "eslint.options": {
        "plugins": ["html"]
     }
```

**2. 配置 .editorconfig 文件**

配置开发时文件代码规范,保持多人开发一致编码样式

**工作流**

![流程图](./doc/前端工作流.png)

- [xmind 文件](./doc/前端工作流.xmind)
- [pdf](./doc/commit规范方案探讨.pdf)

**疑问**

eslint --fix 和 prettier 都可以实现格式化代码，它们之间有什么区别

**参考**

- Npm Life Cycle Scripts https://docs.npmjs.com/cli/v7/using-npm/scripts#life-cycle-scripts

- npm 模块管理器 http://javascript.ruanyifeng.com/nodejs/npm.html
- package.json 介绍 http://javascript.ruanyifeng.com/nodejs/packagejson.html

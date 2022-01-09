# Frontend Workflow Tmplate



这是个人总结工作流模板,学习下如何创建一个工作流,后续会慢慢增加自己所学的工程化内容进来,目前提供功能
1. `commit` 代码校验,避免错误代码提交
2. `commit-message` 提交信息校验,提交信息要规范
3. 提交信息模块是可扩展的,可以查看 `/.cz-config.js` 




### 提交增效

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

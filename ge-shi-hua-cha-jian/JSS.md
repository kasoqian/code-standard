# JSS

[JavaScript Standard Style](https://github.com/standard/standard/blob/master/docs/README-zhcn.md)

目标语言：javascript

## 介绍

JavaScript Standard Style 是一个javascript标准格式库，目前已经有27k star，同时受众多开源项目青睐。拥有它！你无需再用同时维护`eslintrc`，`jshintrc` or `jscsrc`，真正实现了开箱即用！

## 开始使用

安装JJS到开发环境。

```bash
npm install standard --save-dev
```

配置当代码更改时，执行如下命令，即可完成格式化。

```
standard --fix
```

## 强烈推荐

在package.json中补充命令，即可更方便实现对代码的格式化。

```bash
  "scripts": {
    "dev": "standard && node index.js"
  }
```

## ignore

在package.json文件中进行如下配置，即可完成ignore功能。

````js
"standard": {
  "ignore": [
    "**/out/",
    "/lib/select2/",
    "/lib/ckeditor/",
    "tmp.js"
  ]
}
````

## 相关插件推荐

安装 `vscode-standard`（已经包含了自动格式化）。

安装 `vscode-standardjs-snippets` 以获得 JS snippets。安装 `vscode-react-standard` 以获得 React snippets。
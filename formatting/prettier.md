# prettier

注意 Prettier 并不是必须的，有部分开发者认为 Prettier 的折行功能会影响开发体验。总之，是否需要 Prettier 具体还是取决于团队的选择。

**通用配置**

```js
module.exports = {
  printWidth: 80, // 一行的字符数，如果超过会进行换行
  tabWidth: 2, // 一个 tab 代表几个空格数
  useTabs: false, //是否使用 tab 进行缩进
  singleQuote: true, // 字符串是否使用单引号
  semi: true, // 行尾是否使用分号
  trailingComma: 'none', // 是否使用尾逗号
  bracketSpacing: true, // 对象大括号之间是否有空格
};
```

# eslint

**通用配置**

此处默认使用 TypeScript，因为现在 TypeScript 已经是开发的标配了。 

```js
module.exports = {
  env: {
    browser: true,
    es2021: true,
  },
  extends: [
    "eslint:recommended",
    "plugin:react/recommended",
    "plugin:@typescript-eslint/recommended",
    // 如果你不使用 Prettier，要去掉下面两行
    "prettier",
    "plugin:prettier/recommended",
  ],
  parser: "@typescript-eslint/parser",
  parserOptions: {
    ecmaFeatures: {
      jsx: true // jsx 配置
    },
    ecmaVersion: "latest",
    sourceType: "module",
  },
  plugins: ["react", "@typescript-eslint", "prettier"],
  rules: {
    "prettier/prettier": "error", // Prettier 自动修复
    quotes: ["error", "single"], // 单引号
    semi: ["error", "always"], // 分号
    "react/react-in-jsx-scope": "off", // 使用 jsx 不需要引入 React，目前新版本的 React 不需要每次使用都引入
  },
};
```


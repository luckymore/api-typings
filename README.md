# 支付宝小程序类型定义

[![npm package](https://img.shields.io/npm/v/@mini-types/alipay.svg?style=flat-square)](https://www.npmjs.com/package/@mini-types/alipay)
[![GitHub stars](https://img.shields.io/github/stars/ant-mini-program/api-typings.svg)](https://github.com/ant-mini-program/api-typings/stargazers)
[![GitHub forks](https://img.shields.io/github/forks/ant-mini-program/api-typings.svg)](https://github.com/ant-mini-program/api-typings/network/members)
[![NPM downloads](https://img.shields.io/npm/dm/@mini-types/alipay.svg?style=flat-square)](https://www.npmjs.com/package/@mini-types/alipay)
[![GitHub issues](https://img.shields.io/github/issues/ant-mini-program/api-typings.svg)](https://github.com/ant-mini-program/api-typings/issues)

支付宝小程序的 TypeScript 类型定义文件。

需要使用 TypeScript 4.1+。

## 如何使用

首先需要安装 npm 包：

```sh
npm install @mini-types/alipay --save-dev
# or
yarn add -D @mini-types/alipay
```

然后使用 typeRoots 来配置：

```json
{
   "compilerOptions": {
      "typeRoots" : ["./node_modules/@mini-types", "./node_modules/@types"]
   }
}
```

此外，还可以在 `tsconfig.json` 文件中指定 `types` 配置。

```json
{
   "compilerOptions": {
      "types": ["@mini-types/alipay"]
   }
}
```

## FAQ

### 我在代码中使用 `this.` 时没有提示？

请在项目的 tsconfig.json 中配置 `noImplicitThis` 为 `true`：

```diff
{
  "compilerOptions": {
+    "noImplicitThis": true
  },
}
```

## 如何贡献

`@mini-types/my` 中的类型定义是通过工具自动生成的，最好不要直接向该包提交代码。如果发现定义有误欢迎给我们提 issue。

`@mini-types/global` 中是 Page/Component 等的类型定义，如果发现定义有误欢迎给我们提 PR。

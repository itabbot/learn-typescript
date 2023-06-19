# TypeScript：最简单的 Vue.js 应用<!-- omit in toc -->

## 1. 步骤

1. 执行 Vue 脚手架并选择支持 TypeScript

```sh
> npm init vue@latest

Need to install the following packages:
  create-vue@latest
Ok to proceed? (y) y

Vue.js - The Progressive JavaScript Framework

√ Project name: ... simplest-vuejs-app
√ Add TypeScript? ... Yes
√ Add JSX Support? ... No
√ Add Vue Router for Single Page Application development? ... No
√ Add Pinia for state management? ... No
√ Add Vitest for Unit Testing? ... No
√ Add an End-to-End Testing Solution? » No
√ Add ESLint for code quality? ... No
```

2. 安装 VS Code 插件

- `Vue.volar`
- `Vue.vscode-typescript-vue-plugin`

3. 安装依赖

```sh
> npm install
```

4. 编译和热重载（用于开发）

```sh
> npm run dev

  VITE v4.3.9  ready in 544 ms

  ➜  Local:   http://127.0.0.1:5173/
  ➜  Network: use --host to expose
  ➜  press h to show help
```

5. 编译和压缩（用于生产）

```sh
> npm run build

vite v4.3.9 building for production...
✓ 26 modules transformed.
dist/assets/logo-277e0e97.svg    0.28 kB │ gzip:  0.20 kB
dist/index.html                  0.42 kB │ gzip:  0.29 kB
dist/assets/index-bc8397f3.css   3.69 kB │ gzip:  1.19 kB
dist/assets/index-ad5bbf45.js   60.10 kB │ gzip: 23.89 kB
✓ built in 1.04s
```

## 2. 理解

- 初始化：使用 Vue 官方脚手架工具搭建时，选择支持 TypeScript，会自动创建相关的配置文件和代码。
- 开发和构建：Vite 本身会自动识别 TypeScript 文件并自动进行类型检查和编译处理。
- 编译器：TypeScript 编译器 `tsc` 无法识别 `.vue` 文件，需要改用 `vue-tsc` 来执行编译或类型检查。

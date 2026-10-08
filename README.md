# qxj-frontend-mock

QXJ 前端 Mock Demo「改造后」版本的**静态部署仓**：内容为
`qxj-frontend-mock-demo`（after）构建出的纯静态文件（`index.html` + `assets/`），
通过 GitHub Pages 发布。

线上访问：<https://etsuyou.github.io/qxj-frontend-mock/>

## 说明

- 资源以子路径 `/qxj-frontend-mock/` 引用（GitHub Pages 项目站点）；
- 该仓不存放源码，只存放构建产物；源码与改造前后对照见
  `qxj-frontend-mock-demo` 仓库；
- 页面通过 `qxj-frontend-sdk` + mock-jsbridge 演示 JSBridge 登录
  （`VITE_ENABLE_MOCK_JSBRIDGE`），登录页为 `/mock-login`。

## 更新方式

在源码仓构建后，将产物覆盖到本仓：

```bash
# 在 qxj-frontend-mock-demo（after）中
pnpm build
# 把 dist 内容复制到本仓根目录并提交推送，GitHub Pages 自动更新
```

# Tessera 插件目录

由 Tessera 仓库的 `bun run catalog:publish --base-url https://raw.githubusercontent.com/quoteZZZ/tessera-plugins/main` 生成。

- `catalog.json` — 插件市场读取的索引（schemaVersion 1）
- `*.tgz` — 对应版本的插件包（安装前校验 sha256）

## 用法

启动 Tessera 宿主时设置环境变量：

```
TESSERA_CATALOG_URL=https://raw.githubusercontent.com/quoteZZZ/tessera-plugins/main/catalog.json
```

市场面板会出现「目录」段；已安装的插件不会重复显示。

目录与包均由工具生成，请勿手改。

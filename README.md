# Tessera 插件目录

由 Tessera 仓库的

```
bun run catalog:publish --base-url https://raw.githubusercontent.com/quoteZZZ/tessera-plugins/main --extra examples/clock
```

生成。

- `catalog.json` — 插件市场读取的索引（schemaVersion 1）
- `*.tgz` — 对应版本的插件包（安装前校验 sha256）

## 用法

在 `tessera.config.json` 里写 `catalogUrl`，或启动时设置：

```
TESSERA_CATALOG_URL=https://raw.githubusercontent.com/quoteZZZ/tessera-plugins/main/catalog.json
```

市场面板的「目录」段只列出**尚未安装**的条目。`clock` 是示例插件（状态栏时钟），
用来验证「目录 → 安装 → 重启 → 生效」。

目录与包均由工具生成，请勿手改。

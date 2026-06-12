# WC2026 私人 AI 分析台 v20

这是一个单 HTML 的 2026 世界杯私人分析工具。

## 定位

- 私人使用
- 本机保存 API Key
- 手动刷新真实赛程 / 比分
- 由 AI 分析比赛、球队、风险和结论
- 不接后端服务
- 不接数据库
- 不写死任何 API Key

## 本地使用

推荐本地运行：

```bat
run-local.bat
```

然后打开：

```text
http://127.0.0.1:8088
```

也可以直接打开 `index.html`。

## API Key 安全说明

OpenAI API Key、football-data.org Key、API-FOOTBALL Key 都只保存在当前浏览器的 `localStorage`。

- 不会写进 `index.html`
- 不会上传到 GitHub
- 不会自动请求外部 API
- 清除浏览器数据会删除 Key

## 手动请求原则

页面打开时不会自动请求：

- OpenAI
- football-data.org
- API-FOOTBALL

只有手动点击对应按钮才会请求：

- 使用 OpenAI 分析
- 测试 OpenAI 连接
- 刷新真实赛程 / 比分
- 测试赛程 API 连接

## 数据说明

页面默认包含 Demo / Mock / Sample 数据。
如果本机存在真实赛程缓存或手动导入数据，会优先用于 AI Prompt 和分析上下文。

## 风险提示

本工具仅用于赛事分析、学习和情景推演。
模拟预测、示例赔率和模型输出不构成投注建议。

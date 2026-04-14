# Changelog

## Mu0.0.1 - 2026-04-14

### Fix
- 修复公网场景大文件上传失败（默认最大上传体积提升到 1GB，可通过 `MAX_CONTENT_LENGTH` 环境变量覆盖）。
- 上传接口增加缺失文件字段的显式提示，避免前端静默失败。

### Feature
- 新增下载接口：`GET /download/<path>`（仅允许下载 `static/files` 内分离结果文件）。
- Web 页面结果区新增“下载/Download”按钮，支持公网直接下载转换后的音频。

### Ops
- `web_address` 改为支持环境变量 `WEB_ADDRESS` 配置，便于公网部署时生成正确访问地址。


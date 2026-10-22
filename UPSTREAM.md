# 上游来源与本 Fork 维护

## 来源与固定版本

| 项目 | 当前记录 |
| --- | --- |
| 原项目 | [satnaing/shadcn-admin](https://github.com/satnaing/shadcn-admin) |
| 个人 Fork | [haers/zhao-shadcn-admin](https://github.com/haers/zhao-shadcn-admin) |
| 官方 Demo | [shadcn-admin.netlify.app](https://shadcn-admin.netlify.app/) |
| 本地体验与采用对照提交 | [`e16c87f213a5ba5e45964e9b67c792105ec74d26`](https://github.com/satnaing/shadcn-admin/commit/e16c87f213a5ba5e45964e9b67c792105ec74d26) |
| package.json 版本 | `2.2.1` |
| `v2.2.1` 标签实际提交 | `0217f8cb73af66f3cbf4141d5e0d00e1c5c30434`，与本次体验提交不同 |
| 许可证 | [MIT](LICENSE)，Copyright (c) 2024 Sat Naing |
| 最近体验与记录日期 | 2026-10-23 |

## 本 Fork 的维护范围

保留上游源码、锁文件、原始许可证和完整 Git 历史。新增中文介绍、运行方式、采用关系及精选截图；原 README 仅增加中文入口。目录及 GitHub 仓名称为 `zhao-shadcn-admin`，包名和上游应用品牌保留原样。

本仓暂不进行功能开发、不接入真实业务后端。业务适配由使用方各自维护，不从这里自动覆盖。

## Git 远端

```text
origin    https://github.com/haers/zhao-shadcn-admin.git
upstream  https://github.com/satnaing/shadcn-admin.git
```

`origin` 是本 Fork，`upstream` 是原作者仓库。

## 按需更新

有明确需要的能力或修复时，再检查上游差异。先确认工作树和当前本地修改已妥善保存，然后取回远端信息：

```sh
git status --short
git fetch upstream
git log --oneline e16c87f213a5ba5e45964e9b67c792105ec74d26..upstream/main
git diff --stat e16c87f213a5ba5e45964e9b67c792105ec74d26 upstream/main
```

网络访问遵循当前机器的代理约定。`fetch` 只取回信息，不把上游变更直接合入工作树。

确认更新价值后，在独立分支审阅依赖、组件改动与中文说明冲突，按需合并；保留上游许可证与本地文档。完成构建与受影响页面验证后，才修改本文件的固定提交和截图日期。失败时保留已验证版本，记录阻塞原因；不通过强制重置解决冲突。

本 Fork 按需更新，不设置自动同步，不代表官方维护关系或持续追更承诺。

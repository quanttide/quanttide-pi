# 量潮 Pi 智能体（quanttide-pi）

量潮第二大脑适配轴（adapters/）的 Pi 智能体适配仓库。

## 定位

把 `domains/` 的领域知识接通到 Pi 智能体：负责提示词装配、上下文装载与工具对接，不生产领域事实，只做接通。

- 上游：`domains/` 领域知识
- 下游：Pi 智能体

## 结构

| 路径 | 说明 |
|------|------|
| `data/context` | Pi 智能体语境 (git submodule → quanttide-context-of-pi-agent) |
| `docs/handbook` | Pi 智能体手册 (git submodule → quanttide-handbook-of-pi-agent) |
| `docs/gallery` | Pi 智能体案例集 (git submodule → quanttide-gallery-of-pi-agent) |

`data/` 放装载进运行时的记忆资产，`docs/` 放供人阅读的文档产物。

其余随实现演进补充。

## 许可

[CC BY 4.0](LICENSE)

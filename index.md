# 首页

本页按主题汇总仓库内容：每节先说明主题是什么，再列出语境、手册、案例与工具的去处。

## pi-hermes-memory

pi-hermes-memory 是 Pi 的持久记忆扩展：`MEMORY.md`、`USER.md`、`STANDING.md` 与项目级 `MEMORY.md` 是事实源，`sessions.db` 是从中派生的检索索引，冲突时以事实源为准。默认 policy-only 模式下完整记忆不进上下文，靠 agent 自行搜索，记忆因而只具便条效力，当前请求、仓库文件与工具输出优先；`STANDING.md`（`/memory-pin`）是例外，每轮注入且 agent 不可写，是唯一能承载授权的地方，预算 20 条 / 2000 字符。

- 语境：[数据事实源与检索索引](data/context/library/pi-hermes-memory.md)、[洞察：库记事实，你记授权](data/context/insight/pi-hermes-memory.md)；
- 报告：[记忆维护报告（2026-10-04）](data/context/report/2026-10-04-pi-memory-maintenance.md)。
- 手册：[使用规范：记忆四层存放、机制边界、生命周期](docs/handbook/pi-hermes-memory/index.md)、[memory-pin 文案规范](docs/handbook/pi-hermes-memory/memory-pin.md)；
- 案例：[提示词原文三件](docs/gallery/pi-hermes-memory/index.md)（memory-pin、memory-policy、后台复习）；
- 工具：[`pi-hermes-memory` Rust 只读适配包](packages/quanttide-pi-toolkit/packages/rust/crates/pi-hermes-memory/README.md)。

# 项目知识索引

当前状态：模板。以下文件是填写大纲，尚不代表真实项目能力。

每次开始任务先读取本文件，再按需深入。初始化任务优先读取原始需求和已确定决策，之后用实际实现补全知识。

| 文件 | 内容 | 何时读取 |
| --- | --- | --- |
| [01-project-overview.md](01-project-overview.md) | 目标、范围、技术栈与状态 | 首次接手或理解项目边界 |
| [02-architecture.md](02-architecture.md) | 系统组成、依赖方向和关键链路 | 设计与跨模块修改 |
| [03-directory-structure.md](03-directory-structure.md) | 目录职责、入口与文件定位 | 找代码或新增模块 |
| [04-development-guide.md](04-development-guide.md) | 环境、启动、检查与构建 | 本地开发与验证 |
| [05-core-business.md](05-core-business.md) | 业务流程、状态、权限与不变量 | 业务实现和排错 |
| [06-config-and-datasource.md](06-config-and-datasource.md) | 配置、环境和数据源 | 配置与数据变更 |
| [07-external-integrations.md](07-external-integrations.md) | 外部系统与工具入口 | 集成开发和故障定位 |
| [08-dev-conventions.md](08-dev-conventions.md) | 规范索引与已知约束 | 日常开发与交接 |

## 维护规则

- 文档区分：已验证事实、已确定但未实现的设计、待解决问题。
- 关键事实附真实代码/配置路径、需求编号或决策来源；运行结果附验证记录。
- 找不到依据时写 `[待补充]`，无此能力时写“不适用：原因”。
- 重要变更后检查相关条目和索引，更新事实，移除过时内容。
- 过程与临时进度留在 `.tasks/`，设计取舍留在 `docs/decisions/`；索引不堆积会话日志。
- 专题足够复杂时再新增文件，并在此登记，不预先制造业务专题。

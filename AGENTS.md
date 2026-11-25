# AI 协作入口

## 开始工作

1. 先读 [.memories/README.md](.memories/README.md)，按任务需要读取对应知识文件。
2. 查看 `.tasks/` 中相关任务，延续已有决策和进度。
3. 读取下面列出的适用规则；不要假设客户端自动加载 `.agents/`。
4. 若项目尚处模板状态，按 [docs/bootstrap.md](docs/bootstrap.md) 初始化。

## 规则与技能路由

| 触发条件 | 必读来源 |
| --- | --- |
| 编码或设计变更 | [.agents/rules/engineering.md](.agents/rules/engineering.md) |
| 验证、修复和交付 | [.agents/rules/verification.md](.agents/rules/verification.md) |
| 根据需求创建新项目或补齐初始化阶段 | [.agents/skills/project-bootstrap/SKILL.md](.agents/skills/project-bootstrap/SKILL.md) |
| 接入或使用外部工具 | [.agents/mcp/README.md](.agents/mcp/README.md) |

新增专项规则时在此登记触发条件和路径。子目录如需额外约束，使用该目录的 `AGENTS.md`，只补充其职责范围内的差异。客户端的指令优先级以实际运行环境为准。

## 工作约定

- 实现前说明关键假设、范围和可验证目标。影响业务含义、技术栈或数据操作的歧义需澄清；常规实现细节沿用已确定规范。
- 保持最小改动，不附带无关重构，不增加没有需求依据的依赖或基础设施。
- 尊重已有工作，不覆盖他人的未提交修改。
- 按既有授权完成工作；访问工具的能力不等于对外发布、数据写入或其他外部操作的授权。
- 不把凭据、个人数据、内部环境地址从其他项目带入本项目。
- 交付时说明修改、验证结果和剩余事项，不把计划或未运行的命令描述为已完成。

## 项目专属约定

初始化时在本节填写已确定的架构边界、命令文档链接、专项规则入口和环境操作限制。技术栈未确定前，不在这里写入特定语言或框架的要求。

当前状态：模板；项目专属约定 `[待补充]`。

## 知识维护

重要功能、架构调整、性能优化或 Bug 修复后，检查受影响的 `.memories/`。更新长期有效的事实和入口；本次过程留在 `.tasks/`，取舍留在 `docs/decisions/`。没有知识变化时无需制造文档改动。

# 使用 Superpowers 工作流进行开发

Superpowers 是一套面向技能的工程工作流，Trae 会在合适的场景自动触发相关技能，帮助你从设计到交付全流程高效推进。使用方式如下：

- 启动设计（触发 brainstorming）：在对话中描述目标与约束，让助手提问梳理，并给出可选方案与设计文档草案供确认。
- 生成实施计划（触发 writing-plans）：设计确认后，请助手把需求拆成可执行的小任务，明确文件路径、代码片段与验证步骤。
- 创建隔离开发环境（触发 using-git-worktrees）：为本次变更创建独立工作树和分支，安装依赖并跑一遍基线测试，确保环境干净。
- 按计划执行（触发 subagent-driven-development）：逐任务调度子代理执行，先核对与计划的符合度，再进行代码质量与测试的审查。
- 严格 TDD（触发 test-driven-development）：每个任务先写失败用例，再写最小通过实现，保持红→绿→重构的节奏，避免超前实现。
- 阶段评审（触发 requesting-code-review）：在任务间或合并前进行结构化评审，按严重级别列出问题并先解决阻塞项。
- 收尾分支（触发 finishing-a-development-branch）：在所有测试通过后，选择合并或创建 PR，并清理临时工作树保持仓库整洁。

无需额外配置，以上技能已内置于项目的 .trae/skills 目录并按场景自动触发；你也可以在对话中直接给出上述阶段的指令，以加速进入对应的工作流。

## 快速开始
- 设计：说“帮我梳理这个功能的设计与可选方案”（触发 brainstorming）
- 计划：说“把设计拆成可执行任务并给出验证步骤”（触发 writing-plans）
- 环境：说“为本功能创建独立工作树并跑基线测试”（触发 using-git-worktrees）
- 执行：说“按计划逐任务执行并进行两阶段评审”（触发 subagent-driven-development）
- TDD：说“先写失败用例再最小实现，保持红绿重构”（触发 test-driven-development）
- 评审：说“做一次结构化代码评审并列出问题级别”（触发 requesting-code-review）
- 收尾：说“选择合并或 PR，并清理工作树”（触发 finishing-a-development-branch）

## 技能索引与示例
- 设计：[brainstorming](file:///Users/bytedance/Work/ai_learn/ai_trae_superpower_gomoko/.trae/skills/brainstorming/SKILL.md) —— 触发前请描述目标、约束与背景
- 计划：[writing-plans](file:///Users/bytedance/Work/ai_learn/ai_trae_superpower_gomoko/.trae/skills/writing-plans/SKILL.md) —— 每个任务需包含路径、代码与验证
- 工作树：[using-git-worktrees](file:///Users/bytedance/Work/ai_learn/ai_trae_superpower_gomoko/.trae/skills/using-git-worktrees/SKILL.md) —— 创建隔离环境并验证测试基线
- 执行：[subagent-driven-development](file:///Users/bytedance/Work/ai_learn/ai_trae_superpower_gomoko/.trae/skills/subagent-driven-development/SKILL.md) —— 子代理两阶段评审推进
- TDD：[test-driven-development](file:///Users/bytedance/Work/ai_learn/ai_trae_superpower_gomoko/.trae/skills/test-driven-development/SKILL.md) —— 先红后绿再重构
- 评审：[requesting-code-review](file:///Users/bytedance/Work/ai_learn/ai_trae_superpower_gomoko/.trae/skills/requesting-code-review/SKILL.md) —— 按严重级别输出问题与措施
- 收尾：[finishing-a-development-branch](file:///Users/bytedance/Work/ai_learn/ai_trae_superpower_gomoko/.trae/skills/finishing-a-development-branch/SKILL.md) —— 选择合并或 PR 并清理工作树

## 安装说明
- 在 Trae IDE 中，.trae/skills 目录下的技能会被自动加载，无需额外安装。
- 若在其他平台使用，请参考 Superpowers 文档：https://github.com/obra/superpowers

<p align="center">
  <h1 align="center">Claude Code 游戏工作室</h1>
  <p align="center">
    将单一 Claude Code 会话转变为完整的游戏开发工作室
    <br />
    48 个代理 · 37 个工作流 · 一个协同的 AI 团队
  </p>
</p>

<p align="center">
  <a href="LICENSE"><img src="https://img.shields.io/badge/license-MIT-blue.svg" alt="MIT 许可证"></a>
  <a href=".claude/agents"><img src="https://img.shields.io/badge/代理-48-blueviolet" alt="48 个代理"></a>
  <a href=".claude/skills"><img src="https://img.shields.io/badge/技能-37-green" alt="37 个技能"></a>
  <a href=".claude/hooks"><img src="https://img.shields.io/badge/钩子-8-orange" alt="8 个钩子"></a>
  <a href=".claude/rules"><img src="https://img.shields.io/badge/规则-11-red" alt="11 条规则"></a>
  <a href="https://docs.anthropic.com/en/docs/claude-code"><img src="https://img.shields.io/badge/构建于-Claude%20Code-f5f5f5?logo=anthropic" alt="构建于 Claude Code"></a>
  <a href="https://ko-fi.com/donchitos"><img src="https://img.shields.io/badge/Ko--fi-支持本项目-ff5e5b?logo=ko-fi&logoColor=white" alt="Ko-fi"></a>
</p>

---

## 项目初衷

独自使用 AI 开发游戏确实强大 —— 但单一的聊天会话缺乏结构。没有人阻止你硬编码魔法数字、跳过设计文档、或者编写面条代码。没有 QA 流程，没有设计审查，没有人问"这真的符合游戏的愿景吗？"

**Claude Code 游戏工作室** 通过赋予你的 AI 会话真实工作室的结构来解决这个问题。不再是单一的通用助手，你将获得 48 个按工作室层级组织的专业化代理 —— 负责把控愿景的总监、负责各自领域的部门主管、以及执行具体工作的专家。每个代理都有明确的职责、升级路径和质量门禁。

结果：你仍然做出每一个决策，但现在你有一个团队会提出正确的问题、及早发现错误，并从最初的头脑风暴到发布都保持项目有序。

---

## 目录

- [包含内容](#包含内容)
- [工作室层级](#工作室层级)
- [斜杠命令](#斜杠命令)
- [快速开始](#快速开始)
- [升级指南](#升级指南)
- [项目结构](#项目结构)
- [工作原理](#工作原理)
- [设计哲学](#设计哲学)
- [自定义](#自定义)
- [平台支持](#平台支持)
- [社区](#社区)
- [许可证](#许可证)

---

## 包含内容

| 类别 | 数量 | 描述 |
|------|------|------|
| **代理** | 48 | 覆盖设计、编程、美术、音频、叙事、QA 和生产的专业化子代理 |
| **技能** | 37 | 常用工作流的斜杠命令（`/start`、`/sprint-plan`、`/code-review`、`/brainstorm` 等） |
| **钩子** | 8 | 提交、推送、资源变更、会话生命周期、代理审计和缺口检测时的自动验证 |
| **规则** | 11 | 编辑玩法、引擎、AI、UI、网络代码等时自动执行的路径作用域编码标准 |
| **模板** | 29 | GDD、ADR、冲刺计划、经济模型、阵营设计等文档模板 |

## 工作室层级

代理按三个层级组织，模拟真实工作室的运作方式：

```
Tier 1 — 总监层 (Opus)
  creative-director（创意总监）    technical-director（技术总监）    producer（制作人）

Tier 2 — 部门主管层 (Sonnet)
  game-designer（游戏设计师）        lead-programmer（首席程序员）       art-director（美术总监）
  audio-director（音频总监）         narrative-director（叙事总监）      qa-lead（QA主管）
  release-manager（发布经理）        localization-lead（本地化主管）

Tier 3 — 专家层 (Sonnet/Haiku)
  gameplay-programmer（玩法程序员）  engine-programmer（引擎程序员）     ai-programmer（AI程序员）
  network-programmer（网络程序员）   tools-programmer（工具程序员）      ui-programmer（UI程序员）
  systems-designer（系统设计师）     level-designer（关卡设计师）        economy-designer（经济设计师）
  technical-artist（技术美术）       sound-designer（音效设计师）        writer（编剧）
  world-builder（世界构建师）        ux-designer（UX设计师）             prototyper（原型师）
  performance-analyst（性能分析师）  devops-engineer（DevOps工程师）     analytics-engineer（数据分析师）
  security-engineer（安全工程师）    qa-tester（QA测试员）               accessibility-specialist（无障碍专家）
  live-ops-designer（长线运营设计师） community-manager（社区经理）
```

### 引擎专家

模板包含三大主流引擎的代理集。使用与你的项目匹配的那一套：

| 引擎 | 主管代理 | 子专家 |
|------|----------|--------|
| **Godot 4** | `godot-specialist` | GDScript、着色器、GDExtension |
| **Unity** | `unity-specialist` | DOTS/ECS、着色器/VFX、Addressables、UI Toolkit |
| **Unreal Engine 5** | `unreal-specialist` | GAS、蓝图、网络复制、UMG/CommonUI |

## 斜杠命令

在 Claude Code 中输入 `/` 访问全部 37 个技能：

**审查与分析**
`/design-review` `/code-review` `/balance-check` `/asset-audit` `/scope-check` `/perf-profile` `/tech-debt`

**生产管理**
`/sprint-plan` `/milestone-review` `/estimate` `/retrospective` `/bug-report`

**项目管理**
`/start` `/project-stage-detect` `/reverse-document` `/gate-check` `/map-systems` `/design-system`

**发布流程**
`/release-checklist` `/launch-checklist` `/changelog` `/patch-notes` `/hotfix`

**创意设计**
`/brainstorm` `/playtest-report` `/prototype` `/onboard` `/localize`

**团队编排**（协调多个代理完成单一功能）
`/team-combat` `/team-narrative` `/team-ui` `/team-release` `/team-polish` `/team-audio` `/team-level`

## 快速开始

### 前置要求

- [Git](https://git-scm.com/)
- [Claude Code](https://docs.anthropic.com/en/docs/claude-code)（`npm install -g @anthropic-ai/claude-code`）
- **推荐**：[jq](https://jqlang.github.io/jq/)（用于钩子验证）和 Python 3（用于 JSON 验证）

所有钩子在可选工具缺失时会优雅降级 —— 不会出错，只是失去部分验证功能。

### 安装步骤

1. **克隆或使用模板**：
   ```bash
   git clone https://github.com/Donchitos/Claude-Code-Game-Studios.git my-game
   cd my-game
   ```

2. **打开 Claude Code** 并启动会话：
   ```bash
   claude
   ```

3. **运行 `/start`** — 系统会询问你的当前状态（无想法、模糊概念、清晰设计、已有工作）并引导你到合适的工作流。不做任何假设。

   如果你已经知道需要什么，也可以直接跳转到特定技能：
   - `/brainstorm` — 从零开始探索游戏创意
   - `/setup-engine godot 4.6` — 如果你已经知道，配置你的引擎
   - `/project-stage-detect` — 分析现有项目

## 升级指南

已经在使用此模板的旧版本？请参阅 [UPGRADING.md](UPGRADING.md) 获取分步迁移说明、版本间变更明细，以及哪些文件可以安全覆盖、哪些需要手动合并。

## 项目结构

```
CLAUDE.md                           # 主配置文件
.claude/
  settings.json                     # 钩子、权限、安全规则
  agents/                           # 48 个代理定义（markdown + YAML 前置信息）
  skills/                           # 37 个斜杠命令（每个技能一个子目录）
  hooks/                            # 8 个钩子脚本（bash，跨平台）
  rules/                            # 11 条路径作用域编码标准
  docs/
    quick-start.md                  # 详细使用指南
    agent-roster.md                 # 完整代理表及领域
    agent-coordination-map.md       # 委托和升级路径
    setup-requirements.md           # 前置条件和平台说明
    templates/                      # 28 个文档模板
src/                                # 游戏源代码
assets/                             # 美术、音频、VFX、着色器、数据文件
design/                             # GDD、叙事文档、关卡设计
docs/                               # 技术文档和 ADR
tests/                              # 测试套件
tools/                              # 构建和流水线工具
prototypes/                         # 一次性原型（与 src/ 隔离）
production/                         # 冲刺计划、里程碑、发布跟踪
```

## 工作原理

### 代理协调

代理遵循结构化的委托模型：

1. **垂直委托** — 总监委托给主管，主管委托给专家
2. **横向咨询** — 同级代理可以互相咨询，但不能做出跨领域的约束性决策
3. **冲突解决** — 分歧升级到共同父级（设计冲突找 `creative-director`，技术冲突找 `technical-director`）
4. **变更传播** — 跨部门变更由 `producer` 协调
5. **领域边界** — 代理未经明确委托不得修改其领域外的文件

### 协作而非自主

这**不是**自动驾驶系统。每个代理都遵循严格的协作协议：

1. **提问** — 代理在提出方案前先提问
2. **展示选项** — 代理展示 2-4 个选项及优缺点
3. **你做决定** — 用户永远做最终决定
4. **展示草案** — 代理在最终确定前展示工作成果
5. **审批确认** — 没有你的签字，什么都不写入

你保持掌控。代理提供结构和专业知识，而非自主权。

### 自动化安全

**钩子** 在每次会话中自动运行：

| 钩子 | 触发时机 | 功能 |
|------|----------|------|
| `validate-commit.sh` | `git commit` | 检查硬编码值、TODO 格式、JSON 有效性、设计文档章节 |
| `validate-push.sh` | `git push` | 推送到受保护分支时警告 |
| `validate-assets.sh` | `assets/` 文件写入 | 验证命名规范和 JSON 结构 |
| `session-start.sh` | 会话开启 | 加载冲刺上下文和最近 git 活动 |
| `detect-gaps.sh` | 会话开启 | 检测新项目（建议 `/start`）和代码/原型存在时缺失的文档 |
| `pre-compact.sh` | 上下文压缩 | 保存会话进度笔记 |
| `session-stop.sh` | 会话关闭 | 记录完成事项 |
| `log-agent.sh` | 代理启动 | 所有子代理调用的审计跟踪 |

`settings.json` 中的**权限规则**自动允许安全操作（git status、测试运行）并阻止危险操作（force push、`rm -rf`、读取 `.env` 文件）。

### 路径作用域规则

编码标准根据文件位置自动执行：

| 路径 | 强制内容 |
|------|----------|
| `src/gameplay/**` | 数据驱动值、delta time 使用、无 UI 引用 |
| `src/core/**` | 热路径零分配、线程安全、API 稳定性 |
| `src/ai/**` | 性能预算、可调试性、数据驱动参数 |
| `src/networking/**` | 服务器权威、版本化消息、安全性 |
| `src/ui/**` | 无游戏状态所有权、本地化就绪、无障碍 |
| `design/gdd/**` | 必需 8 个章节、公式格式、边界情况 |
| `tests/**` | 测试命名、覆盖率要求、测试夹具模式 |
| `prototypes/**` | 放宽标准、必需 README、假设文档化 |

## 设计哲学

此模板基于专业游戏开发实践：

- **MDA 框架** — 机制、动态、美学分析法用于游戏设计
- **自我决定理论** — 自主性、能力感、关联性驱动玩家动机
- **心流状态设计** — 挑战-技能平衡促进玩家投入
- **Bartle 玩家类型** — 受众定位和验证
- **验证驱动开发** — 先写测试，再实现

## 自定义

这是一个**模板**，而非锁定框架。一切都是可自定义的：

- **添加/删除代理** — 删除你不需要的代理文件，为你的领域添加新的
- **编辑代理提示词** — 调整代理行为，添加项目特定知识
- **修改技能** — 调整工作流以匹配你团队的流程
- **添加规则** — 为你的项目目录结构创建新的路径作用域规则
- **调整钩子** — 调整验证严格度，添加新检查
- **选择你的引擎** — 使用 Godot、Unity 或 Unreal 代理集（或不用）

## 平台支持

在 **Windows 10** + Git Bash 环境下测试。所有钩子使用 POSIX 兼容模式（`grep -E` 而非 `grep -P`）并包含缺失工具的降级方案。无需修改即可在 macOS 和 Linux 上工作。

## 社区

- **讨论区** — [GitHub Discussions](https://github.com/Donchitos/Claude-Code-Game-Studios/discussions) 用于提问、创意分享和展示你的作品
- **问题反馈** — [Bug 报告和功能请求](https://github.com/Donchitos/Claude-Code-Game-Studios/issues)

---

*本项目正在积极开发中。代理架构、技能和协调系统已经稳固可用 —— 但还有更多内容即将推出。*

## 许可证

MIT 许可证。详见 [LICENSE](LICENSE)。

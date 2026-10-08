# dependence（依赖声明）

本技能**不内嵌**其他技能内容；能力经声明依赖获得。每行一条 `名称 | 类型 | 来源`，类型为 skill|software|repo。SMS 安装时对本目录条目与本体做同样检查与净化。
```
file_ops          | skill    | local:skill_manage_system
code-guidelines   | skill    | local
pavedpath-code    | skill    | local
ui-design           | skill | local
database-management | skill | local
concurrency-design  | skill | local
web-design-expert   | skill    | local
python-expert       | skill    | local
cpp-expert          | skill    | local
c-expert            | skill    | local
interface-design-expert | skill | local
qt-qtquick-expert   | skill    | local
windows-app-dev-expert | skill | local
linux-dev-expert    | skill    | local
web-app-dev-expert  | skill    | local
python            | software | system
git               | software | system
```
## 用途映射
| 依赖 | 承担能力 | 触发节点 |
|---|---|---|
| file_ops | 联网搜索/抓取（ff_lite.py search/fetch·须 :grant network） | 经验查询 / 浏览器学习 / 知识库构建 |
| code-guidelines | 命名、注释、复杂度、坏味道准则 | 脚本构建 / 整体审查 |
| pavedpath-code | 已验证实现路径与脚手架范式 | 大纲构建 / 分支分析 / 脚本构建 |
| ui-design | UI/视觉/交互/无障碍专项（流程同本体） | 大纲构建 / 分支分析命中 UI 专项时 |
| database-management | 建模/SQL/迁移/性能/备份专项（流程同本体） | 分支分析命中数据专项时 |
| concurrency-design | 并发/内存模型/锁与无锁/取消安全专项 | 分支分析命中并发专项时 |
| python | 脚本运行时与测试执行器 | 脚本构建 / 构建测试 |
| git | 功能分支→dev→main 版本流 | 每步收尾（见 git 工作流约束） |
| web-design-expert | Web 视觉/交互/响应式/无障碍专项指导 | 经验查询 / 需求确认·命中该语言或方向任务时 |
| python-expert | Python 语言与生态专项指导 | 经验查询 / 需求确认·命中该语言或方向任务时 |
| cpp-expert | C++ 语言/内存/模板/并发专项指导 | 经验查询 / 需求确认·命中该语言或方向任务时 |
| c-expert | C 语言/指针/内存/可移植性专项指导 | 经验查询 / 需求确认·命中该语言或方向任务时 |
| interface-design-expert | 接口/契约设计专项指导 | 经验查询 / 需求确认·命中该语言或方向任务时 |
| qt-qtquick-expert | Qt/Qt Quick 框架专项指导 | 经验查询 / 需求确认·命中该语言或方向任务时 |
| windows-app-dev-expert | Windows 桌面/安装包/服务专项指导 | 经验查询 / 需求确认·命中该语言或方向任务时 |
| linux-dev-expert | Linux 构建打包/systemd 服务化专项指导 | 经验查询 / 需求确认·命中该语言或方向任务时 |
| web-app-dev-expert | Web 前后端契约/部署安全专项指导 | 经验查询 / 需求确认·命中该语言或方向任务时 |

## 规则
1. 依赖缺失时**降级不得静默**：记 process_chain interrupt 并向用户报告缺项，禁止伪造能力。
2. 禁止把依赖技能正文复制进本技能目录（薄技能原则）；只允许引用其名称与调用方式。
3. 新增/删除依赖须走 update 审批流并记 CHANGELOG。
4. 专项技能（ui-design / database-management / concurrency-design / web-design-expert / python-expert / cpp-expert / c-expert / interface-design-expert / qt-qtquick-expert / windows-app-dev-expert / linux-dev-expert / web-app-dev-expert）只传「意图+参数」，由对方在其目录内独立执行；索引见 [references](../references/references.md)。

- 返回 [SKILL.md](../SKILL.md) · [浏览器学习约束](../resistance/浏览器学习约束/浏览器学习约束.md)

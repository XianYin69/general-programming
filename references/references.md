# references（知识库索引）

本目录存**摘要与出处**，不存受版权保护的正文。两类来源标注：
`[联网]` = knowledge_fetch/convert 抓取可溯；`[本地]` = 模型既有常识，未经联网确证（本环境 Wikipedia 不可达，已按知识库构建兜底降级并如实标注，禁止当作已验证事实引用）。

## 编程侧

| 领域 | 条目 | 来源 |
|---|---|---|
| 代码质量 | [清洁代码](代码质量/清洁代码.md) · [Google风格指南](代码质量/Google风格指南.md) | [本地] · [联网] |
| 编程实践 | [务实程序员](编程实践/务实程序员.md) · [代码大全](编程实践/代码大全.md) | [本地] |
| 设计模式 | [GoF设计模式](设计模式/GoF设计模式.md) · [重构](设计模式/重构.md) | [本地] |
| 算法 | [算法导论](算法/算法导论.md) · [代码预训练模型](算法/代码预训练模型.md) | [本地] · [联网] |
| 领域建模 | [领域驱动设计](领域建模/领域驱动设计.md) | [本地] |

## 项目侧

| 领域 | 条目 | 来源 |
|---|---|---|
| 项目管理 | [人月神话](项目管理/人月神话.md) · [人件](项目管理/人件.md) | [本地] |
| 敏捷流程 | [Scrum指南](敏捷流程/Scrum指南.md) | [联网] |

## 专项技能索引（外置薄技能·只引用不内嵌）

| 专项 | 技能 | 知识库入口 | 何时派发 |
|---|---|---|---|
| UI 设计 | ui-design | [references](../../ui-design/references/references.md) | 视觉/交互/无障碍任务 |
| 数据库管理 | database-management | [references](../../database-management/references/references.md) | 建模/SQL/迁移/备份任务 |
| 并发设计 | concurrency-design | [references](../../concurrency-design/references/references.md) | 线程/锁/内存模型/异步任务 |
| Web 设计 | web-design-expert | [knowledge](../../web-design-expert/knowledge/knowledge.md) | Web 界面/前端任务 |
| Python | python-expert | [知识树](../../python-expert/references/知识树/知识树.md) | Python 脚本与服务任务 |
| C++ | cpp-expert | [references](../../cpp-expert/references/references.md) | C++ 项目任务 |
| C | c-expert | [references](../../c-expert/references/references.md) | C 语言与系统底层任务 |
| 接口设计 | interface-design-expert | [知识树](../../interface-design-expert/references/知识树/知识树.md) | 接口/API/契约设计任务 |
| Qt/Qt Quick | qt-qtquick-expert | [知识树](../../qt-qtquick-expert/references/知识树/知识树.md) | Qt/Qt Quick/QML 桌面与嵌入式 UI 任务 |

派发方式：只传「意图+参数」，专项技能在其目录内按同流程独立执行并收口返回（薄技能规则 4）。

## 拓扑判据与收口

- 展开链：代码质量 → 编程实践 → 设计模式/重构 → 领域建模 → 算法 → 测试 → 项目管理 → 人因 → 流程。
- 收口条件：新增主题不再引出未覆盖的相邻领域 → 停止。
- 缺口（安全、性能）属**按需触发**，由 [浏览器学习](../branch/流程/浏览器学习/浏览器学习.md)
  在遇到时补齐，不预建空目录；并发/数据/UI 已升级为专项技能（见上表）。

## 使用规则

1. 引用 `[本地]` 条目须先经浏览器学习确证再落实现；`[联网]` 条目可直接引用并附 URL。
2. 每条目 ≤50 行；超出即拆子主题。
3. 缓存 HTML 落用户缓存/tmp，禁止入本目录。

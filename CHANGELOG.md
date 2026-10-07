# CHANGELOG

## 0.1.0 — 初版（general-programming）

- 新增：创建路径 13 节点（镜像 Skill_Generator 十节点 + 构建测试 + 浏览器学习 + 修改流程）。
- 新增：五大机制约束（垃圾回收 / 上下文压缩 / 逻辑链 / 过程链存取 / 惩罚）与沙盒机制。
- 新增：`dependence/` 薄技能依赖声明（file_ops / code-guidelines / pavedpath-code / python / git），
  能力经声明获取，本体不内嵌他技能正文。
- 新增：`resistance/浏览器学习约束/` 红线——遇不明必派 file_ops 联网学习并蒸馏入知识链。
- 新增：`references/` 知识库八域索引（代码质量 / 编程实践 / 设计模式 / 算法 / 领域建模 /
  项目管理 / 敏捷流程），联网条目带出处，未联网确证条目显式标注 `[本地]`。
- 新增：`scripts/` 16 个英文命名脚本，全部 ≤50 行、语法零错误、lint 零问题。
- 新增：MIT `LICENSE`（工作区根 + tmp 镜像）。
- 违规后果：见各约束文件；约束变更须走 [update 审批流](update/update.md)。

## 0.1.1 — 专项技能索引注入

- 新增：dependence 声明 ui-design / database-management / concurrency-design 三个专项薄技能（只引用不内嵌）。
- 新增：references 增设「专项技能索引」表——各专项知识库入口与派发时机；并发/数据/UI 缺口由按需浏览器学习升级为专项技能承接。
- 规则：派发只传「意图+参数」，专项技能在其目录内独立执行收口（薄技能规则 4）。

## 0.1.2 — 仓库可见性规则

- 新增：`resistance/git工作流约束` 第 11 条「仓库可见性」——存在侵犯著作权、损害人类社会、涉嫌违法等
  违规内容的可能，或含用户需保密部分的仓库，可见性必须 PRIVATE；其他仓库一律 PUBLIC。
- 规则：建仓/推送前先判定可见性，判定不了时询问用户，不得擅自设为 PUBLIC。
- 违规后果：违规/涉密仓库设为 PUBLIC → 侵权与泄密扩散，不可撤回。
- 同步：SKILL.md 红线摘要与 `branch/流程/收尾/收尾.md` 各加一句可见性判定。

## 0.1.3 — 注册接口设计与 Qt 专家技能

- 新增：dependence 声明 `interface-design-expert`（接口/契约设计专项指导）与 `qt-qtquick-expert`
  （Qt/Qt Quick 框架专项指导）两个专项薄技能，触发节点＝经验查询 / 需求确认·命中该方向任务时。
- 新增：`dependence/deps.json` 两条 skill 条目（source_url `local://…`·license MIT·version 0.1.0·
  source_url_status verified），deps_check 缺失 = 0。
- 新增：references「专项技能索引」两行，入口指向各技能 `references/知识树/知识树.md`（已实测存在·悬空链接 0）。
- 规则：薄技能原则不变——只引用名称与入口，不内嵌他技能正文；派发只传「意图+参数」。
- 排版：dependence.md / references.md 合并个别折行以满足 .md ≤50 行红线（内容无删减）。

## 0.1.4 — 注册平台三专家技能

- 新增：dependence 声明 windows-app-dev-expert / linux-dev-expert / web-app-dev-expert 三个专项薄技能，承担能力分别＝Windows 桌面/安装包/服务专项指导、Linux 构建打包/systemd 服务化专项指导、Web 前后端契约/部署安全专项指导，触发节点＝经验查询 / 需求确认·命中该语言或方向任务时。
- 新增：`dependence/deps.json` 三条 skill 条目（type=skill·source_url `local://<name>`·license MIT·version local·source_url_status verified·checked_at 当轮时刻），插在 qt-qtquick-expert 之后、python 软件条目之前，deps_check 缺失 = 0。
- 新增：references「专项技能索引」三行，知识库入口按实测存在路径给：windows→`references/references.md`，linux 与 web→`references/知识树.md`（三者落盘结构不同，均实测存在，不写不存在路径以免悬空链接）。
- 同步：SKILL.md 工作原则 6 的薄技能枚举补齐这三项，使 dependence.md / deps.json / references.md / SKILL.md 四处口径一致。
- 规则：薄技能原则不变——只引用名称与入口，严禁把三技能正文复制进 general-programming；派发只传「意图+参数」。
- 排版：dependence.md 合并首段折行、删「## 用途映射」与「| 触发节点 |」分隔行间空行并合并两处表格行折行；references.md 合并导语、缺口条目与各索引行折行、删表前一空行；SKILL.md 原则 6 由两行折行改三行折行——三文件吸收 3 行新增后仍 ≤50 行、语义无删减；本文件历史条目排版未动，仅追加本节。

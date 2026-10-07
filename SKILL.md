---
name: general-programming
version: 0.1.0
description: >
  通用编程技能：接收编程任务→澄清需求→回忆经验→规划大纲→分析分支/语言→写代码→构建测试→审查→交付；
  薄技能（能力经 dependence/ 声明），遇不明处强制派发 file_ops 联网学习并沉淀知识链。
license: MIT
metadata:
  category: development
---

# general-programming

使用 `general-programming` skill 来完成用户请求。

## 工作原则

1. **按流程执行**：不跳步、不静默越权；决策节点留逻辑链。
2. **双链辩论**：审查节点运行正反双链（logic_chain.py debate）。
3. **返回机制**：审查失败记中断（process_chain.py interrupt），修复后 resume；任一路径完成＝收口返回调度方整合续排。
4. **惩罚熔断**：重试达 10 次即熔断，强制回退或求助用户。
5. **垃圾回收**：tmp 收尾后释放到目标 skill 并删除；未指定目录时固定路径沙盒作业。
6. **薄技能**：本体不内嵌他技能内容，能力经 [dependence/](dependence/dependence.md) 声明；UI/数据库/并发专项经其索引派发。
   Web/Python/C++/C/接口设计/Qt 与 Qt Quick、Windows/Linux/Web 应用专家技能（web-design-expert /
   python-expert / cpp-expert / c-expert / interface-design-expert / qt-qtquick-expert /
   windows-app-dev-expert / linux-dev-expert / web-app-dev-expert）同经该索引派发，只传意图+参数。

## 执行路径

**创建路径**：初始化→需求确认→经验查询→大纲构建→分支分析→脚本构建→构建测试→知识库构建→浏览器学习→约束编写→整体审查→收尾→**完成**
**修改路径**：初始化→修改流程→**完成**

> 浏览器学习为横切节点：任一步遇到不明 API/库/报错即触发，学完沉淀知识链再回原节点。

## 可用工具（scripts/）

check_links / logic_chain / process_chain / garbage_collect / context_compress / penalty /
sandbox / deps_check / run_tests / lint_check / browser_learn / scaffold_project

## 红线

- 不得跳过初始化（含 MIT `LICENSE`，已有不覆盖）；不得静默写盘（默认 `--dry-run`）；不得删除 resistance/ 约束。
- 悬空链接必须为 0；所有 .md ≤ 50 行（50 行红线只约束 markdown 文本；脚本 .py/.ps1/.sh/.cmd 不限行数，但仍禁裸 except、print 调试残留、>100 字符长行、超长函数）；缓存文件不得写入 skill 目录（落用户缓存目录）。
- 文件夹名=流程名；脚本使用英文名称；SKILL.md 必含 YAML frontmatter；agent/ 四格式提示词一句话。
- 遇不明必派 file_ops 联网学习（见 [浏览器学习约束](resistance/浏览器学习约束/浏览器学习约束.md)），禁止凭记忆臆造 API。
- Git 工作流：每步功能分支提交→审核通过合 dev→整体审查通过 dev 合 main 并推送（推送前须用户确认；疑似违规或涉密仓库须 PRIVATE，见 [git工作流约束](resistance/git工作流约束/git工作流约束.md)第 11 条）。

## 详细流程

- 流程节点：[branch/流程/](branch/流程/流程.md)；约束兜底：[resistance/](resistance/resistance.md)

# dependence（依赖声明）

声明本技能包依赖的技能包/软件/仓库地址：每行一条 `名称 | 类型 | 来源`，类型为 skill|software|repo：

```
safe-mouse-automation | skill | gh:owner/repo
pandas | software | pip
```

SMS 包管理器安装技能包时，本目录条目与技能包本体接受同样的检查与净化（trust 标注·未审/隔离拒装·仓库下载须网络授权·见 skill_manage_system pkg_deps.py），审过后方可下载安装执行。

# 刘禹锡·分清条件与行动空间

分清条件与行动空间：有资料依据、有使用边界、可复核的中文 Agent Skill。

**把熟悉的思想，变成下一次任务可用的方法。**

适合：把失败全怪运气、辨认可以改变与不能控制的部分。

交付：记录事件与目标 → 列自然条件、制度条件、他人选择与自身行动 → 为每项写可控程度及证据 → 找可行动的小范围 → 比较改善条件、请求支持与改变目标的代价 → 输出行动空间图。

**一分钟看懂**：求职三次失败便认为自己注定不行。

本 Skill 会这样处理：核岗位匹配、材料和市场条件；选择可改善的作品与反馈，不把结果当命运或人格。

[用途与同类差异](references/positioning.md)。人物知名度提供发现入口，实际价值来自工作流与可复核产物；不保证星标增长。

## 安装与使用
公开仓库直接提供 Skill，不依赖 GitHub Release。
```sh
npx skills add constantin2088/liu-yuxi-agency-skill
```
也可将仓库内容复制到支持该格式的客户端 Skill 目录，保留以 `liu-yuxi-agency-skill` 命名的文件夹和根目录 SKILL.md。客户端支持范围以其文档为准。安装后提出具体任务，由客户端按描述加载。

**试用任务**：求职三次失败便认为自己注定不行。

## 内容
- [执行说明](SKILL.md)
- [资料卡](references/sources.md)、[工作表](references/frameworks.md)、[边界](references/boundaries.md)
- [三个示例](examples/demo.md)、[十个行为评测场景](evals/test-cases.md)

## 验证与贡献
```sh
python scripts/check_skill.py . --release
python -m unittest discover -s tests -v
python scripts/check_links.py
```
`--release` 是完整性检查参数，不创建 GitHub Release。CI 在每次提交运行上述检查。独立客户端模型行为评测尚未执行；用例、结构检查与实际模型能力分开报告。
修改时提供来源和定位，区分原文与转译；运行检查后直接提交到仓库。不要创建发布附件作为必需安装步骤。系列标识、链接和推荐由总仓库 catalog/skills.json 同步，避免手工修改受管理区块。

## 许可
项目原创内容使用 [MIT](LICENSE)。链接所指第三方作品保留原权利，本仓库不重新许可它们。

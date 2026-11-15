# US Tenbagger Stock Picker

[English](README.md) · **简体中文**

“它能成长十倍吗？”值得好奇，也值得把计算过程写出来。

一个研究美股长期成长候选公司的 Codex Skill，结合因子检查和每股价值复利框架，研究企业变大之后，每位股东能否真正受益。

## 研究哪些问题

Skill 对十个维度分别给出 0–3 分的研究评分：起始市值、估值差异、盈利质量、每股自由现金流变化、再投资质量、Costco 式规模共享、NVDA 式技术积累、数据或 AI 的持续反馈、价格趋势与回撤、宏观流动性。

输出包括投资假设、评分表、商业模式分类、市场可能忽略的部分、需要核验的指标、推翻判断的条件和研究结论。评分帮助组织研究，结果不代表收益预测。

## 安装与调用

在仓库根目录执行：

```bash
mkdir -p ~/.codex/skills/us-tenbagger-stock-picker
cp SKILL.md ~/.codex/skills/us-tenbagger-stock-picker/SKILL.md
```

```text
使用 us-tenbagger-stock-picker 深入研究 TICKER。
提供评分表、模式分类、需要核验的指标，以及会推翻判断的证据。
```

也可以快速筛选、比较两家公司，或建立研究名单。[HIMS 示例](examples/hims-example.md)展示交付结构；其中数据与判断需要按研究日期重新核验。

## 始终需要回答

公司为什么能够变得更大？市场价格隐含了什么？每股价值如何增长？股份稀释、经营失败和大幅回撤会怎样影响结果？

使用时需要财报、公告和当前行情。Skill 提供研究流程，使用者需要独立验证资料并作出决策。完整说明见 [SKILL.md](SKILL.md)。

[MIT License](LICENSE)。

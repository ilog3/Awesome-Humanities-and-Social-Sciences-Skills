# 来源与许可声明 / Credits & Licensing

## 一、版权归属 / Ownership

本 `skill-library/` 下的 **30 个 Skill 的内容均为原创**，源自开源项目 [OpenAgentHarness](https://github.com/openagentharness) 生态中的教育研究技能包（`education-research-skills/`）与学者蒸馏技能（`.agents/skills/scholar-distill/`）。

- 29 个 `education-*` Skill：原创方法论，围绕教育研究论文写作、统计分析与研究设计编写。
- `scholar-distill`：原创学者画像蒸馏方法论。

未从任何第三方 Skill 库（如 inno-agent-hub）复制内容。各 Skill 的 `SKILL.md` 文本、工作流与输出规范均为本项目自研。

## 二、开源许可 / License

本仓库声明采用 MIT License（README 徽标与声明）。

```
MIT License

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software...
```

> ⚠️ **仓库暂缺独立 LICENSE 文件**：README 声明了 MIT 许可，但仓库根目录未提交独立的 `LICENSE` 文件（历史提交 "Create LICENSE" 实际未包含许可文本）。如需对外正式开源，请在仓库根添加标准 MIT LICENSE 文件。

## 三、第三方工具与方法引用 / Third-Party Tool & Method References

以下 Skill 在**工作流中调用或参考**了第三方工具/API/方法论。这些工具是"被调用的外部资源"，其本身有各自的许可证与条款，**不包含**在本 Skill 包内。使用对应 Skill 前请遵守各工具的许可条款：

| Skill | 引用的第三方工具/方法 | 链接 | 说明 |
|---|---|---|---|
| `education-topic-decomposition` | STORM（Stanford） | https://github.com/stanford-oval/storm | 多视角提问启发引擎，仅参考其提问思路 |
| `education-evidence-check` | Scite, Elicit | https://scite.ai/ , https://elicit.com/ | 引文语境与证据报告服务 |
| `education-literature-map` | VOSviewer, bibliometrix | https://www.vosviewer.com/ , https://www.bibliometrix.org/ | 文献计量可视化工具 |
| `education-systematic-review-preparation` | PRISMA/PRISMA-ScR, Rayyan, Covidence | https://www.prisma-statement.org/ , https://www.rayyan.ai/ , https://www.covidence.org/ | 系统综述报告规范与筛选工具 |
| `education-theory-framework-matching` | ResearchRabbit, Litmaps, Connected Papers | https://www.researchrabbit.ai/ , https://www.litmaps.com/ , https://www.connectedpapers.com/ | 引文网络探索工具 |
| `education-sampling-data-management`, `education-quantitative-study-design` | G\*Power | https://www.psychologie.hhu.de/ | 功效与样本量计算 |
| `education-meta-analysis-preparation` | R `metafor`/`meta` | https://cran.r-project.org/package=metafor | 元分析统计包 |
| 多个 Skill | OpenAlex API | https://docs.openalex.org/ | 学术元数据检索（无需 Key，建议 mailto） |
| 多个 Skill | Semantic Scholar API | https://www.semanticscholar.org/product/api | 论文检索（可选 Key） |

**使用说明**：上述工具仅作为 Skill 工作流中可选的外部调用，未在任何 Skill 中嵌入或复制这些工具的代码、UI 或内容。若需商用或二次分发，请同时遵守各工具的许可条款。

## 四、若引用他人 Skill 的标注规范 / Attribution for Third-Party Skills

后续若向本库补充来自其他开源项目的 Skill，请在对应 `SKILL.md` 的 frontmatter 中标注：

```yaml
---
name: example-skill
category: 研究检索
source:
  origin: original            # original=自研 | collected=收集
  author: 作者名
  repo: https://github.com/xxx/repo
  license: MIT                # 原项目的开源许可
  note: 迁移时如需改动的说明
---
```

若原作者要求署名或限制用途，必须在 `SKILL.md` 正文顶部附上原作者与原始链接。

---

*文档生成于 2026-08-03。*

# Awesome Humanities and Social Sciences Skills

人文与社会科学研究技能库 — 面向教育研究、社会科学与学术写作的可迁移 Skill 集合。

每个 Skill 为独立目录，包含 `SKILL.md`（YAML frontmatter：`name` / `category` / `description`），可直接打包为 `.zip` 上传到支持 Skill 的 Agent 平台（如 Inno Agent等）。

> 分类规范：`研究检索` / `教学辅导` / `开发工具` 三类，标签拼写需与此表完全一致。

---

## Reference
本技能库同步发布 【至Inno Agent项目】，相关项目资源：
- Inno Agent 主项目：https://github.com/hhyqhh/inno-agent
- Inno Agent Hub 资源仓库：https://github.com/Chloris-Blaxk/inno-agent-hub.git

---

## Skill 清单

### 研究检索（11 个）

| Skill | 功能描述 | 目录 |
|---|---|---|
| `education-evidence-check` | Use when checking whether claims, theory choices, research questions, variable relationshi… | `education-evidence-check/` |
| `education-literature-map` | Use when creating education literature maps, bibliometric analyses, keyword co-occurrence … | `education-literature-map/` |
| `education-meta-analysis-preparation` | Use for education meta-analysis papers or systematic reviews that quantitatively synthesiz… | `education-meta-analysis-preparation/` |
| `education-paper-type-router` | Use after an education research topic and research questions are drafted, or whenever the … | `education-paper-type-router/` |
| `education-policy-comparative-analysis` | Use for education policy analysis, curriculum standard analysis, comparative education pap… | `education-policy-comparative-analysis/` |
| `education-research-question-generation` | Use when generating, refining, comparing, or validating education research questions and h… | `education-research-question-generation/` |
| `education-systematic-review-preparation` | Use for education systematic reviews, scoping reviews, evidence maps, and rigorous literat… | `education-systematic-review-preparation/` |
| `education-theory-framework-matching` | Use when matching an education research topic, question, or variable model to appropriate … | `education-theory-framework-matching/` |
| `education-topic-decomposition` | Use when decomposing a broad education research topic into focused subtopics, searchable c… | `education-topic-decomposition/` |
| `education-variable-identification` | Use when identifying independent variables, dependent variables, mediators, moderators, co… | `education-variable-identification/` |
| `scholar-distill` | Use when distilling a scholar, professor, research group, or intellectual lineage into an … | `scholar-distill/` |

### 教学辅导（10 个）

| Skill | 功能描述 | 目录 |
|---|---|---|
| `education-action-research-design` | Use for teacher-led action research, teaching practice papers, classroom improvement studi… | `education-action-research-design/` |
| `education-design-based-research` | Use for design-based research (DBR) in education, including iterative design of learning e… | `education-design-based-research/` |
| `education-learning-analytics-design` | Use for learning analytics, educational data mining, LMS log analysis, AI platform behavio… | `education-learning-analytics-design/` |
| `education-mixed-methods-design` | Use for education papers combining quantitative and qualitative data, including explanator… | `education-mixed-methods-design/` |
| `education-program-evaluation` | Use for education program evaluation, curriculum evaluation, platform/tool evaluation, tea… | `education-program-evaluation/` |
| `education-psychometric-scale-development` | Use for education scale development, questionnaire validation, test development, rubric va… | `education-psychometric-scale-development/` |
| `education-qualitative-study-design` | Use for qualitative education papers including case study, interview study, classroom obse… | `education-qualitative-study-design/` |
| `education-quantitative-study-design` | Use for education papers using quantitative survey, correlational, regression, experimenta… | `education-quantitative-study-design/` |
| `education-sampling-data-management` | Use before collecting education research data, or when planning samples, recruitment, part… | `education-sampling-data-management/` |
| `education-survey-instrument-design` | Use when designing survey instruments, questionnaires, scales, rubrics, or measurement too… | `education-survey-instrument-design/` |

### 开发工具（9 个）

| Skill | 功能描述 | 目录 |
|---|---|---|
| `education-advanced-quantitative-modeling` | Use when education research needs advanced quantitative modeling beyond common t-tests, AN… | `education-advanced-quantitative-modeling/` |
| `education-ai-assisted-qualitative-analysis` | Use when applying AI to support qualitative education analysis, including initial coding s… | `education-ai-assisted-qualitative-analysis/` |
| `education-coder-reliability` | Use when education qualitative or content-analysis projects involve multiple coders, codin… | `education-coder-reliability/` |
| `education-descriptive-statistics` | Use after quantitative education data cleaning to summarize datasets before reliability, v… | `education-descriptive-statistics/` |
| `education-inferential-statistics` | Use after descriptive statistics when an education research project needs hypothesis testi… | `education-inferential-statistics/` |
| `education-learning-analytics-modeling` | Use after learning analytics or educational data mining data are available and cleaned, es… | `education-learning-analytics-modeling/` |
| `education-qualitative-coding-analysis` | Use when analyzing qualitative education data such as interviews, focus groups, classroom … | `education-qualitative-coding-analysis/` |
| `education-quantitative-data-cleaning` | Use after quantitative education data are collected and before descriptive, inferential, r… | `education-quantitative-data-cleaning/` |
| `education-validity-reliability-analysis` | Use when education research uses scales, questionnaires, tests, rubrics, or latent constru… | `education-validity-reliability-analysis/` |

---

共 30 个 Skill。
## 使用说明

1. 下载单个 Skill 目录（含 `SKILL.md` 及其子目录），打包为 `.zip`。
2. 在目标 Agent 平台上传该 `.zip`，即可按 `category` 归类使用。
3. 统计/建模类 Skill 依赖 Python（pandas / scipy / statsmodels / R 等），按需安装。
4. 检索类 Skill 使用 OpenAlex、Semantic Scholar 等开放学术接口，无需 API Key 即可使用（有 Key 效果更佳）。

---

## 许可与来源 / License & Credits


- **许可**：本仓库声明采用 [MIT License](../../LICENSE)（README 徽标声明；仓库暂未提交独立 LICENSE 文件，如需正式开源请补充）。
- **第三方工具引用**：部分 Skill 在工作流中调用或参考了外部工具/API（STORM、OpenAlex、Semantic Scholar、Scite、PRISMA 等），这些工具本身有各自的许可条款，且**不包含**在本 Skill 包内。
- **完整明细**：参见 [CREDITS.md](./CREDITS.md)。

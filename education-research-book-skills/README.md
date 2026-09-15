# 教育研究参考书 Book Skills

这是一个面向教育研究、质性研究、民族志、访谈、案例研究和教育思想研究的 Agent Skills 合集。仓库中的 27 个 Skill 分别对应一本参考书；它们不会融合成一个总 Skill，从而保留每本书独立的概念体系、研究立场、方法流程和适用边界。

这些 Skill 使用 [book-to-skill](https://github.com/virgiliojr94/book-to-skill) 从合法取得的本地资料中生成。它们是结构化、可执行的学习与研究辅助材料，不包含原书文件，也不用于替代原著。

## 工作方式

每个 Skill 都把一本书转换为一组可供 Agent 调用的研究工具：

- `SKILL.md`：触发条件、核心框架、任务流程、方法边界和主题索引。
- `chapters/`：按主题组织的详细知识，由 Agent 在需要时加载。
- `patterns.md`：可以反复应用的研究方法与操作模式。
- `cheatsheet.md`：方法选择、判断规则和快速检查表。
- `glossary.md`：关键概念及其含义。
- `agents/openai.yaml`：供支持该格式的 Agent 发现 Skill 的元数据。

这种结构让 Agent 先加载简短的核心规则，再根据问题读取相关章节，而不是每次加载所有内容。

## Skill 目录

| # | 参考书或主题 | Skill 名称 |
|---:|---|---|
| 01 | 陈向明主编《教育研究方法》（2013） | `chen-xiangming-education-research-methods-2013` |
| 02 | Wiersma、Jurs《教育研究方法导论》第9版 | `wiersma-jurs-education-research-methods` |
| 03 | Johnson、Christensen《教育研究：定量、定性和混合方法》第4版 | `johnson-christensen-education-research` |
| 04 | Creswell、Guetterman《Educational Research》第6版 | `creswell-guetterman-educational-research` |
| 05 | Jorgensen《参与观察法》 | `participant-observation-jorgensen` |
| 06 | Clandinin、Connelly《叙事探究》 | `clandinin-connelly-narrative-inquiry` |
| 07 | 杨宝忠《大教育视野中的家庭教育》 | `yang-family-education-system` |
| 08 | Muncey、McQuillan《学校和课堂中的改革与抗拒》 | `muncey-mcquillan-reform-resistance` |
| 09 | 贺晓星《教育中的权力／知识分析》 | `interview-power-knowledge-china` |
| 10 | 叶澜《教育概论》 | `ye-lan-education-system` |
| 11 | Wolcott《校长办公室的那个人》 | `wolcott-principal-office-ethnography` |
| 12 | Yin《案例研究：设计与方法》第五版 | `yin-case-study-research` |
| 13 | Fetterman《民族志：步步深入》 | `ethnography-step-by-step-fetterman` |
| 14 | Benedict《菊与刀》 | `benedict-chrysanthemum-sword` |
| 15 | Mead《萨摩亚人的成年》 | `coming-of-age-samoa-mead` |
| 16 | 赵娟《流动人口家庭子女教养方式的质性研究》 | `migrant-family-parenting-qualitative` |
| 17 | Mauss《礼物》 | `mauss-gift-exchange` |
| 18 | Whyte《街角社会》 | `whyte-street-corner-society` |
| 19 | 《质性研究方法导论》 | `qualitative-research-methods-introduction` |
| 20 | Corbin、Strauss《质性研究的基础》 | `corbin-strauss-grounded-theory` |
| 21 | Rubin、Rubin《质性访谈方法》 | `rubin-responsive-qualitative-interviewing` |
| 22 | 白芸《质的研究指导》 | `qualitative-research-guidance-baiyun` |
| 23 | 陈向明《质的研究方法与社会科学研究》 | `chen-xiangming-qualitative-research` |
| 24 | 陆有铨《躁动的百年》 | `lu-youquan-twentieth-century-education-history` |
| 25 | Thompson《过去的声音：口述史》 | `thompson-oral-history` |
| 26 | 佐藤学《静悄悄的革命》 | `quiet-revolution-learning-community` |
| 27 | 《现代中国精神：知名教育家的生活故事》 | `modern-china-educator-life-stories` |

## 安装

先克隆这个私有仓库，然后将需要的 Skill 复制到 Codex 的个人 Skill 目录。

安装全部 Skill：

```bash
mkdir -p ~/.codex/skills
cp -R skills/. ~/.codex/skills/
```

只安装一个 Skill，例如 Creswell–Guetterman 教育研究方法：

```bash
mkdir -p ~/.codex/skills
cp -R skills/creswell-guetterman-educational-research ~/.codex/skills/
```

安装后请新建或重启 Agent 会话，让 Skill 列表重新加载。

如果使用其他兼容 Agent，可将相同的 Skill 目录复制到该 Agent 的个人 Skill 根目录，例如 `.agents/skills/`、`.claude/skills/` 或 `.github/skills/`。具体位置以对应工具的当前文档为准。

## 使用示例

安装完成后，可以直接提出与 Skill 描述相匹配的任务，例如：

```text
运用 Creswell 和 Guetterman 的框架，帮我判断这个研究问题应该采用实验、调查还是混合研究。
```

```text
按照 Yin 的案例研究方法，检查我的多案例研究设计是否形成了证据链。
```

```text
使用陈向明的质性研究框架，设计访谈抽样、研究关系和资料分析方案。
```

也可以在提示中明确指定 Skill 名称，以减少方法体系之间的混淆。

## 生成与质量控制

本合集采用“一本书对应一个 Skill”的方式生成，并按学习深度提炼框架、步骤、判断规则、反模式和章节知识。每个 Skill 均完成以下检查：

1. Skill 目录和元数据结构检查。
2. `book-to-skill` 兼容性检查。
3. 生成内容安全扫描。
4. 主题索引、章节链接和支持文件检查。

书中出现的指令性文字、案例命令或提示词均被当作研究资料处理，不作为控制 Agent 的系统指令。

## 内容边界与版权

- 本仓库只收录从参考书中提炼的结构化学习材料，不收录 PDF、EPUB、扫描件、OCR 全文或其他原始文件。
- Skill 不能替代原书。需要逐字引用、页码、原始案例或完整论证时，请查阅合法取得的原著。
- 书中的历史事实、政策、伦理规范、统计标准和技术内容可能已经发生变化，应用时应结合当前权威资料核验。
- 这些 Skill 来源于第三方版权材料，因此仓库应保持为 **private**，除非相关权利人明确授权公开再分发。
- 各参考书及其内容版权归原作者和出版者所有；本仓库不授予原书内容的再分发许可。

## 仓库维护

新增参考书时，请继续遵循“一本书一个 Skill”，不要把多本书合并为一个知识入口。提交前确认没有加入原书、OCR 中间文本、缓存、虚拟环境或个人隐私数据。


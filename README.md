# Combinatorial Taste

**中文 / English · v0.1.1 · A Codex Skill for reference-driven website design**

## 中文

把你喜欢的网站参考，转化为适合自己业务、有自身辨识度的页面。

`combinatorial-taste-skill` 的核心是**有约束的排列组合**：观察参考中的设计关系，判断哪些方法兼容，再用统一的视觉规范和实际内容重新构成页面。它适合能辨认好看网站、但需要帮助把参考落实为自己页面的用户。

初版主要覆盖**品牌首页、产品落地页、个人作品集首页**，支持设计方案、页面改造和可运行实现。复杂后台、完整电商系统和多页面产品超出主要范围。

你可以提供一份或多份**网页截图、可访问的网址、录屏**，并说明网站用途、受众、首要目标、已有内容和品牌素材，以及技术栈和交付限制。一份可读参考就足够；多份参考也不必全部出现在成品里。

工作流程：

1. **实际查看参考。** 查看渲染页面、图片或可读取的录屏片段，区分观察事实与设计推断；看不到的区域、动效和响应式行为保持未知。
2. **围绕业务组合。** 内部比较两到三个有明确差异的候选方向，选择适合用户目标且彼此兼容的方法。
3. **统一并重构。** 建立具体的颜色、字体、间距、布局和组件 tokens，用实际内容检验。借鉴对齐、分组、层级等方法，不复制参考标志、文案、专有图片或具有鲜明识别性的整套构图。
4. **检查并交付。** 在工具允许时查看实际渲染结果、检查主要操作并修正问题，说明已验证范围和剩余限制。代码检查不能代替视觉验收。

方案请求交付可执行的结构、内容安排和视觉规范；实现请求继续交付可运行页面及使用方式。缺失文案可写明确标记的草案，不编造客户、指标或背书。设计请求本身不包含发布或部署。

## English

Turn websites you admire into a page that fits your business and has an identity of its own.

`combinatorial-taste-skill` uses **constrained composition**: inspect design relationships, decide which methods work together, and rebuild the page through a coherent visual language and real content. It is for people who recognize good design but need help making it their own.

The initial scope covers **brand homepages, product landing pages, and personal portfolio homepages**, including proposals, redesigns, and runnable implementations. Complex dashboards, complete ecommerce systems, and full multipage products are outside the primary scope.

Provide one or more **screenshots, accessible website URLs, or screen recordings**, together with your purpose, audience, primary goal, content, brand assets, and any stack or delivery constraints. One readable reference is enough. Multiple references are analyzed, but only suitable methods are retained.

The workflow inspects the actual rendered references, separates observations from inferences, and leaves unseen behavior unknown. It compares two or three directions internally, selects compatible methods around your business goal, then defines concrete design tokens for color, typography, spacing, layout, and components. Real content tests the result. It transfers methods such as alignment, grouping, and hierarchy without copying logos, proprietary images, copywriting, or a distinctive complete composition.

A proposal includes an actionable page structure and visual specification. An implementation also includes a runnable page and usage instructions. When tools permit, the rendered output and necessary interactions are checked and repaired; delivery states what was verified and what remains unverified. Code checks alone do not establish visual acceptance. Missing copy may be drafted and labeled, but clients, metrics, and endorsements are never invented. Publishing and deployment are separate actions.

## 安装 / Install

在支持此目录的 Codex 版本中，克隆到个人技能目录；其他平台使用其支持的个人技能位置。 / On Codex versions that support this directory, clone into your personal skills directory; otherwise use your platform's supported personal skills location.

```sh
mkdir -p ~/.agents/skills
git clone https://github.com/Chrischou920-spec/combinatorial-taste-skill.git ~/.agents/skills/combinatorial-taste-skill
```

目标目录已存在时，`git clone` 会停止，不覆盖已有 Skill。 / If the destination already exists, `git clone` stops without overwriting your existing Skill.

## 调用 / Use

```text
$combinatorial-taste-skill
参考我附上的截图，为我的咨询工作室设计并实现中文首页。
受众是小团队负责人，首要目标是预约初次沟通。
使用我提供的品牌素材和内容，交付可在本地运行的页面。
```

```text
$combinatorial-taste-skill
Use the attached screenshots to design and implement an English homepage
for my consulting studio. The audience is small-team leaders; the primary
goal is booking an introductory conversation. Use my supplied assets and
content, and deliver a page that runs locally.
```

符合范围的自然语言请求也可触发；输入与输出语言遵循用户要求。 / Matching natural-language requests can also activate the Skill. Input and output language follow your request.

## 文档与规则 / Documentation and rules

The [Skill entry point / 中文入口](SKILL.md) defines the workflow. The [English guide](README.en.md) provides detailed usage and limits. Read the relevant language path; these documents describe one Skill.

| 规则 / Rules | 中文 | English |
| --- | --- | --- |
| 参考分析 / Reference analysis | [原版](references/analysis-template.md) | [English](references/en/analysis-template.md) |
| 组合方法 / Composition | [原版](references/composition-rules.md) | [English](references/en/composition-rules.md) |
| 视觉规范 / Design tokens | [原版](references/design-tokens.md) | [English](references/en/design-tokens.md) |
| 检查与验收 / Review | [原版](references/review-rubric.md) | [English](references/en/review-rubric.md) |

See also the [English workflow](references/en/workflow.md). Verification reports describe the work actually checked; they are not certification or promises of future error-free output.

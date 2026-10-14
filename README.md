# Combinatorial Taste

**Chris 原创的 Taste Skill · A Taste Skill created by Chris**

一句话：一个 Codex Skill，从你喜欢的网页参考中提炼兼容的设计方法，为你的业务设计或实现有自身辨识度的首页。

In one sentence: a Codex Skill that combines compatible methods from website references to design or implement a distinctive homepage for your business.

## ✨ 功能 / Features

- **查看参考 / Inspect references**：分析一份或多份网页截图、可访问的网址或录屏；区分实际观察与推断。Analyze one or more screenshots, accessible URLs, or recordings, separating observations from inferences.
- **组合与重构 / Compose and rebuild**：围绕业务目标选择兼容的方法，统一颜色、字体、间距与组件规范，用真实内容重建页面。Choose compatible methods around the business goal, define consistent design tokens, and rebuild the page with real content.
- **方案与实现 / Proposals and implementation**：支持品牌首页、产品落地页、个人作品集首页的设计、改造或可运行实现。Create proposals, redesigns, or runnable implementations for brand, product, and portfolio homepages.
- **检查与交付 / Review and delivery**：工具允许时查看渲染结果、检查主要操作，说明已验证范围和剩余限制。Inspect rendered output and key interactions when tools permit, and report what was verified and what remains unverified.

## 🛠 技术栈 / Stack

- **Markdown**：`SKILL.md` 入口与设计规则文档。Skill entry point and design rules.
- **YAML**：`agents/openai.yaml` 配置显示名称、默认提示词和隐式调用。Display name, default prompt, and implicit invocation settings.
- **Codex**：读取 Skill 并执行设计工作流；当前版本没有可执行 helper。Runs the Skill workflow; this version contains no executable helper.

## 🚀 快速开始 / Quick start

将仓库安装到 Codex 的个人技能目录。以下路径适用于支持 `~/.agents/skills` 的版本；其他平台使用其支持的技能目录。

Install into Codex's personal skills directory. The commands below apply to versions supporting `~/.agents/skills`; otherwise use your platform's supported skills location.

```bash
mkdir -p ~/.agents/skills
git clone https://github.com/Chrischou920-spec/combinatorial-taste-skill.git ~/.agents/skills/combinatorial-taste-skill
```

目标目录已存在时，`git clone` 会停止，不覆盖已有 Skill。If the destination exists, `git clone` stops without overwriting your existing Skill.

在 Codex 中附上参考和业务背景，然后调用：Attach your references and business context in Codex, then invoke:

```text
$combinatorial-taste-skill
参考附上的截图，为我的项目设计并实现中文首页。
受众是独立开发者，主要目标是让访客查看项目演示。
使用我提供的内容与素材，交付可在本地运行的页面。
```

```text
$combinatorial-taste-skill
Use the attached screenshots to design and implement an English homepage
for my project. The audience is independent builders; the main goal is
opening the project demo. Use my supplied content and assets, and deliver
a page that runs locally.
```

符合范围的自然语言请求也可触发；输入和输出语言遵循你的要求。Matching natural-language requests can also activate the Skill; input and output follow your requested language.

## 📖 文档与边界 / Docs and scope

- [Skill 入口 / Skill entry point](SKILL.md)
- [详细英语说明 / Detailed English guide](README.en.md)
- [中文组合规则 / Composition rules in Chinese](references/composition-rules.md) · [English](references/en/composition-rules.md)
- [中文验收规则 / Review rules in Chinese](references/review-rubric.md) · [English](references/en/review-rubric.md)

当前版本 **0.1.1** 主要面向首页，复杂后台、完整电商系统和多页面产品超出主要范围。设计请求本身不包含发布或部署。

Version **0.1.1** focuses on homepages. Complex dashboards, complete ecommerce systems, and full multipage products are outside the primary scope. Design requests do not include publishing or deployment.

借鉴设计关系，不复制参考标志、文案、专有图片或整套标志性构图；不编造客户、指标或背书。代码检查不能代替视觉验收，未检查的行为保持未验证。

Transfer design relationships without copying logos, copywriting, proprietary images, or distinctive complete compositions. Do not invent clients, metrics, or endorsements. Code checks do not establish visual acceptance; unchecked behavior remains unverified.

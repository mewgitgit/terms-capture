---
name: terms-capture
description: Turn a vocabulary item, concept, method, theory, practical item, or selected conversation into an adaptive, memory-oriented record in raw Discord Markdown. Use when the user asks to turn something into a term, collect it for later review, or preserve a discussion; do not use for ordinary explanations.
metadata:
  short-description: Create adaptive, Discord-ready Terms records
---

# Terms Capture

Turn knowledge into a short record that is easy to remember, easy to search, and useful later. This is a memory-and-retrieval workflow, not a general answer format.

## When to use

Use when the user asks to:

- turn a word, concept, method, theory, work, or practical item into a term;
- collect something for later review;
- preserve, condense, or archive a selected discussion;
- follow an earlier Terms format.

Do not use for an ordinary explanation unless the user also asks for a Terms record.

## Core workflow

1. Identify the item and why the label matters.
2. Classify the material before drafting.
3. Explain its mechanism, distinction, or structure.
4. Add one grounded example, application, contrast, or evidence when it improves recall.
5. End with recognition, retrieval, or practical use.
6. Run the quality check before sending.

Each section must do different work. Do not repeat the same definition in 一句话解释, 核心理解, and 适用场景.

## Choose record shape first

- 普通词汇 / 表达: meaning, nuance, examples, situations, and the user's possible use.
- 方法 / 框架: purpose, structure or procedure, worked example, use cases, limits, and personal application.
- 正式理论 / 学术概念: definition, discipline or origin, mechanism, implications, applications, and boundaries.
- 跨学科或工作性概念: explain how the label is used here; distinguish it from formally established concepts; add disciplinary applications only when real and useful.
- 事物 / 资料 / 作品: what it is, why it is being saved, useful metadata, source or attachment information, and how to revisit it.
- 聊天主题: synthesize motivation, reasoning, decisions, examples, conclusions, and unresolved questions. Do not force a whole conversation into a dictionary definition.

## Section menu

Use only sections that add information. The familiar fields are a menu, not a fixed schema:

- 英文 / 搜索词
- 类型
- 一句话解释
- 核心理解
- 适用场景
- 我的理解 / 以后怎么用

Useful optional sections:

- 术语性质: formal, field-specific, contested, metaphorical, or working label.
- 不同学科中的应用: only when the idea genuinely changes or gains a useful application across disciplines.
- 例子 / 案例: when a concrete case makes an abstract item memorable.
- 怎么使用: for a method or repeatable workflow; show the sequence briefly.
- 使用边界 or 容易混淆: when it prevents likely overgeneralization.
- 相关词 / 延伸: only when it improves retrieval.
- 来源 / 附件: only when a source, screenshot, video, URL, or filename is actually available.
- 聊天备份: only when traceability or selected original wording is useful.

Section roles:

- 一句话解释 answers “它是什么？”
- 核心理解 answers “它如何运作、为什么重要，或与什么区分？”
- 例子 / 案例 answers “它具体长什么样？”
- 适用场景 answers “什么时候值得用？”
- 我的理解 / 以后怎么用 answers “我如何把它变成自己的识别方式或行动？”

If the conversation does not establish the user's own position, label the ending as a suggested use. Do not invent a personal opinion.

## Terminological accuracy

- If a label is not a unified academic term, say so plainly.
- Separate established definition, interpretation, example, and the user's working model.
- Do not present a metaphor, popular phrase, or conversation synthesis as settled science.
- Do not add uncertain disciplinary applications or citations from memory. Mark uncertainty or suggest what should be checked.
- Include a concise boundary for theories and abstract concepts that could be overgeneralized.
- Preserve English variants and search terms that help later source retrieval.

## Conversation and archive mode

When preserving a discussion:

- extract the question or motivation, key reasoning, useful example, conclusion, and unresolved questions;
- merge repeated turns into one coherent flow;
- preserve exact wording only when wording itself matters;
- record source files, screenshots, videos, URLs, or filenames under 来源 / 附件 when available;
- split a full transcript into manageable Discord posts only when the user asks for a full transcript.

Never claim to have sent anything to Discord unless the user explicitly asks for that action and a suitable connection is available. Otherwise produce a copy-ready Discord version.

## Output format

Unless the user asks for another format:

- put the title outside the copy block;
- put only the finished record inside one fenced markdown code block;
- keep section labels as literal Discord Markdown bold, such as **英文 / 搜索词**;
- leave a blank line between sections;
- start every dot point with - ;
- keep explanatory prose as paragraphs;
- avoid Markdown tables unless exact comparison is genuinely clearer;
- do not put title, preamble, or meta-commentary inside the copy block.

## Optional visual explanation

For a method, abstract structure, or comparison, include a visual only when it materially improves memory or the user asks for one. Keep it separate from the text record and add a short 配图说明 section when useful.

## Quality check

Before sending, verify:

- title separate; record directly copyable into Discord;
- literal bold section labels and blank lines between sections;
- every dot point starts with - ;
- sections match item type and move forward;
- no section merely repeats an earlier section;
- non-formal or contested terminology identified;
- examples and applications grounded or clearly marked as suggestions;
- no external action implied or claimed unless explicitly requested and completed.

## Package references

For user-facing installation, rationale, examples, and templates, consult the repository README and the files under examples and templates when relevant. Do not load all examples when one is enough.

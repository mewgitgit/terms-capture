# Terms Capture

An adaptive Codex skill for turning concepts, methods, theories, practical items, and selected conversations into searchable, memory-oriented records that can be pasted into Discord.

## Project status

- Project type: reusable Codex skill
- Output target: copy-ready Discord Markdown
- Structure: adaptive records, examples, templates, source traceability
- Repository: public GitHub project

## Overview

Terms Capture sits between a glossary and a personal knowledge archive. It does not save every sentence or force every topic into one rigid card. It selects a record shape based on the material, then connects the label, mechanism, example, boundary, and future use.

The core question is not only “What does this mean?” It is also:

- Why does this label matter?
- How does the idea work or differ from nearby ideas?
- What does it look like in practice?
- How will the user recognize, search, or use it later?

## Inspiration

The skill was designed around a recurring problem in chat-based learning and research:

- dictionary notes preserve definitions but lose the user's reason for caring;
- full transcripts preserve context but make later retrieval slow;
- rigid templates create empty sections or repeat the same definition;
- polished explanations can quietly turn a working label or interpretation into a false established fact.

Terms Capture responds with adaptive capture: classify the material, preserve only the useful reasoning structure, separate established meaning from interpretation, and end with a retrieval or action cue.

## Goals

- Make records easier to remember and retrieve.
- Preserve the user's reasoning rather than only a generic definition.
- Keep formal concepts, methods, works, sources, and conversations structurally distinct.
- Support English search variants and later source retrieval.
- Produce a finished Discord-ready record without claiming that it was posted.
- Mark uncertain, contested, metaphorical, or cross-disciplinary terminology.

## Non-goals

- It is not a general answer style.
- It is not a full transcript exporter unless requested.
- It is not an automatic Discord sender.
- It is not a citation generator or a substitute for source verification.
- It does not require every available section in every record.

## Features

### Adaptive record shapes

- Ordinary vocabulary: meaning, nuance, examples, situations, and personal use.
- Method or framework: purpose, procedure, worked example, use cases, limits, and application.
- Formal theory or academic concept: definition, discipline, mechanism, implications, and boundary.
- Cross-disciplinary working concept: local meaning, terminological status, distinction, and useful application.
- Thing, work, or source: identity, save reason, metadata, source, and revisit path.
- Conversation topic: motivation, reasoning, decisions, examples, conclusion, and open questions.

### Retrieval-oriented writing

Records can include English variants, search terms, related words, source filenames, and recognition cues. These details give the future reader more than one way back to the idea.

### Evidence and terminology discipline

The workflow separates established definition, interpretation, example, and the user's working model. It identifies non-formal labels instead of presenting them as settled academic terminology.

### Discord-ready output

By default, the title stays outside one finished markdown code block. The body uses literal bold section labels, blank lines, and hyphen bullets so it can be copied directly into Discord.

## How it works

1. Identify the item and why it matters.
2. Classify the material before drafting.
3. Choose only sections that add information.
4. Explain the mechanism, distinction, or structure.
5. Add one grounded example, application, contrast, or source when useful.
6. Mark boundaries, uncertainty, or likely confusion.
7. End with recognition, retrieval, or practical use.
8. Check format, duplication, terminology status, and external-action claims.

## How to use in Codex

### Explicit invocation

    $terms-capture Turn construct validity into a reviewable Terms record.

    $terms-capture Preserve the discussion about AI-mediated art interpretation. Keep the central disagreement and unresolved questions.

    $terms-capture Collect this method in the previous format. Add one concrete example and one usage boundary.

### Natural-language invocation

The skill applies when the request clearly asks to:

- turn a word, concept, method, or conversation into a term;
- collect something for later review;
- follow a previous Terms format;
- preserve or condense a useful discussion;
- make a Discord-ready record.

### Better input

The result improves when the request includes:

- the term and English variants;
- the source paragraph, screenshot, URL, or filename;
- why the user encountered it;
- the user's interpretation or uncertainty;
- the intended use: study, research, writing, project work, or archive.

## Output contract

The default result contains:

- title outside the copy block;
- one finished Discord Markdown code block;
- literal bold section labels;
- blank lines between sections;
- hyphen bullets only;
- sections chosen for the material rather than filled mechanically.

The record is copy-ready. It must not imply that it was sent to Discord unless the user explicitly requested that external action and it was completed.

## Examples and templates

Examples:

- examples/formal-concept.md — formal academic concept.
- examples/method.md — repeatable method.
- examples/cross-disciplinary.md — working label across fields.
- examples/conversation-archive.md — selected discussion preserved as a coherent record.

Templates:

- templates/concept.md — compact concept or theory record.
- templates/method.md — method or framework record.
- templates/chat-archive.md — selected conversation archive.

Templates are starting points, not mandatory schemas. The skill may remove, merge, or add sections.

## Intended outcomes

When used with accurate source material and a clear user context, the skill is intended to produce:

- faster later recognition of a concept;
- better recall through mechanism, contrast, example, and application;
- clearer separation between fact, interpretation, and personal synthesis;
- more useful search terms for future reading;
- less transcript noise;
- stronger connection between understanding and action.

These are intended workflow benefits, not measured guarantees. The skill does not claim to improve memory, grades, research quality, or decision quality in every case. Those outcomes depend on source accuracy, user engagement, later review, and the quality of the captured context.

## Limitations and risks

- A concise record can omit nuance if the source discussion is too thin.
- A working label may remain unsettled even after careful explanation.
- The skill can preserve an incorrect premise unless the source is checked.
- User context can be misread when the request does not state the intended use.
- Search terms can improve retrieval but cannot replace reading primary sources.
- Discord formatting is copy-ready, not a guarantee of perfect rendering in every client.
- A source, URL, screenshot, or citation is recorded only when actually available.

For high-stakes academic, legal, medical, financial, or technical claims, verify the underlying source separately.

## Design rationale

### Memory

Definition alone gives one retrieval path. Mechanism, contrast, concrete case, and future use create several paths back to the idea.

### Agency

The final section asks how the user will recognize or use the item. The record remains personal knowledge, not detached reference data.

### Accuracy

Terminological status and uncertainty are visible. A conversation synthesis does not silently become a formal theory.

### Adaptability

Different material needs different structure. A method needs sequence; a theory needs a boundary; a conversation needs reasoning and open questions.

### Traceability

Real files, URLs, screenshots, and source information can be retained without inventing metadata.

## Installation

For a local Codex installation, place this folder under the user's Codex skills directory:

    C:\Users\<user>\.codex\skills\terms-capture

Keep SKILL.md as the required entry point. The agents/openai.yaml file supplies optional UI metadata and keeps implicit invocation enabled.

## Maintenance

Keep the entry skill focused on decisions that affect output quality. Put substantial examples and templates in their own folders. When a failure appears, fix the narrow rule that caused it instead of adding a universal rule for every case.

For future GitHub project releases, use the same mature documentation order:

project status, overview, inspiration, goals, concrete outcomes, usage, examples, limitations, maintenance, English introduction first, then a complete Chinese version.

---

# 中文说明

## 项目状态

- 项目类型：可复用 Codex skill
- 输出目标：可直接复制到 Discord 的 Markdown 记录
- 结构：自适应记录、案例、模板、来源追踪
- 仓库策略：当前为公开 GitHub 项目

## 项目简介

Terms Capture 位于词汇表和个人知识库之间。它不会保存每一句聊天，也不会把所有主题强行塞进同一张固定卡片。它会先判断材料类型，再把术语、机制、例子、边界和未来用法连接起来。

核心问题不只是“它是什么意思”，还包括：

- 为什么这个标签值得保存？
- 它如何运作？和相近概念有什么区别？
- 它在实际情境里是什么样子？
- 以后如何识别、搜索或使用它？

## 项目启发

这个 skill 针对聊天式学习和研究中的几个常见问题：

- 字典式笔记保留定义，却丢失用户为什么在乎这个概念；
- 完整聊天记录保留上下文，却让之后检索变慢；
- 僵硬模板产生空栏目，或重复同一个定义；
- 语言很完整的解释，可能把工作性标签、个人解释误写成已经确立的学术事实。

Terms Capture 的解决方式是自适应收录：先判断材料类型，只保留有用的推理结构，把已确立的含义和解释分开，最后给出检索提示或行动提示。

## 项目目标

- 让记录更容易记忆和检索。
- 保留用户自己的推理，不只保存通用定义。
- 区分正式概念、方法、作品、资料和聊天主题。
- 保留英文变体和之后查资料有用的搜索词。
- 生成可以直接复制到 Discord 的完整记录，但不声称已经发送。
- 标出非正式、有争议、隐喻性或跨学科的术语。

## 非目标

- 不是普通回答的统一格式。
- 不是默认导出完整聊天记录的工具。
- 不是自动发送 Discord 消息的工具。
- 不是引用生成器，也不能替代来源核查。
- 不要求每条记录都填满所有栏目。

## 主要功能

### 自适应记录类型

- 普通词汇：含义、语气、例子、使用情境和个人用法。
- 方法或框架：目的、步骤、操作例子、适用场景、边界和应用。
- 正式理论或学术概念：定义、学科背景、机制、影响和边界。
- 跨学科工作性概念：本次对话中的含义、术语性质、区别和有用应用。
- 事物、作品或资料：身份、保存原因、元数据、来源和之后如何回看。
- 聊天主题：动机、推理、决定、例子、结论和未解决问题。

### 面向检索的写法

记录可以包含英文变体、搜索词、相关词、来源文件名和识别提示，让未来不只通过一种方式找回这个概念。

### 证据和术语纪律

工作流程区分已确立定义、解释、例子和用户自己的工作模型。遇到非正式标签，会明确说明其性质，不把它直接写成已经确立的学术术语。

### Discord-ready 输出

默认把标题放在代码块外，正文放在一个完成的 Markdown 代码块中。栏目使用字面加粗、空行和短横线列表，方便直接复制到 Discord。

## 工作流程

1. 确认要保存什么，以及为什么重要。
2. 写作前先判断材料类型。
3. 只选择真正增加信息的栏目。
4. 解释机制、区别或结构。
5. 在有帮助时加入真实例子、应用、对比或来源。
6. 标出边界、不确定性或容易混淆之处。
7. 用识别、检索或实际使用方式收尾。
8. 检查格式、重复、术语性质和外部行动声明。

## 在 Codex 中使用

### 显式调用

    $terms-capture 把 construct validity 变成一个可复习的 Terms record。

    $terms-capture 保存刚才关于 AI-mediated art interpretation 的讨论，保留核心争议和未解决问题。

    $terms-capture 按之前格式收录这个方法，加一个具体例子和使用边界。

### 自然语言调用

以下请求通常会触发：

- 把词、概念、方法或聊天变成 term；
- 收录内容，之后方便复习；
- 按之前的 Terms 格式整理；
- 保存或压缩一段有用讨论；
- 生成 Discord-ready 术语记录。

### 更好的输入

如果能提供以下信息，结果会更准确：

- 术语和英文变体；
- 来源段落、截图、URL 或文件名；
- 为什么遇到它；
- 自己的理解或不确定之处；
- 使用目的：学习、研究、写作、项目工作或聊天备份。

## 输出约定

默认输出包含：

- 标题在复制区块外；
- 一个完成的 Discord Markdown 代码块；
- 字面形式的加粗栏目标题；
- 栏目之间留空行；
- 只使用短横线列表；
- 根据材料选择栏目，不机械填表。

记录可以直接复制使用，但不能暗示已经发送到 Discord，除非用户明确要求外部发送并且确实完成。

## 案例和模板

案例：

- examples/formal-concept.md：正式学术概念。
- examples/method.md：可重复使用的方法。
- examples/cross-disciplinary.md：跨学科工作性标签。
- examples/conversation-archive.md：把选定讨论整理成连贯记录。

模板：

- templates/concept.md：概念或理论记录。
- templates/method.md：方法或框架记录。
- templates/chat-archive.md：聊天主题备份。

模板只是起点，不是强制 schema。skill 可以删除、合并或新增栏目。

## 预期成果

当来源材料准确、用户情境清楚时，这个 skill 预期带来：

- 之后更快认出一个概念；
- 通过机制、对比、例子和应用增强回忆；
- 更清楚地区分事实、解释和个人综合；
- 为之后查资料留下更好搜索词；
- 减少聊天记录噪音；
- 把理解连接到之后的行动。

这些是工作流层面的预期收益，不是经过统一测量的保证。它不能保证记忆、成绩、研究质量或决策质量一定提升；结果仍取决于来源准确性、用户参与、之后复习和被保存内容的质量。

## 限制和风险

- 来源讨论太少时，简短记录可能遗漏重要细节。
- 工作性标签即使经过解释，也可能仍未形成统一定义。
- 如果没有核查来源，skill 可能保留错误前提。
- 请求没有说明用途时，用户情境可能被误读。
- 搜索词能改善检索，但不能替代阅读一手来源。
- Discord-ready 只表示方便复制，不保证每个客户端都完全一致渲染。
- 只有真实存在的来源、URL、截图或引用才会被记录。

涉及高风险学术、法律、医疗、财务或技术判断时，仍需单独核查基础来源。

## 设计理由

### 记忆

只有定义时，回忆入口很少。加入机制、对比、具体案例和未来用法后，找回概念的路径更多。

### 主体性

最后一栏要求说明以后如何识别或使用它。记录不是脱离用户的资料，而是个人知识的一部分。

### 准确性

术语性质和不确定性显式保留。聊天中的综合不会悄悄变成正式理论。

### 自适应

不同材料需要不同结构：方法需要步骤，理论需要边界，聊天需要推理和未决问题。

### 可追踪

真实文件、URL、截图和来源信息可以保留下来，但不会凭空补造元数据。

## 安装

本地 Codex 安装时，把整个文件夹放到用户级 skill 目录：

    C:\Users\<user>\.codex\skills\terms-capture

SKILL.md 是必需入口。agents/openai.yaml 提供可选 UI 信息，并保持隐式调用开启。

## 维护

让入口 skill 只保留会影响输出质量的判断规则。较长案例和模板放到独立文件夹。出现失败时，修正导致问题的窄规则，不要为每个案例添加一条普遍规则。

以后发布 GitHub 项目，统一采用成熟顺序：

项目状态、项目简介、项目启发、目标、具体成果、使用说明、案例、限制、维护；先完整英文介绍，再放完整中文版。

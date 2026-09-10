# Terms Capture

An adaptive Codex skill for turning concepts, methods, theories, practical items, and selected conversations into searchable, memory-oriented records that can be pasted into Discord.

## Why this exists

Most notes fail in one of two ways:

- they store a dictionary definition but not the user's way to recognize or use the idea;
- they preserve a conversation transcript but make later retrieval slow.

Terms Capture sits between a glossary and a personal knowledge archive. It keeps the label, mechanism, example, boundary, and future use connected. It also changes record shape according to the material, so a formal theory is not forced into a vocabulary card and a conversation is not flattened into a dictionary entry.

The point is not to save every sentence. The point is to preserve the smallest useful structure that lets a future reader answer:

- What is this?
- Why does the label matter?
- How does it work or differ from nearby ideas?
- What does it look like in practice?
- When should I recognize, search, or use it?

## What “Terms Capture” means

Terms Capture is a working name for a retrieval-oriented writing workflow. It is not a claim that all learning must use one fixed template. Its central idea is adaptive capture:

recognize the item, choose its shape, explain the mechanism, ground it in an example, mark its limits, and connect it to future action.

## Repository layout

- SKILL.md — instructions loaded by Codex when the skill applies.
- agents/openai.yaml — optional UI metadata and default invocation prompt.
- examples/ — finished records showing different material types.
- templates/ — lightweight starting structures. They are menus, not mandatory forms.

## How to use in Codex

### Explicit invocation

Use the skill name in the request:

> $terms-capture 把 construct validity 变成一个可复习的 Terms record。

> $terms-capture 把刚才关于 AI-mediated art interpretation 的讨论保存下来，保留核心争议和未解决问题。

> $terms-capture 按之前格式收录这个方法，并加一个实际例子和使用边界。

### Natural-language invocation

The skill also applies when the request clearly asks to:

- 把这个变成 term / terms；
- 按之前格式收录；
- 收录这个概念，之后方便搜索；
- 保存刚才聊天内容，之后复习；
- 做一个 Discord-ready 的术语记录。

### Give better input

Useful input includes:

- the term or phrase, including English variants;
- the source paragraph, screenshot, URL, or filename if available;
- why the user encountered it;
- the user's own interpretation or uncertainty;
- whether the goal is study, research, writing, project work, or conversation backup.

Example:

> $terms-capture 记录 “AI as experimental variable”。这是我在研究 AI 艺术中介 prototype 时使用的工作性概念。说明它和普通工具变量有什么区别，给出应用场景和边界。

### Expected output

By default, the result has:

- title outside the copy block;
- one finished Discord Markdown code block;
- literal bold section labels;
- blank lines between sections;
- hyphen bullets only;
- adaptive sections selected for the item type.

The result should be copy-ready, but it should not claim that it was posted to Discord.

## How the skill decides structure

| Material | Record emphasis |
| --- | --- |
| Ordinary word or phrase | meaning, nuance, example, situation, personal use |
| Method or framework | purpose, sequence, worked example, limits, application |
| Formal theory or academic concept | definition, mechanism, implications, boundary |
| Cross-disciplinary working concept | local meaning, status, distinction, useful application |
| Thing, work, or source | identity, save reason, metadata, source, revisit path |
| Conversation topic | motivation, reasoning, decisions, examples, conclusion, open questions |

This decision is editorial. It usually does not need to be shown in the answer.

## Examples

- examples/formal-concept.md — formal academic concept.
- examples/method.md — repeatable method.
- examples/cross-disciplinary.md — working label across fields.
- examples/conversation-archive.md — selected discussion preserved as a coherent record.

The examples are demonstrations, not facts to memorize. Replace their content with the user's context.

## Templates

- templates/concept.md — compact concept or theory record.
- templates/method.md — method or framework record.
- templates/chat-archive.md — selected conversation archive.

Start with a template only when it helps. The skill may remove, merge, or add sections.

## Design meaning

### Memory

Definition alone is weak retrieval. Mechanism, contrast, concrete case, and future use create more paths back to the idea.

### Agency

The user's own interpretation matters. The final section asks how the user will recognize or use the item instead of treating knowledge as detached reference data.

### Accuracy

The workflow separates established meaning from interpretation and working labels. This reduces the risk of turning a metaphor or personal synthesis into a false academic fact.

### Retrieval

English variants, search terms, related words, source filenames, and clear section roles make later search faster.

### Adaptability

Different objects need different records. A method needs a sequence. A theory needs a boundary. A conversation needs reasoning and open questions.

## What this skill is not

- not a general answer style;
- not a demand to create every section every time;
- not a full transcript exporter unless requested;
- not a citation generator;
- not an automatic Discord sender;
- not a replacement for source verification when accuracy matters.

## Maintenance

Keep SKILL.md focused on decisions Codex must make while producing a record. Put substantial examples and user-facing explanation in this README or the example/template folders. When a failure appears, fix the narrow rule that caused it instead of adding a universal rule for every possible case.

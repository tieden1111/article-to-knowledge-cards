---
name: make-knowledge-cards
description: Turn a user's pasted article or local Markdown/TXT file into 5-8 concise, source-grounded knowledge cards. Use when asked to extract and study the important ideas in supplied text. Do not use for webpage retrieval, PDFs, Anki decks, or graphical interfaces.
---

# Make Knowledge Cards

Convert supplied source text into a small set of accurate, useful study cards. Prefer fewer cards over repetition or unsupported filler.

## Workflow

1. **Read the source.** Accept text pasted in the conversation or a local `.md`/`.txt` file. For a file, use available file-reading tools to inspect its contents before summarizing; do not infer contents from its name. If it cannot be accessed or is not a supported format, say so and ask for pasted text or a supported file. Do not fetch webpages or attempt to process PDFs.
2. **Find candidate ideas.** Identify the source's central claims, principles, explanations, decisions, steps, or distinctions. Prioritize ideas that are important to understanding or applying the text, not incidental details.
3. **Consolidate.** Merge repeated statements and overlapping candidates. Keep meaningful qualifications, scope, uncertainty, and cause-and-effect relationships from the source. Exclude points that add no distinct learning value.
4. **Choose the count.** Produce 5-8 cards when the source supports that many distinct, worthwhile ideas. Use fewer if it does not; never split one idea into multiple cards, repeat a point, or add outside knowledge just to reach five. When there are more than eight candidates, keep the most central and useful ones.
5. **Draft and verify.** Give each card one knowledge point. Check every factual statement against the source, including the explanation and any example or question. Do not add facts, definitions, assumptions, examples, or conclusions absent from the source. If the source is ambiguous, preserve that ambiguity or state that the source does not specify.

## Output format

Start with a concise, source-appropriate heading. Then number the cards. Use this structure for every card:

### 1. [Short, specific title]
- **核心知识：** State the single key point in one clear sentence.
- **简明解释：** Explain that same point briefly, using only what the source supports.
- **例子或自测：** Give a source-supported example, or ask one focused self-test question answerable from the source.

Use a self-test question when the source provides no example. Do not invent a scenario and present it as a fact from the article. If a useful example or question cannot be made without adding unsupported information, say so briefly in this field rather than fabricating one.

Keep cards concise and distinct. Preserve technical terms that matter, explaining them only when the source does. Do not add a general introduction, unrelated advice, citations, or an answer key unless the user requests them.

## Scope

- Supported inputs: user-pasted article text and local Markdown (`.md`) or plain-text (`.txt`) files.
- Not supported: webpage fetching, PDF processing, Anki export, or building a graphical interface. Briefly clarify the limitation and offer a supported input route when asked for one of these.

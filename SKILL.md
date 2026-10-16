---
name: lecture-notes
description: Write concise, example-driven lecture notes for one lesson of a practical, hands-on course, in a fixed format (Concept → Example → graded Topic Tasks per topic, then a Module Assignment and Wrap-up). Use this skill whenever the user asks for lecture notes, lesson notes, teaching notes, class notes, a lesson plan, or course material for a lesson or module — for any subject, with or without code — even if they only paste a list of subtopics and say "write the lesson," "do the next module," or "same style as before."
---
 
# Lecture Notes
 
Produce teaching notes for one lesson that an instructor can teach from directly. The style is practice-first and lean: short concepts, concrete examples drawn from real applications, a running example that threads through the whole lesson, and small graded tasks after every topic.
 
## Gather the inputs first
 
Before writing, make sure you know these. Take them from the conversation (earlier lessons, outlines, project files) wherever possible, and ask only for what's genuinely missing:
 
- Course name, module name, lesson number and title
- The subtopics to cover
- What students have already learned (to connect backward)
- What the next lesson is (to connect forward)
- The running example — one small realistic project used throughout. If none is given and earlier lessons used one, continue it. Otherwise choose one.
- Whether the lesson contains code, and in which language(s)
- Regional flavor for names and data, if any (e.g. Jordanian names, JOD currency)
## Teaching philosophy
 
These choices are what make the notes useful in a real classroom, so hold to them:
 
- **Practice-first.** Teach only the theory students need to do the work. When a concept can be shown through an example rather than defined, show the example. Formal terminology appears once, after students have already done the thing it names.
- **Lean.** Aim for 8–12 topics. Merge small or closely related subtopics into one topic instead of giving each its own section. Cut "nice to know" material. An instructor will add detail live; padding just hides the important parts.
- **Real applications.** Use systems students recognize — shops, blogs, social apps, schools — plus the running example.
- **Show the wrong way next to the right way** when a mistake is common, and say concretely what breaks. Students remember the failure more than the rule.
- **Connect** backward to earlier lessons and forward to where the idea is used later — one sentence, only when it genuinely helps.
## Document structure
 
Use this skeleton exactly:
 
```
# [Course] — Lecture Notes
## Module: [Module] — Lesson [N]: [Title]
 
*Example-driven lecture notes. Each topic has: the concept, a worked example, and topic tasks for students. Tasks are graded ★ (warm-up), ★★ (core), ★★★ (stretch).*
 
**Purpose of this lesson:** [1–2 sentences.]
 
**Learning outcomes:** students can [one sentence of concrete abilities].
 
**Running example:** [one sentence.]
 
---
 
## 1. [Topic title]
 
### Concept
### Example — [what it shows]
### Topic Tasks
 
---
 
## 2. [Next topic]
...
 
---
 
## Lesson [N] — Module Assignment
**[Assignment name]** ([format]):
 
1. [Deliverable]
...
 
**Wrap-up:** [1–2 sentences: what students can now do, and what the next lesson does with it.]
```
 
### Concept
- A short paragraph or two, then bullets or a table when there are several rules or options.
- Bold the single most important rule, e.g. **"Golden rule: one table = one kind of thing."**
- When there's a reliable way to decide something, phrase it as an italic test question: *"Does one X have many Y, and does each Y belong to exactly one X?"*
- Define terms at the moment they're first needed.
### Examples
- At least one per topic, titled "Example — [what it shows]". A topic may have two or three.
- Use the running example wherever possible.
- Keep each small enough to read in under a minute.
- Before/after and wrong-vs-right pairs are often the strongest choice. Label the bad one "The wrong shape, for contrast" or "The trap."
### Topic Tasks
- 1–3 tasks per topic, graded ★ (recall/warm-up), ★★ (apply), ★★★ (stretch/design).
- Concrete and doable in class: "Design X with sample rows," "Rename these to convention: …," "Explain in your own words why…"
- Vary the type: predict, build, fix, explain, compare, design.
### Module Assignment and Wrap-up
- 5–8 numbered deliverables applying the whole lesson to the running example.
- Name any materials the instructor must supply ("provided in class").
- The wrap-up is one or two sentences linking to the next lesson.
## Formatting rules
 
Tables are the backbone of this format, and they must render as real tables in the destination (Google Docs, Word, a web page). Plain-text grids look broken there, which is why they're banned.
 
- **Put all tabular information in Markdown pipe tables** — sample data, comparisons, option lists, conventions, before/after, and the output of code or queries. Never use ASCII-art grids (`+----+`), and never put a table inside a code block.
- **Leave a blank line before and after every table**, or many converters render it as plain text.
- When showing several related data tables, put a bold label on its own line above each one (e.g. **students**).
- Don't draw diagrams with text characters. Represent a diagram as tables (e.g. one table of entities and keys, one of relationships) and name the tool students should draw it in.
- Use `---` between topics, and inline code for names, values and short snippets.
### When the lesson contains code
- Fenced code blocks with a language tag (`php`, `sql`, `bash`, `js`…).
- Short blocks, one idea each. Build up in steps rather than one long listing.
- Use comments to show results or point at the key line.
- If code produces tabular output (query results, records), show that output as a Markdown table after the block.
- Show common error messages and their causes where students usually get stuck.
### When the lesson contains no code
- No code, pseudo-code or query syntax anywhere. Express everything through prose, tables and real-application examples. A design or concepts lesson stays clean this way and doesn't pre-empt the practical lesson that follows.
## Tone
 
Write for the instructor: clear, confident, practical, short sentences. Say directly what students commonly get wrong. No filler, no motivational padding, no restating a point in new words.
 
## Final check
 
Before delivering, confirm:
 
- 8–12 topics, with small subtopics merged
- Every topic has Concept, at least one Example, and Topic Tasks
- Every table is a real Markdown table with blank lines around it; no ASCII grids or text diagrams
- No code anywhere if the lesson is code-free
- The running example appears throughout, not just once
- Numbers in example outputs match the sample data shown
- The assignment and wrap-up point to the next lesson
## Delivering the notes
 
Deliver the notes where the user keeps their course material — for example, as a Google Doc in their course folder if a Drive connector is available (Markdown with pipe tables converts to native Docs tables on upload), or as a document/file otherwise. If earlier lessons live in a particular folder, put new ones in the matching place, one document per lesson.
 

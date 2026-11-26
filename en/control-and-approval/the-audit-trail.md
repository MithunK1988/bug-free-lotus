---
title: The audit trail
internalDescription: What the commit history proves, what it does not, and how to read it.
tags:
  - control
  - git
labels:
  - sample-content
seo:
  title: The audit trail in a Git-backed documentation project
  description: Proving what a procedure said, and who changed it.
display:
  toc: true
  outline: true
---

## What the history gives you

[d360]: # 'table border="all" striped="true"'

| Question | Answered by |
| :--- | :--- |
| What did this procedure say on 3 March? | The repository at that date |
| Who changed this step, and when? | The commit that touched the line |
| Why was it changed? | The commit message, if somebody wrote one |
| Who approved it? | The approval on the change that merged it |
| Has anything been altered since? | The history itself |

[d360]: # "/table"

Reading one line's history is one command:

```bash
git log -p --follow docs/en/writing-procedures/the-shape-of-a-procedure.md
```

[d360]: # 'callout kind="success"'

> **"What did it say then" is the question auditors actually ask**
>
> Most document-control systems answer it with a stored PDF of each revision. Here it is the
> repository at a point in time, which is the same evidence without the filing.

[d360]: # "/callout"

## What it does not give you

> [!CAUTION]
> **A history is only evidence if nothing else can change the text**
>
> If anybody can push directly to the published branch, the trail records what happened without
> constraining it. Protect the branch, require approval on merges, and the history becomes proof
> rather than a log.

It also does not tell you whether a procedure was *followed*. That evidence lives in your records,
not in the documentation, and conflating the two is a common and expensive mistake.

## Writing commit messages worth reading

[d360]: # 'table border="all" striped="true"'

| Useful | Useless |
| :--- | :--- |
| `SOP-14: add pressure check before start` | `Update` |
| `Correct emergency number after site change` | `Fixes` |
| `Clarify step 6 after near-miss report NM-203` | `As discussed` |

[d360]: # "/table"

> [!IMPORTANT]
> **The message is the only part of the trail a machine cannot reconstruct**
>
> The diff shows what changed. Only the author can say why, and in a year that is the thing somebody
> will need.

## Showing it to somebody

[d360]: # 'pdf src="https://www.w3.org/WAI/ER/tests/xhtml/testfiles/resources/pdf/dummy.pdf" width="100%" height="420"'

[d360]: # "/pdf"

A one-page summary of what the repository can evidence, for the conversation with whoever owns
compliance — who will reasonably want to know before you move your procedures.

> [!TIP]
> **Have that conversation before the migration, not after**
>
> It usually goes well, and it goes much better when the answer to "can you show me what SOP-14 said
> last March" is demonstrated rather than promised.

[d360]: # 'snippet name="deleteMe"'

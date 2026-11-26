---
title: Your first change
internalDescription: Making, reviewing and approving one change, from the portal and from a clone.
tags:
  - control
  - getting-started
  - writer
labels:
  - sample-content
seo:
  title: Make your first change
  description: Edit a procedure and take it through approval.
display:
  toc: true
  outline: true
---

This page is sample content, so it is a safe thing to break.

## In the portal

[d360]: # 'multi-level-list styles="decimal,lower-alpha"'

1. Open the article in <span data-variable="editorName">{{variable.editorName}}</span>.
2. Change a sentence. Save keeps a draft; Save to branch commits it to the branch you are working on.
3. Send it for review.
4. Once it is approved and merged, publish.

[d360]: # "/multi-level-list"

## In a clone

```bash
git clone <your repository>
cd docs/en/start-here
$EDITOR your-first-change.md
git commit -am "SOP: clarify the first step"
git push
```

Both routes write the same file. That is what makes a mixed team workable — a writer in the portal
and an engineer in Vim are editing the same procedure.

> [!IMPORTANT]
> **Saving is not approving, and approving is not publishing**
>
> Three separate events, deliberately. In a controlled document each of them is a different person's
> responsibility, and collapsing them is how unapproved text reaches the floor.

## Read the diff

```diff
-Check the pressure gauge before starting the pump.
+Check the pressure gauge before starting the pump. If it reads above 4 bar, stop and call the duty engineer.
```

One sentence added, one line in the diff. A reviewer sees exactly what changed — which, on a
procedure somebody follows under time pressure, is the only kind of review worth having.

> [!CAUTION]
> **Turn off automatic reflowing for this repository**
>
> An editor that re-wraps paragraphs on save turns a one-word fix into a whole-file diff, and a
> reviewer who cannot see what changed will approve it anyway.

[d360]: # 'video src="https://commondatastorage.googleapis.com/gtv-videos-bucket/sample/ForBiggerEscapes.mp4" width="720" height="405" controls="true"'

[d360]: # "/video"

[d360]: # 'divider style="dashed"'

---

## Four things worth trying

- [ ] Change a sentence and look at the diff.
- [ ] Find this file's history and read one earlier version.
- [ ] Ask somebody to review it, and have them send it back.
- [ ] Delete this article. It is sample content.

[d360]: # 'callout kind="success"'

> **Have your first review rejected on purpose**
>
> A team that has never seen the changes-requested path does not know its own process. Find out on
> sample content rather than on a procedure somebody is waiting for.

[d360]: # "/callout"

[d360]: # 'snippet name="deleteMe"'

---
title: Change notification
internalDescription: Telling people a procedure changed, and the difference between publishing and informing.
tags:
  - control
  - procedures
labels:
  - sample-content
seo:
  title: Telling people a procedure changed
  description: Publishing is not notification, and the gap between them is where accidents live.
display:
  toc: true
  outline: true
---

Publishing makes the new text available. It does not reach the person who learned the old version in
training and has had no reason to look since.

## Which changes need telling

[d360]: # 'table border="all" striped="true"'

| Change | Tell people? |
| :--- | :--- |
| A step added, removed or reordered | Yes, before it takes effect |
| A limit, figure or contact changed | Yes |
| A warning added | Yes, and say why |
| Wording clarified, same actions | A note is enough |
| A typo | No |

[d360]: # "/table"

> [!IMPORTANT]
> **Decide this when you write the change, not when you publish it**
>
> By publishing time the author has moved on and the question gets answered by whoever is around.
> Make it part of the review: does this need telling, and who tells them?

## What the repository gives you to work with

[d360]: # "tabs"

<details>
<summary>The diff</summary>

The exact change, in a form you can paste into whatever you send. A notification that shows the old
and new text is far more use than one saying a procedure was updated.

</details>

<details>
<summary>The commit message</summary>

Why it changed, if somebody wrote it properly. This is usually the sentence your notification needs
and the reason commit messages are worth insisting on.

</details>

<details>
<summary>The history</summary>

When it changed and who approved it, which is what somebody will ask when they question whether they
were told.

</details>

[d360]: # "/tabs"

> [!CAUTION]
> **Do not notify on everything**
>
> A team that gets a message for every typo stops reading the messages, and the one about the new
> isolation step arrives in a stream they have learned to ignore.

## Acknowledgement

If somebody must confirm they have read a change, that record belongs in whatever system tracks
training and competence. Documentation can tell you what changed and when; it cannot tell you who
read it.

> [!NOTE]
> **Keep the two systems separate and link them**
>
> Trying to make the documentation project hold read receipts ends with a worse version of a training
> system. The documentation's job is to be the authoritative text and to show when it changed.

[d360]: # 'snippet name="deleteMe"'

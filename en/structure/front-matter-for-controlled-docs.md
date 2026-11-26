---
title: Front matter for controlled documents
internalDescription: The fields at the top of a file, which ones matter here, and the write-only-what-differs rule.
tags:
  - control
  - structure
labels:
  - sample-content
seo:
  title: Front matter in a Document360 Lotus project
  description: The fields at the top of each file and what they do.
display:
  toc: true
  outline: true
---

Every article begins with a block of YAML. It holds the article's metadata, it is reviewed like the
prose, and on a controlled document some of it is part of the control.

## The fields that earn their place here

[d360]: # 'table border="all" striped="true"'

| Field | Why it matters on a procedure |
| :--- | :--- |
| `title` | What readers and search see |
| `internalDescription` | Why the page exists; not shown to readers |
| `tags` | How people find it — names, never ids |
| `labels` | Internal editorial state; never reaches the site |
| `status.expiresAt` | The review date |
| `seo` | How it appears in a search result |

[d360]: # "/table"

> [!IMPORTANT]
> **Tags and labels are written as names**
>
> An id is meaningless to anyone reading the repository and unresolvable in a review. The whole point
> of the content being files is that a person can read the change; ids undo that.

## Write only what differs

Boolean settings have stored defaults, and a value equal to the default is noise in every diff
forever. Leave it out.

> [!NOTE]
> **This page's own front matter follows that rule**
>
> It sets no booleans, because none of them differ from their defaults here. Worth checking on your
> own pages: a field written out at its default is a line reviewers learn to skip.

## What front matter is not

> [!CAUTION]
> **Do not put the approval in a custom field and consider it recorded**
>
> A name typed into YAML is text that anybody can change. The approval that counts is the one on the
> change that merged it, which nobody can edit afterwards. Front matter can *display* the approver;
> it cannot *be* the approval.

## Keeping it consistent

- [ ] Agree the field set for procedures, and write it down.
- [ ] Put it in the template rather than in people's memories.
- [ ] Check it automatically, because nobody enjoys reviewing YAML.

> [!TIP]
> **Front matter is the cheapest thing to validate and the most tedious to review**
>
> Unknown keys, a missing review date, a tag that does not exist — all detectable in a second, all
> invisible to a human reading for meaning.

[d360]: # 'snippet name="deleteMe"'

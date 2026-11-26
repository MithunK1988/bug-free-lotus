---
title: Reuse
internalDescription: Variables and snippets as files, what to reuse, and the glossary gap.
tags:
  - procedures
  - writer
labels:
  - sample-content
seo:
  title: Reusing content across procedures
  description: Variables and snippets in a Document360 Lotus project.
display:
  toc: true
  outline: true
---

In this product type the reusable things are files in `.document360/`, which means they are reviewed,
versioned and diffed like everything else.

## The two

[d360]: # 'table border="all" striped="true"'

| | Holds | Use for |
| :--- | :--- | :--- |
| **Variable** | A short string, inline | A site name, a role title, a document number prefix |
| **Snippet** | A block of content | A control block, a standing safety warning, a prerequisite |

[d360]: # "/table"

Both are referenced by name. Edit the file and every page using it changes, in one commit a reviewer
can read.

> [!IMPORTANT]
> **This is the argument for controlled documents in a repository, in one sentence**
>
> "Change the emergency contact on two hundred procedures" is one file, one diff, one approval and
> one timestamp — rather than two hundred edits nobody can prove were all made.

## What to reuse and what not to

[d360]: # 'table border="all" striped="true"'

| Reuse | Do not reuse |
| :--- | :--- |
| Things that must agree everywhere | Things that happen to match today |
| A control block | A paragraph two pages share by coincidence |
| A warning mandated by policy | A sentence you expect to tune per page |

[d360]: # "/table"

> [!CAUTION]
> **Before editing a shared snippet, find out what uses it**
>
> A one-word improvement is a one-word change on every page carrying it, including the procedures you
> have never read. Search the repository first; it is one command.

## The glossary

Glossary terms define a word once and show the definition where it appears. They are files like
everything else here: **one Markdown file per term**, in the workspace's glossary folder, named for
the term's slug. The term and its aliases are in front matter, the definition is in the body, and it
syncs both ways like a snippet does.

> [!IMPORTANT]
> **A definition is a controlled statement too**
>
> Once a glossary term is a file, changing what "competent person" means is a reviewed, approved,
> timestamped change like any other. That is a stronger position than most document-control systems
> manage, where the glossary is a page somebody edits.

> [!TIP]
> **A procedures project benefits from a glossary more than most**
>
> Controlled documents are full of words with precise, local meanings — "verify", "competent person",
> "shift". Defining them once beats defining them differently on four pages.

[d360]: # 'snippet name="deleteMe"'

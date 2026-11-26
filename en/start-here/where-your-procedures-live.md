---
title: Where your procedures live
internalDescription: The repository layout, what each file and folder is, and what not to touch.
tags:
  - getting-started
  - git
  - structure
labels:
  - sample-content
seo:
  title: The repository layout
  description: What is in the repository and what each part of it does.
display:
  toc: true
  outline: true
---

## The layout

Everything readers see sits under a documentation root — `docs/` in a default setup — with one folder
per language inside it. test

```text
docs/
└── en/
    ├── start-here/
    │   ├── README.md
    │   └── how-this-project-works.md
    └── writing-procedures/
        ├── README.md
        └── the-shape-of-a-procedure.md
```

A folder is a category. Its `README.md` is the category's own page. Every other `.md` file is an
article.

> [!IMPORTANT]
> **Folders do not decide the order readers see**
>
> `d360.json` does. The folder layout is storage; the manifest is navigation. They are allowed to
> disagree, and on a large manual they usually should.

## The parts that are not articles

[d360]: # 'table border="all" striped="true"'

| Path | Holds |
| :--- | :--- |
| `d360.json` | The navigation tree and the languages |
| `.document360/variables.json` | Short strings reused inline |
| `.document360/tags.json` | Tag groups and tags |
| `.document360/labels.json` | Label groups and labels |
| `.document360/snippets/global/` | Reusable blocks of content |

[d360]: # "/table"
[d360]: # 'figure align="center" width="820"'

![Storage on the left, the navigation readers see on the right, joined by the manifest](https://placehold.co/820x340/0f172a/c7d2fe/png?text=Folders++%E2%86%92++d360.json++%E2%86%92++Navigation){width="820" height="340"}

Folders hold the files. The manifest decides what readers get. Changing one does not change the
other, which is why renaming a folder is safe and reordering the manifest is not a file move.

[d360]: # "/figure"

## What to leave alone until you have read more

> [!CAUTION]
> **d360.json is the file where a careless edit is visible to readers**
>
> A node pointing at a file that is not there, or a file in no node, produces a navigation that is
> wrong in a way nothing announces. [Categories and the manifest](../structure/categories-and-the-manifest.md)
> covers it properly.

## Where everything else goes

Images, attachments and anything else a page references live in the repository too, beside the pages
that use them. A procedure and its diagram move together, which is what you want the day somebody
reorganises the manual.

> [!TIP]
> **Keep an asset next to the page that uses it, not in one shared folder**
>
> A single `images/` folder at the root is tidy on day one and unmaintainable by page two hundred,
> because nothing tells you which file is still in use.

[d360]: # 'snippet name="deleteMe"'

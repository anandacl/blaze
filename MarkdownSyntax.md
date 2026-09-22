---
description: "A reference for the Markdown syntax you can use across the Blaze docs."
icon: "hash"
---

## Headings

Use one to six `#` characters to set the heading level. Reserve `#` for the page
title and start your body content at `##` so the table of contents nests properly.

```markdown
# Page title
## Section
### Subsection
```

## Text formatting

| Effect | Syntax | Result |
| --- | --- | --- |
| Bold | `**important**` | **important** |
| Italic | `_subtle_` | _subtle_ |
| Strikethrough | `~~removed~~` | ~~removed~~ |
| Inline code | `` `mint dev` `` | `mint dev` |

Combine them freely — `**_both at once_**` renders as **_both at once_**.

## Lists

Unordered lists take `-`, `*`, or `+`. Ordered lists take a number followed by a
period. Indent by two spaces to nest.

```markdown
- Install the CLI
  - Node 20 or later is required
- Run the dev server
1. Write the page
2. Add it to `docs.json`
```

## Links and images

```markdown
[Quickstart](/quickstart)
[Mintlify docs](https://mintlify.com/docs)
![Hero](/images/hero-light.svg)
```

Internal links start with `/` and drop the file extension. `mint broken-links`
fails the build if one of them points at a page that does not exist.

## Code blocks

Fence a block with three backticks and name the language for syntax
highlighting. Add a title after the language to label the block.

````markdown
```bash Install
npm i -g mint
```
````

## Blockquotes

```markdown
> Quoted text carries over line breaks
> as long as every line starts with `>`.
```

## Tables

Pipes separate the cells and the second row sets the alignment.

```markdown
| Left | Center | Right |
| :--- | :----: | ----: |
| one  | two    | three |
```

## Horizontal rules

Three or more dashes on their own line draw a divider:

```markdown
---
```

## Escaping

Put a backslash before any character you want rendered literally — `\*not
italic\*` stays as \*not italic\*. Inside code spans and fenced blocks nothing
needs escaping.

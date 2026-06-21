# Blog posts

Each blog post is a single Markdown file in this folder. To publish a new post,
just add a file here — it will automatically appear on the [Blog](/blog/) page
and get its own page rendered from your Markdown.

## File naming

Use the format:

```
YYYY-MM-DD-some-title.md
```

For example: `2026-06-21-welcome-to-my-blog.md`. The date in the filename sets
the post date and the URL.

## Front matter

Start every file with a YAML front matter block:

```yaml
---
title: "My Post Title"
date: 2026-06-21
excerpt: "One-line summary shown in the blog list."
tags:
  - research
  - llm
---
```

- `title` — required. Shown as the heading and in the list.
- `date` — required. Use `YYYY-MM-DD`.
- `excerpt` — optional. A short summary shown under the title in the blog list.
- `tags` — optional. Shown as small chips.

Everything after the front matter is the post body, written in Markdown
(headings, lists, code blocks, links, images, math, etc.).

## Images

Put images in `/images/` and reference them like:

```markdown
![Alt text](/images/my-figure.png)
```

## Previewing locally

Run the site locally and posts will render at `/blog/`:

```bash
bundle exec jekyll serve
```

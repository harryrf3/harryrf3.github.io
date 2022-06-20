---
# (require) default post layout
layout: post
# (require) a string title
title: "Your Title"
# (require) a post date
date: 2016-04-20 19:51:02 +0700
# (custom) some categories, but makesure these categories already exists inside path of `category/`
categories: [javascript]
# (custom) tags only for meta `property="article:tag"`
tags: [foo, bar]
# (custom) image only for meta `property="og:image"`, save your image inside path of `static/img/_posts`
image: Broadcast_Mail.png
---

# Log Entry Setup & Cheat Sheet

## Log Entry Setup:

* Create new file and name it using this formula: `YYYY-MM-DD-LOG-ENTRY-NAME.md`

* type `hblog` to generate the above block (between ---'s)

* Fill out all relative information: `layout, title, date, categories, tags, and image`
<br/>
[layout needs **no** change at this point]

<br/><br/><br/>

> Credit goes to [The Markdown Guide](https://www.markdownguide.org)!

### Heading

# H1
## H2
### H3

### Bold

**bold text**

### Italic

*italicized text*

### Blockquote

> blockquote

### Ordered List

1. First item
2. Second item
3. Third item

### Unordered List

- First item
- Second item
- Third item

### Code

`code`

### Horizontal Rule

---

### Link

[Markdown Guide](https://www.markdownguide.org)

### Image

![alt text](https://www.markdownguide.org/assets/images/tux.png)

## Extended Syntax

These elements extend the basic syntax by adding additional features. Not all Markdown applications support these elements.

### Table

| Syntax | Description |
| ----------- | ----------- |
| Header | Title |
| Paragraph | Text |

### Fenced Code Block

```
{
  "firstName": "John",
  "lastName": "Smith",
  "age": 25
}
```

### Footnote

Here's a sentence with a footnote. [^1]

[^1]: This is the footnote.

### Heading ID

### My Great Heading {#custom-id}

### Definition List

term
: definition

### Strikethrough

~~The world is flat.~~

### Task List

- [x] Write the press release
- [ ] Update the website
- [ ] Contact the media

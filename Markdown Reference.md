---
layout: post
title: Markdown with Typora
---

[TOC]

### Overview

**Markdown** is created by [Daring Fireball](http://daringfireball.net/), the original guidelineis [here](http://daringfireball.net/projects/markdown/syntax). Its syntax, howerer, varies betwween different parsers or editors. **Typora** is using [GitHub Flavored Marksown](https://help.github.com/articles/github-flavored-markdown/).

### Headers

```markdown
# This is an H1

## This is an H2

###### This is an H6
```

### Blockquotes

```markdown
> This is a blockquote with two paragraphs. This is first paragraph.
>
> This is second pragraph. Vestibulum enim wisi, viverra nec, fringilla in, laoreet vitae, risus.



> This is another blockquote with one paragraph. There is three empty line to seperate two blockquote.
```

### Lists

```markdown
## un-ordered list
* Red
* Green
* Blue

## ordered list
1. Red
2. Green
3. Blue
```

### Task List

```markdown
- [ ] a task list item
- [ ] list syntax required
- [ ] normal **formattin**, @mentions, #1234 refs
- [ ] incomplete
- [x] completed
```

### (Fenced) Code Blocks

```markdown
Here's an example:
​```
function test() {
    console.log("notice the blank line before this function?");
}
​```

syntax highlighting:
​```ruby
markdown = Redcarpet.new("Hello World!")
puts markdown.to_html
​```
```

### Math Blocks

You can render *LaTeX* mathematical expressions using **MathJax**.

Input `$$`, then press ‘Return’ key will trigger an input field which accept *Tex/LaTex* source. Following is an example:
$$
\mathbf{V}_1 \times \mathbf{V}_2 =  \begin{vmatrix} 
\mathbf{i} & \mathbf{j} & \mathbf{k} \\
\frac{\partial X}{\partial u} &  \frac{\partial Y}{\partial u} & 0 \\
\frac{\partial X}{\partial v} &  \frac{\partial Y}{\partial v} & 0 \\
\end{vmatrix}
$$
In markdown source file, math block is *LaTeX* expression wrapped by ‘$$’ mark:

```markdown
$$
\mathbf{V}_1 \times \mathbf{V}_2 =  \begin{vmatrix} 
\mathbf{i} & \mathbf{j} & \mathbf{k} \\
\frac{\partial X}{\partial u} &  \frac{\partial Y}{\partial u} & 0 \\
\frac{\partial X}{\partial v} &  \frac{\partial Y}{\partial v} & 0 \\
\end{vmatrix}
$$
```

### Tables

```markdown
| First Header | Second Header |
| ------------ | ------------- |
| Content Cell | Content Cell  |
| Content Cell | Content Cell  |

| Left-Aligned  | Center Aligned  | Right Aligned |
| :------------ |:---------------:| -----:|
| col 3 is      | some wordy text | $1600 |
| col 2 is      | centered        |   $12 |
| zebra stripes | are neat        |    $1 |
```

### Footnotes

```markdonw
You can create footnotes like this[^footnote].
[^footnote]: Here is the *text* of the **footnote**.
```

### Horizontal Rules

```markdown
Input ** or --- on a blank line and press *return will draw a horizontal line.
```

### Yaml Front Matters

Typora support [YAML Front Matters](http://jekyllrb.com/docs/frontmatter/) now.. Input --- at the top of the article and then press `Enter` well introduce one. Or insert one metadata block from the menu.

### Table of Contents (TOC)

Input `[toc]` then press *Return* key will create a section for "Table of Contents" extracting all headers from one's writing, its contents will be updated automatically.

### Span Elements

#### Links

```markdown
This is [an example](http://example.com/ "Title") inline link.
[This link](http://example.com/) has no title attribute.
```

##### internal Links

**You can set the href to headers**, which well create a bookmark that allow you to fump to that section after clicking.

Command(on Windows: Ctrl) + Click [This link](#Headers) will jump to header `Header`.	

##### Reference Links

```markdown
This is [an example][id] reference-style link.
Then, anywhere in document, you define your link label like this, on a line by itself:
[id]:  http://example/ "Optional Tilte Here"

[Google][]
ANd then define the link:
[Google]: http://google.com/
```

### URLs

Typora allows you to insert URLs as links, wrapped by <brackets>.

`<i@typora.io>` becomes <i@typora.io> 

Typora will also auto link standard URLs. e.g: www.google.com

### Images

```markdown
![Alt text](/path/to/img.jpg)
![Alt text](path/to/img.jpg "Optional title")
```

### Emphasis

```markdown
*single asterisks*
_single underscores_

\*this text is surrounded by literal asterisks\*
```

### Strong

```markdown
**double asterisks**
__double underscores__
```

### Code

```markdown
Use the `printf()` function.
```

### Strikethrough

`~~Mistaken text.~~` becomes ~~Mistaken text.~~

### Underlines

`<u>Underline</u>` becomes <u>Underline</u>.

### Emoji :happy:

Input emoji with syntax `:smile:`.

### Inline Math

`$\lim_{x \to \infty} \exp(-x) = 0$`	

rendered

$\lim_{x \to \infty} \exp(-x) = 0$

### Subscript

To use this feature, first, please enalbe it in `Preference` Panel -> `Markdown` Tab. Then use `~` to wrap subscript content, for example: `H~2~o, X~long\ text~/`

### Superscript

To use this feature, first, please enable it in`Preference` Panel -> `Markdown` Tab. Then use `^` to wrap superscript content, for example: `X^2^`

### Highlight

To use this feature, first, please enable it in `Preference` Panel -> `Markdown` Tab. Then use `==` to wrap highlight content, example: `==highlight==`.


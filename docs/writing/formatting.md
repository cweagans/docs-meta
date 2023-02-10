---
title: Formatting
weight: 20
---

{{< lead text="All documentation is written in Markdown. Some extensions beyond the core Markdown spec are available." >}}

Below, you can see examples of all of the plain markdown formatting available to you within project documentation. There are also [Shortcodes]({{< ref "shortcodes.md" >}}) that you can use for specific scenarios.

## H2
### H3
#### H4

## Paragraph styles

Text can be **bold** or _italicized_ or ~~crossed out~~. Text can be `inline code`. You can also [link](https://example.com) to external pages (see [Shortcodes]({{< ref "shortcodes.md" >}}) if you need to link to internal pages or headings).

> Sometimes, you may need to quote something that somebody said.

You can show code in syntax-highlighted code blocks:

```json
{
  "foo": "bar",
  "baz": 123
}
```

You may also need to:
* Put
* Items
* In
* A
* List

Or possibly even:
1. an
2. ordered
3. list

You can add a footnote if you want [^1]

You can also define things if needed.:

**term**
: definition

**another term**
: definition

You can have images too:

![kitteh](http://placekitten.com/g/200/300)

(if you're including images in your content, you may want to be aware of the `figure` shortcode)

Maybe you need to present data in a table:

| Syntax | Description |
| --- | ----------- |
| Header | Title |
| Paragraph | Text |

You can also set alignment within columns:

| Syntax      | Description | Test Text     |
| :---        |    :----:   |          ---: |
| Header      | Title       | Here's this   |
| Paragraph   | Text        | And more      |

[^1]: This is the footnote

---

{{< details title="markdown source for reference (click to expand)" >}}
```markdown
[//]: # (This is how you write a comment in markdown)

## H2
### H3
#### H4

## Paragraph styles

Text can be **bold** or _italicized_ or ~~crossed out~~. Text can be `inline code`. You can also [link](https://example.com) to external pages (see [Shortcodes]({{< ref "shortcodes.md" >}}) if you need to link to internal pages or headings).

> Sometimes, you may need to quote something that somebody said.

You can show code in syntax-highlighted code blocks:

[//]: # (Note that the slashes preceding the backticks on either side of the fenced code block below must be removed in real content. They had to be escaped to show the source inline like this.)

\```json
{
  "foo": "bar",
  "baz": 123
}
\```

You may also need to:
* Put
* Items
* In
* A
* List

Or possibly even:
1. an
2. ordered
3. list

You can add a footnote if you want [^1]

You can also define things if needed.:

**term**
: definition

**another term**
: definition

You can have images too:

![kitteh](http://placekitten.com/g/200/300)

(if you're including images in your content, you may want to be aware of the `figure` shortcode)

Maybe you need to present data in a table:

| Syntax | Description |
| --- | ----------- |
| Header | Title |
| Paragraph | Text |

You can also set alignment within columns:

| Syntax      | Description | Test Text     |
| :---        |    :----:   |          ---: |
| Header      | Title       | Here's this   |
| Paragraph   | Text        | And more      |

[^1]: This is the footnote
```


{{< /details >}}

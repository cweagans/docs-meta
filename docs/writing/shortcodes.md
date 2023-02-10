---
title: Shortcodes
weight: 30
quicklinks:
- title: "Example 1"
  icon: themes
  description: "Some text should go here to describe the link to the user who might click on it."
  href: "#"
- title: "Example 2"
  icon: installation
  description: "Some text should go here to describe the link to the user who might click on it."
  href: "#"
- title: "Example 3"
  icon: plugins
  description: "Some text should go here to describe the link to the user who might click on it."
  href: "#"
- title: "Example 4"
  icon: architecture
  description: "Some text should go here to describe the link to the user who might click on it."
  href: "#"
---

{{< lead text="In addition to the standard markdown formatting, shortcodes can be used for 'fancy' elements." >}}

---

## Relref
Use a `relref` shortcode to link to internal pages or headings.

### Example
[Style Guide]({{< relref "style-guide.md" >}})

[Style Guide (External Resources)]({{< relref "style-guide.md#external-resources" >}})

[Features]({{< relref "../general/features.md" >}})


### Syntax
```markdown
[Style Guide]({{</* relref "style-guide.md" */>}})

[Style Guide (External Resources)]({{</* relref "style-guide.md#external-resources" */>}})

[Features]({{</* relref "../general/features.md" */>}})
```

---

## Figure
Use a `figure` shortcode to display an image with an attached caption.

### Example
{{< figure src="http://placekitten.com/g/200/300" title="A cute kitten" >}}

### Syntax
```markdown
{{</* figure src="http://placekitten.com/g/200/300" title="A cute kitten" */>}}
```

---

## Details
Use a `details` shortcode to create a collapsed content section that can be expanded. This is useful for long code samples or other long reference material that doesn't need to always be visible.

### Example
{{< details title="This is the title of the collapsed section" >}}
This is the content of the collapsed section. **Markdown** can be used too.
{{< /details >}}

### Syntax
```markdown
{{</* details title="This is the title of the collapsed section" */>}}
This is the content of the collapsed section. **Markdown** can be used too.
{{</* /details */>}}
```

---

## Lead
The `lead` shortcode can be used for an introductory sentence at the top of a page that gives context or a summary to the page.

### Example

{{< lead text="This is the text of the lead paragraph" >}}

### Syntax
```markdown
{{</* lead text="This is the text of the lead paragraph" */>}}
```

---

## Callout

A `callout` can be used to draw the reader's attention to something important that might otherwise be overlooked.

### Example

{{< callout title="This is the callout title" >}}
This is some text for the callout. **Markdown** _can_ be used here too.
{{< /callout >}}

### Syntax
```markdown
{{</* callout title="This is the callout title" */>}}
This is some text for the callout. **Markdown** _can_ be used here too.
{{</* /callout */>}}
```

---

## Warning

A `warning` should be used when presenting information that might be considered risky (for example, if performing an action incorrectly could lead to data loss).

### Example

{{< warning title="This is the warning title" >}}
This is some text for the warning. **Markdown** _can_ be used here too.
{{< /warning >}}

### Syntax
```markdown
{{</* warning title="This is the warning title" */>}}
This is some text for the warning. **Markdown** _can_ be used here too.
{{</* /warning */>}}
```

---

## Quicklinks

`quicklinks` are primarily used on project pages in this site. While the shortcode itself is simple, there is some other required configuration in the front matter of the page that they will be displayed on.

### Example

{{< quicklinks >}}

### Syntax

The `quicklinks` shortcode should be inserted into your content wherever you'd like the links to be placed.

```markdown
{{</* quicklinks */>}}
```

The quicklinks must also be defined in the front matter of the page that they are displayed on. 

```yaml
---
title: The Page Title
quicklinks:
- title: "Example 1"
  icon: themes
  description: "Some text should go here to describe the link to the user who might click on it."
  href: "#"
- title: "Example 2"
  icon: installation
  description: "Some text should go here to describe the link to the user who might click on it."
  href: "#"
- title: "Example 3"
  icon: plugins
  description: "Some text should go here to describe the link to the user who might click on it."
  href: "#"
- title: "Example 4"
  icon: architecture
  description: "Some text should go here to describe the link to the user who might click on it."
  href: "#"
---
```

There are four icons available (an example of each is included above), but if you need a different icon, open a documentation issue using the link at the bottom of this page and include some detail about what you need.

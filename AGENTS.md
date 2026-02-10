# Markdown Best Practices

Reference guide for writing consistent and compatible Markdown.
Source: [Markdown Guide](https://www.markdownguide.org/basic-syntax/)

> **Note for AI Agents:** If you have doubts about any specific Markdown syntax or best practice, use the `fetch_webpage` tool to access the official documentation:
> - Basic syntax: `https://www.markdownguide.org/basic-syntax/`
> - Extended syntax: `https://www.markdownguide.org/extended-syntax/`
> - Cheat sheet: `https://www.markdownguide.org/cheat-sheet/`

## ⭐ Emphasis (Italic and Bold)

### Italic

Use **asterisks** (`*`) instead of underscores (`_`) for italics:

| ✅ Correct | ❌ Incorrect |
|------------|--------------|
| `*text*` | `_text_` |
| `*.devcontainer*` | `_.devcontainer_` |

> **Reason:** Markdown applications don't agree on how to handle underscores in the middle of a word. For compatibility, use asterisks.

### Bold

Use **double asterisks** (`**`) instead of double underscores (`__`):

| ✅ Correct | ❌ Incorrect |
|------------|--------------|
| `**text**` | `__text__` |

### Bold and Italic

Use **triple asterisks** (`***`):

| ✅ Correct | ❌ Incorrect |
|------------|--------------|
| `***text***` | `___text___` |

---

## 📝 Headings

- Always put a **space** after the `#`
- Put **blank lines** before and after headings

| ✅ Correct | ❌ Incorrect |
|------------|--------------|
| `# Heading` | `#Heading` |

---

## 📋 Lists

### Unordered Lists

- Use **dashes** (`-`) consistently
- Don't mix delimiters (`-`, `*`, `+`) in the same list

| ✅ Correct | ❌ Incorrect |
|------------|--------------|
| `- Item 1`<br>`- Item 2` | `- Item 1`<br>`* Item 2` |

### Ordered Lists

- Use **periods** (`.`) after the number, not parentheses

| ✅ Correct | ❌ Incorrect |
|------------|--------------|
| `1. Item` | `1) Item` |

---

## 🔗 Links

- Encode spaces with `%20` in URLs
- Encode parentheses: `(` → `%28`, `)` → `%29`

```markdown
[link](https://example.com/my%20page)
```

---

## 📦 Code Blocks

- For inline code: use backticks `` ` ``
- For blocks: use triple backticks with the language

```markdown
`inline code`
```

---

## ➖ Horizontal Rules

- Put **blank lines** before and after

```markdown
Previous text

---

Following text
```

---

## 💬 Blockquotes

- Put **blank lines** before and after blockquotes

```markdown
Previous text

> This is a quote

Following text
```

---

## 🖼️ Images

```markdown
![Alt text](path/to/image.jpg "Optional title")
```

---

## 🔧 Escaping Characters

Use `\` to display literal characters:

```markdown
\* This is not a list
\# This is not a heading
```

Characters you can escape: `\ ` `` ` `` `*` `_` `{}` `[]` `<>` `()` `#` `+` `-` `.` `!` `|`

---

## ✅ Quick Reference

| Element | Use | Don't Use |
|---------|-----|-----------|
| Italic | `*text*` | `_text_` |
| Bold | `**text**` | `__text__` |
| Bold+Italic | `***text***` | `___text___` |
| Unordered list | `-` | Mix `-`, `*`, `+` |
| Ordered list | `1.` | `1)` |
| Headings | `# Heading` | `#Heading` |

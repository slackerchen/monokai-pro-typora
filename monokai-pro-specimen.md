# Monokai Pro (CE) for Typora

Make room for ideas taking shape.

An independently maintained Community Edition for Typora, inspired by Monokai Pro. Warm charcoal, considered contrast, and a little color exactly where you need it.

## 01 — Reading and writing

Good notes keep your attention on the content. Comfortable line spacing, clear heading levels, and system fonts support research notes, technical documentation, and ideas that are still taking shape.

**Clear emphasis without distraction.** *A quiet emphasis.* ~~An idea no longer needed.~~ Use `inline code` for identifiers and <mark>highlighting</mark> for passages worth revisiting. Links use a warm yellow: [Monokai Pro](https://monokai.pro/).

> Color should help you understand, then get out of the way.
>
> Keep the words at the center of the page.

### Write it down to make it clear

- Record the context and assumptions.
- Break a large question into steps you can verify.
  - Identify the facts you know.
  - Keep track of what remains uncertain.
- Review the reasoning behind the answer.

## 02 — Code

Six accent colors distinguish syntax categories. Neutral text and punctuation balance the page, while comments remain readable in a quieter shade.

```javascript
// A small space for a better idea.
class Notebook {
  constructor(title = "A quiet workspace") {
    this.title = title;
    this.pages = 24;
  }

  write(thought) {
    const entry = { text: thought, starred: true };
    return `${this.title}: ${entry.text}`;
  }
}

const notebook = new Notebook();
console.log(notebook.write("Make room for what matters."));
```

```python
from dataclasses import dataclass

@dataclass
class Experiment:
    name: str
    samples: int = 128

    def progress(self, completed: int) -> float:
        """Return progress as a fraction between 0 and 1."""
        return min(completed / self.samples, 1.0)

print(Experiment("Reading rhythm").progress(96))
```

```css
:root {
  --background: #2d2a2e;
  --foreground: #fcfcfa;
}

.workspace:hover {
  color: var(--foreground);
  padding: 1.5rem;
}
```

```json
{
  "theme": "Monokai Pro (CE) for Typora",
  "offline": true,
  "pageWidth": 880,
  "dependencies": null
}
```

```diff
- const noise = "more decoration";
+ const focus = "more clarity";
```

## 03 — Tables and tasks

| Color | Hex | Typical use |
| :--- | :--- | :--- |
| Rose | `#ff6188` | Keywords and operators |
| Orange | `#fc9867` | Parameters and special syntax |
| Yellow | `#ffd866` | Strings, links, and highlights |
| Green | `#a9dc76` | Declarations, functions, and attributes |
| Cyan | `#78dce8` | Types and inline code |
| Purple | `#ab9df2` | Numbers and constants |

- [x] Give the idea a clear structure.
- [x] Record the important details.
- [ ] Leave room to reconsider.

Press <kbd>⌘</kbd> + <kbd>F</kbd> on macOS to find text, or use the View menu to switch to source mode.

## 04 — Alerts and quotations

> [!NOTE]
> Add context to help readers understand what follows.

> [!TIP]
> Start with the simplest useful version and refine it.

> [!IMPORTANT]
> Important information should stand out and remain readable.

> [!WARNING]
> Check this assumption before taking the next step.

> [!CAUTION]
> This example checks the warning color and text contrast.

## 05 — Math and diagrams

Inline math $e^{i\pi}+1=0$ shares the surrounding text color.

$$
\operatorname{Attention}(Q,K,V)
=\operatorname{softmax}\left(\frac{QK^\top}{\sqrt{d_k}}\right)V
$$

```mermaid
flowchart LR
    A[Observe] --> B[Think]
    B --> C{Verify}
    C -->|Refine| B
    C -->|Ready| D[Share]
```

```mermaid
sequenceDiagram
    participant W as Writer
    participant N as Notebook
    W->>N: Capture an idea
    N-->>W: Make it visible
    Note over W,N: A little clarity, every day.
```

### Preserve custom diagram colors

```mermaid
flowchart LR
    A[Custom style]:::custom --> B[Default style]
    classDef custom fill:#ffd866,color:#221f22,stroke:#ffd866
```

## 06 — Headings, footnotes, and edge cases

### Level three · A clear section

This is a regular paragraph. Footnotes keep supporting material nearby without interrupting the reading flow.[^note]

#### Level four · A smaller thought

Body text keeps the same size beneath deeper heading levels.

##### Level five · Supporting detail

A quieter shade distinguishes the heading without making it too small.

###### Level six · A final detail

Even small details should remain clear.

1. The first item in an ordered list.
2. The second item includes a code block:

   ```javascript
   const nested = { readable: true, depth: 2 };
   ```

3. The third item returns to the regular reading flow.

> An outer quotation.
>
> > The nested quotation retains a distinct left border.

Long URL: [https://example.com/research/notes/a-very-long-document-name-for-checking-responsive-layout-and-line-breaking](https://example.com/research/notes/a-very-long-document-name-for-checking-responsive-layout-and-line-breaking)

```text
This intentionally long line checks the code editor's own wrapping or horizontal scrolling behavior without changing the cursor geometry, breaking indentation, or clipping the language selector at the edge of the fence.
Another long line checks that indentation and cursor positioning remain intact when the window narrows, with scrolling or wrapping controlled by Typora settings.
```

[TOC]

[^note]: The theme controls appearance. Typora handles Markdown editing, math typesetting, and diagram rendering.

---

Keep your tools quiet. Let your ideas speak.

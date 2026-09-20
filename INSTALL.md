# Installation

## Install

1. Open [monokai-pro.css](monokai-pro.css) and choose **Download raw file** on GitHub. Save the CSS file, not the GitHub page.
2. In Typora, open **Settings / Preferences → Appearance → Open Theme Folder**.
3. Place `monokai-pro.css` in that folder.
4. Restart Typora and select **Themes → Monokai Pro**.

Typora derives the menu label **Monokai Pro** from `monokai-pro.css`. The full project name is **Monokai Pro (CE) for Typora**.

Open the [Markdown specimen](monokai-pro-specimen.md) to check the result. Math, diagrams, and extended Markdown features depend on your Typora version and Markdown settings.

## Customize

Create `monokai-pro.user.css` in the same theme folder to keep personal changes separate from updates:

```css
:root {
    --mp-page-width: 960px;
    --mp-code-font: "JetBrains Mono", Menlo, Consolas, monospace;
}

html { font-size: 17px; }
```

Install any custom fonts yourself. Typora's font preferences may override theme defaults.

## Update

Back up any changes made directly to the theme, replace `monokai-pro.css` with the new version, and restart Typora. Keep your `monokai-pro.user.css` file.

## PDF and printing

If a PDF looks different from the editor, check **Settings / Preferences → Export → PDF → Theme**. Select the current theme or **Monokai Pro** to use this theme's print stylesheet.

The print stylesheet uses a light background; Mermaid diagrams retain a dark panel so their labels stay readable. The specimen was exported and visually checked in Typora 1.14.10 on macOS. Long code blocks can continue on the next page. Check your own long tables, formulas, and diagrams after export.

## Uninstall

Switch to another theme, remove `monokai-pro.css` from the theme folder, and restart Typora. Remove or keep `monokai-pro.user.css` as needed.

Reference: [Typora — About Themes](https://support.typora.io/About-Themes/).

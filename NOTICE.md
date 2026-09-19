# Attribution and distribution scope

## Monokai Pro Community Edition

The public project name is **Monokai Pro (CE) for Typora**. This is an independently maintained implementation for Typora, based on the default Monokai Pro palette. It is not an official Monokai product and does not claim acceptance into the official Community Edition directory.

Sources:

- Original palette and brand: <https://monokai.pro/>
- Community Edition publishing rules: <https://monokai.pro/contribute>
- Official repository template: <https://github.com/monokai-pro/community-edition>
- Template license: <https://github.com/monokai-pro/community-edition/blob/main/LICENSE.md>

`LICENSE.md` preserves the MIT text and the `Copyright © 2025 Monokai` notice from the official CE template retrieved on 2026-09-19. A separate 2026 notice identifies this project's contributors. The template license does not license an unrelated author's files or grant ownership of Monokai's brand or official icon pack.

## CE publishing rules

The official contribution page specifies that a Community Edition must target an app without an official Monokai Pro theme, use the name “Monokai Pro (CE)”, contain only the default filter, be free, non-commercial and open source, allow Monokai to potentially take over the package, and use the official template.

This project is prepared for that community publishing route and grants Monokai the right to potentially take over this package under those rules. The MIT license is retained as supplied by the template; the publisher's CE rules are recorded separately rather than silently rewriting the license. Consult Monokai for clarification before a distribution model that conflicts with those published rules.

The project does not bundle official paid extensions, additional filters, or the official icon pack. The publishing rules should be checked again before submitting to the official directory.

## Included files

The distributable implementation consists of `monokai-pro.css`, the authored Markdown specimen and the accompanying project documentation. The CSS uses installed system fonts and contains no remote imports, bundled fonts or JavaScript libraries.

Typora's application CSS was consulted to identify supported selectors and variables. Its stylesheets are not included in the standalone theme file.

## Excluded local material

The `參考/` directory, legacy `monokai.css` / `light-monokai.css`, local development notes, `.DS_Store` and generated HTML/PDF files are not part of this distribution.

In particular, `monokai-pro-specimen.html` is a local Typora export containing additional Typora/CodeMirror styles, MathJax SVG output and Mermaid diagram styles/output. A complete set of applicable redistribution licenses and notices for those embedded components has not been established. That HTML is excluded until a separate component-by-component license review is completed. This exclusion is not a claim that all exported documents are prohibited from redistribution.

This repository starts with the curated, independently authored theme and documentation. It does not include the reference project's Git history or legacy theme files.

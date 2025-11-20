# Docker image of Material for MkDoc

> [!Warning]
> Material for MkDocs is now in maintenance mode
>
> This is the last release of Material for MkDocs that will receive new features. Going forward, the Material for MkDocs team focuses on [Zensical](https://zensical.org/), a next-gen static site generator built from first principles. We will provide critical bug fixes and security updates for Material for MkDocs for 12 months at least.

## How to build

### Latest

```sh
docker buildx build \
    --platform linux/amd64,linux/arm64 \
    --output=type=registry \
    --tag sig9/mkdocs-material:latest \
    versions/9.7.0/
```

### 9.7.0

```sh
docker buildx build \
    --platform linux/amd64,linux/arm64 \
    --output=type=registry \
    --tag sig9/mkdocs-material:9.7.0 \
    versions/9.7.0/
```

## Installed extensions

### Themes

- [Material Design theme](https://squidfunk.github.io/mkdocs-material/) usings Google’s Material Design guidelines.

### Plugins

- [autorefs](https://github.com/mkdocstrings/autorefs) automatically link across pages.
- [markdown](https://github.com/Python-Markdown/markdown) is Python implementation of John Gruber's Markdown.
- [Material Extensions](https://github.com/facelessuser/mkdocs-material-extensions) extension resources for MkDocs for Material
- [Minify](https://github.com/byrnereese/mkdocs-minify-plugin) to minify HTML and/or JS files prior to being written to disk.
- [Mkdocs with Confluence](https://github.com/pawelsikora/mkdocs-with-confluence/) Plugin for uploading markdown documentation to Confluence via Confluence REST API
- [mkdocs_macros_plugin](https://github.com/fralau/mkdocs_macros_plugin) transforms the markdown pages into jinja2 templates that use variables, calls to macros and custom filters.
- [mkdocs_puml](https://github.com/MikhailKravets/mkdocs_puml) is a fast and simple package that brings plantuml diagrams to MkDocs documentation.
- [mkdocs_pymdownx_material_extras](https://github.com/facelessuser/mkdocs_pymdownx_material_extras)
- [mkdocs-abs-rel-plugin](https://github.com/sander76/mkdocs-abs-rel-plugin)
- [mkdocs-add-number-plugin](https://github.com/ignorantshr/mkdocs-add-number-plugin) plugin to automatically number the headings (h1-h6) in each markdown page and the nav.
- [mkdocs-autolinks-plugin](https://github.com/midnightprioriem/mkdocs-autolinks-plugin/) simplifies relative linking between documents.
- [mkdocs-awesome-pages-plugin](https://github.com/lukasgeiter/mkdocs-awesome-pages-plugin) allows you to customize how your pages show up the navigation of your MkDocs without having to configure the full structure in your `mkdocs.yml`.
- [mkdocs-breadcrumbs-plugin](https://github.com/mihaigalos/mkdocs-breadcrumbs-plugin) is Mkdocs location-based breadcrumbs navigation.
- [mkdocs-build-plantuml-plugin](https://github.com/christo-ph/mkdocs_build_plantuml) automates the generation of PlantUML image files when using mkdocs serve.
- [mkdocs-categories-plugin](https://github.com/EddyLuten/mkdocs-categories-plugin) allows for multiple categories per page and will generate a category index page
- [mkdocs-drawio](https://github.com/tuunit/mkdocs-drawio/) enables you to embed interactive drawio diagrams in your documentation.
- [mkdocs-enumerate-headings-plugin](https://github.com/timvink/mkdocs-enumerate-headings-plugin) will enumerate the headings (h1-h6) across site pages.
- [mkdocs-exclude-unused-files](https://github.com/JonasDoesThings/mkdocs-exclude-unused-files) for excluding files from being included in the mkdocs output if they are not referenced on other pages.
- [mkdocs-exclude](https://github.com/apenwarr/mkdocs-exclude) allows you to exclude files from your input using unix-style wildcards (globs) or regular expressions (regexes).
- [mkdocs-gallery](https://smarie.github.io/mkdocs-gallery/)
- [mkdocs-gemini-chatbot](https://github.com/vimmoos/mkdocs-gemini-chatbot) that adds a conversational chatbot to your documentation site, powered by Google's Gemini models. The chatbot uses the entire content of your documentation, including auto-generated API references, to provide intelligent, context-aware answers with precise, clickable links to the relevant sections.
- [mkdocs-gen-files](https://oprypin.github.io/mkdocs-gen-files/) programmatically generates documentation pages during the build.
- [mkdocs-git-authors-plugin](https://github.com/timvink/mkdocs-git-authors-plugin)
- [mkdocs-git-committers-plugin-2](https://github.com/ojacques/mkdocs-git-committers-plugin-2)
- [mkdocs-git-revision-date-localized-plugin](https://github.com/timvink/mkdocs-git-revision-date-localized-plugin)
- [mkdocs-img2fig-plugin](https://github.com/stuebersystems/mkdocs-img2fig-plugin) converts `<img>` to `<figure>`.
- [mkdocs-kroki-plugin](https://github.com/AVATEAM-IT-SYSTEMHAUS/mkdocs-kroki-plugin)
- [mkdocs-link-marker](https://github.com/timmeinerzhagen/mkdocs-link-marker) for marking external or mail links in your documentation.
- [mkdocs-literate-nav](https://oprypin.github.io/mkdocs-literate-nav/) specifies the navigation in Markdown instead of YAML.
- [mkdocs-markdownextradata-plugin](https://github.com/rosscdh/mkdocs-markdownextradata-plugin) injects the mkdocs.yml extra variables into the markdown template.
- [mkdocs-merge](https://github.com/ovasquez/mkdocs-merge) allows you to merge the source of multiple MkDocs sites into a single one converting each of the specified sites to a sub-site of the master site.
- [mkdocs-monorepo-plugin](https://github.com/spotify/mkdocs-monorepo-plugin) Build multiple documentation in a single Mkdocs. Designed for large codebases.
- [mkdocs-multirepo-plugin](https://github.com/jdoiro3/mkdocs-multirepo-plugin) Build documentation in multiple repos into one site.
- [mkdocs-nav-weight](https://github.com/shu307/mkdocs-nav-weight) enables to organize navigation in a more markdownic way
- [mkdocs-no-sitemap-plugin](https://github.com/leonardehrenfried/mkdocs-no-sitemap-plugin) disables the generation of a sitemap in Mkdocs sites.
- [mkdocs-print-site-plugin](https://timvink.github.io/mkdocs-print-site-plugin/index.html) adds a page to your site combining all pages, allowing your site visitors to `File > Print > Save as PDF` the entire site.
- [mkdocs-publish-control](https://github.com/gabrielbdornas/mkdocs-publish-control) that allows you to control page visibility based on metadata. Perfect for managing draft content or private documentation within your MkDocs site.
- [mkdocs-publisher](https://mkusz.github.io/mkdocs-publisher/)
- [mkdocs-redirects](https://github.com/datarobot/mkdocs-redirects) to create page redirects (e.g. for moved/renamed pages).
- [mkdocs-ruby-plugin](https://github.com/lesliezhu/mkdocs-ruby-plugin) to add pinyin/furigana to Chinese/Japanese Kanji text.
- [mkdocs-safe-text-plugin](https://github.com/raimon49/mkdocs-safe-text-plugin) for safe text editing with MKDocs.
- [mkdocs-same-dir](https://oprypin.github.io/mkdocs-same-dir/) allows placing mkdocs.yml in the same directory as documentation.
- [mkdocs-simple-hooks](https://github.com/aklajnert/mkdocs-simple-hooks) to define your own hooks for mkdocs, without having to create a new package.
- [mkdocs-simple-plugin](https://www.althack.dev/mkdocs-simple-plugin) enables you to build a documentation site from markdown interspersed within your repository using mkdocs.
- [mkdocs-swagger-ui-tag](https://blueswen.github.io/mkdocs-swagger-ui-tag/)
- [mkdocs-table-of-figures](https://gitlab.com/thiti-mkdocs-plugins/mkdocs-table-of-figures) that automatically generates figures with a figcaption, and lists all figures across your documentation into a Table of Figures that can be inserted into your Markdown pages.
- [mkdocs-toggle-sidebar-plugin](https://github.com/six-two/mkdocs-toggle-sidebar-plugin) allows you to toggle the left (navigation) and right (table of contents) sidebars on a couple of MkDocs themes such as Material for MkDocs.
- [mkdocs-video](https://github.com/soulless-viewer/mkdocs-video) allows you to embed videos on the documentation pages using a simple Markdown syntax.
- [Mkdocstrings](https://mkdocstrings.github.io/) automatic documentation from sources.
- [Neoterot plugins](https://www.neoteroi.dev/mkdocs-plugins/)

### Markdown extension

- [Breakless Lists Markdown Extension](https://github.com/adamb70/mdx-breakless-lists) Use lists without requiring a line break above them.
- [Customblocks](https://github.com/vokimon/markdown-customblocks) settles a common markup for parametrizable and nestable components.
- [Include](https://github.com/cmacmackin/markdown-include/) allows the inclusion of the contents of other Markdown documents.
- [Mdx Truly Sane Lists](https://github.com/radude/mdx_truly_sane_lists) that makes lists truly sane. Features custom indents for nested lists and fix for messy linebreaks and paragraphs between lists.
- [Pygments](http://pygments.org/) is a generic syntax highlighter.
- [PyMdown Extensions](https://facelessuser.github.io/pymdown-extensions/) is a collection of extensions for Python Markdown.

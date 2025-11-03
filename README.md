# Docker image of Material for MkDoc

## How to build

```sh
docker buildx build \
    --platform linux/amd64,linux/arm64 \
    --output=type=registry \
    --tag sig9/mkdocs-material:latest \
    versions/9.6.23/
```

```sh
docker buildx build \
    --platform linux/amd64,linux/arm64 \
    --output=type=registry \
    --tag sig9/mkdocs-material:9.6.23 \
    versions/9.6.23/
```

## Installed extensions

### Themes

- [Material Design theme](https://squidfunk.github.io/mkdocs-material/) usings Google’s Material Design guidelines.

### Plugins

- [autorefs](https://github.com/mkdocstrings/autorefs) automatically link across pages.
- [Markdown](https://github.com/Python-Markdown/markdown) is Python implementation of John Gruber's Markdown.
- [mkdocs_macros_plugin](https://github.com/fralau/mkdocs_macros_plugin) transforms the markdown pages into jinja2 templates that use variables, calls to macros and custom filters.
- [mkdocs_notion_plugin](https://github.com/cartaorobbin/mkdocs-notion-plugin) that integrates Notion content into your documentation.
- [mkdocs_puml](https://github.com/MikhailKravets/mkdocs_puml) is a fast and simple package that brings plantuml diagrams to MkDocs documentation.
- [mkdocs_pymdownx_material_extras](https://github.com/facelessuser/mkdocs_pymdownx_material_extras)
- [mkdocs-abs-rel-plugin](https://github.com/sander76/mkdocs-abs-rel-plugin)
- [mkdocs-add-number-plugin](https://github.com/ignorantshr/mkdocs-add-number-plugin) plugin to automatically number the headings (h1-h6) in each markdown page and the nav.
- [mkdocs-addresses](https://gitlab.com/frederic-zinelli/mkdocs-addresses) Abstraction of the concrete tree hierarchy of pages and anchors within those when writing a link, utilizing unique identifiers.
- [mkdocs-ai-summary-wcowin](https://github.com/Wcowin/Mkdocs-AI-Summary-Plus) An intelligent MkDocs plugin that automatically generates AI-driven summaries for your documentation pages using multiple AI services, including OpenAI, DeepSeek, Google Gemini, and GLM.
- [mkdocs-ansible-collection](https://github.com/cmsirbu/mkdocs-ansible-collection) that automatically generates documentation pages for Ansible Collections. Check out the showcase over on the project's documentation page and more detailed User and Developer guides!
- [mkdocs-api-autonav](https://github.com/tlambert03/mkdocs-api-autonav) Autogenerate API reference including navigation for all submodules, with mkdocstrings.
- [mkdocs-apidescribed-plugin](https://github.com/idlesign/mkdocs-apidescribed-plugin) to generate API documentation for Python programs.
- [mkdocs-asciidoctor-backend](https://github.com/aireilly/mkdocs-asciidoctor-backend) replaces the MkDocs default Markdown processor with Asciidoctor for AsciiDoc files, allowing you to write documentation in AsciiDoc while keeping full compatibility with Material for MkDocs.
- [mkdocs-asciinema-player](https://github.com/pa-decarvalho/mkdocs-asciinema-player) to include asciinema player in your documentation.
- [mkdocs-audiotag](https://github.com/aeskildsen/mkdocs-audiotag) for the wonderful mkdocs static site generator that allows for easy embedding of audio files using the default HTML5 audio element.
- [mkdocs-authors-plugin](https://github.com/thomaszwagerman/mkdocs-authors-plugin) designed to dynamically generate an "Authors" page for your documentation site from a simple YAML file. This allows you to easily manage and display information about contributors without manually updating Markdown files.
- [mkdocs-auto-figure-list](https://github.com/Privatacc/mkdocs-auto-figure-list) earches through all markdown files for the HTML tags `<figure>` and `<figcaption>`.
- [mkdocs-auto-refresh-build-pages](https://github.com/JakubAndrysek/mkdocs-auto-refresh-build-pages) for live development in production. The plugin adds a popup window that asks the user if he wants to reload the (compiled) page when the page has been updated. This tool is useful when you are deploying your MkDocs pages to production and you want to inform the user that the page has been updated.
- [mkdocs-autolinks-plugin](https://github.com/midnightprioriem/mkdocs-autolinks-plugin/) simplifies relative linking between documents.
- [mkdocs-autorefs](https://mkdocstrings.github.io/autorefs/) Automatically link across pages in MkDocs.
- [mkdocs-awesome-nav](https://github.com/lukasgeiter/mkdocs-awesome-nav) gives you full control over your navigation structure without having to write the entire thing by hand. Whether you just want to add an external link or restructure the entire navigation tree, awesome-nav has you covered.
- [mkdocs-awesome-pages-plugin](https://github.com/lukasgeiter/mkdocs-awesome-pages-plugin) allows you to customize how your pages show up the navigation of your MkDocs without having to configure the full structure in your `mkdocs.yml`.
- [mkdocs-backlinks-section-plugin](https://github.com/six-two/mkdocs-backlinks-section-plugin) Adds a backlinks section that lists every page linking to the current page.
- [mkdocs-badges](https://github.com/six-two/mkdocs-badges) allows you to add badges to your MkDocs site.
- [mkdocs-breadcrumbs-plugin](https://github.com/mihaigalos/mkdocs-breadcrumbs-plugin) is Mkdocs location-based breadcrumbs navigation.
- [mkdocs-build-plantuml-plugin](https://github.com/christo-ph/mkdocs_build_plantuml) automates the generation of PlantUML image files when using mkdocs serve.
- [mkdocs-callouts-codeblock](https://github.com/yimoyuyan/mkdocs-callouts-codeblock) Based on the mkdocs-callouts extension. Depends on Obsidian-Plugin.
- [mkdocs-categories-plugin](https://github.com/EddyLuten/mkdocs-categories-plugin) allows for multiple categories per page and will generate a category index page
- [mkdocs-cc-license-plugin](https://github.com/JM2K69/mkdocs-cc-license-plugin) that automatically adds Creative Commons license icons and links based on the license property in page metadata.
- [mkdocs-changelog-feed-plugin](https://tmb.codeberg.page/mkdocs-changelog-feed-plugin/) plugin that adds RSS and Atom feeds for a changelog.
- [mkdocs-charts-plugin](https://github.com/timvink/mkdocs-charts-plugin) to create plots from data using the declarative vegalite syntax.
- [mkdocs-click](https://github.com/mkdocs/mkdocs-click) to generate documentation for Click command line applications.
- [mkdocs-copy-markdown](https://github.com/ndrezn/mkdocs-copy-markdown) that adds a "Copy as Markdown" button to every rendered documentation page, making it easy to copy content for pasting into AI assistants or sharing with others.
- [mkdocs-copy-to-llm](https://github.com/leonardocustodio/mkdocs-copy-to-llm) that adds "Copy to LLM" buttons to your documentation, making it easy to copy code blocks and entire pages in formats optimized for Large Language Models (LLMs).
- [mkdocs-coverage](https://pawamoy.github.io/mkdocs-coverage/) to integrate your coverage HTML report into your site.
- [mkdocs-decodiff-plugin](https://github.com/kkAyataka/mkdocs-decodiff-plugin) is an MkDocs plugin for decorating Git diff lines.
- [mkdocs-document-dates](https://github.com/jaywhj/mkdocs-document-dates) A new generation MkDocs plugin for displaying exact creation time, last update time, authors, email of documents
- [mkdocs-drawio](https://github.com/tuunit/mkdocs-drawio/) enables you to embed interactive drawio diagrams in your documentation.
- [mkdocs-encryptcontent-plugin](https://unverbuggt.github.io/mkdocs-encryptcontent-plugin/) allows you to have password protected articles and pages in MKdocs.
- [mkdocs-entangled-plugin](https://entangled.github.io/mkdocs-plugin/) Using this plugin, you can make your Entangled documents look better.
- [mkdocs-enumerate-headings-plugin](https://github.com/timvink/mkdocs-enumerate-headings-plugin) will enumerate the headings (h1-h6) across site pages.
- [mkdocs-excalidraw](https://github.com/qdeli187/mkdocs-excalidraw) A simple mkdocs plugin to easily embed your excalidraw drawings into your docs.
- [mkdocs-exclude-unused-files](https://github.com/JonasDoesThings/mkdocs-exclude-unused-files) for excluding files from being included in the mkdocs output if they are not referenced on other pages.
- [mkdocs-exclude](https://github.com/apenwarr/mkdocs-exclude) allows you to exclude files from your input using unix-style wildcards (globs) or regular expressions (regexes).
- [mkdocs-execute-plugin](https://gitlab.kwant-project.org/qt/mkdocs-execute-plugin) that executes documentation files using jupytext and embeds the output in your documentation.
- [mkdocs-extrafiles](https://paddy74.github.io/mkdocs-extrafiles/) is a lightweight MkDocs plugin that allows you to add files and directories from outside MkDocs document directory (docs_dir) to your MkDocs site build.
- [mkdocs-ezglossary-plugin](https://github.com/realtimeprojects/mkdocs-ezglossary) A powerful glossary plugin for MkDocs.
- [mkdocs-fedi-comments](https://bovine.codeberg.page/mkdocs_fedi_comments/) Consider a generated static site, e.g. this one. Wouldn't it be nice if you could comment from the Fediverse on it? Well you can! Just copy the URL of this page into your Fediverse application search and look up an object, you can comment on, to add comments here.
- [mkdocs-fun-plugin](https://github.com/gbbirkisson/mkdocs-fun-plugin) Dead simple custom python functions with mkdocs.
- [mkdocs-gallery](https://smarie.github.io/mkdocs-gallery/)
- [mkdocs-gemini-chatbot](https://github.com/vimmoos/mkdocs-gemini-chatbot) that adds a conversational chatbot to your documentation site, powered by Google's Gemini models. The chatbot uses the entire content of your documentation, including auto-generated API references, to provide intelligent, context-aware answers with precise, clickable links to the relevant sections.
- [mkdocs-gen-files](https://oprypin.github.io/mkdocs-gen-files/) programmatically generates documentation pages during the build.
- [mkdocs-git-authors-plugin](https://github.com/timvink/mkdocs-git-authors-plugin)
- [mkdocs-git-committers-plugin-2](https://github.com/ojacques/mkdocs-git-committers-plugin-2)
- [mkdocs-git-latest-changes-plugin](https://tombreit.github.io/mkdocs-git-latest-changes-plugin/) that allows you to display a list of recently modified pages from the Git log.
- [mkdocs-git-revision-date-localized-plugin](https://github.com/timvink/mkdocs-git-revision-date-localized-plugin) plugin that enables displaying the date of the last git modification of a page.
- [mkdocs-glightbox](https://blueswen.github.io/mkdocs-glightbox/) supports image lightbox with GLightbox. GLightbox is a pure javascript lightbox library with mobile support.
- [mkdocs-google-translate](https://github.com/sondregronas/mkdocs-google-translate) to add relative paths to Google Translate queries.
- [mkdocs-htmlproofer-plugin](https://github.com/manuzhang/mkdocs-htmlproofer-plugin) plugin that validates URLs, including anchors, in rendered html files.
- [mkdocs-image-gallery-plugin](https://github.com/APinchofDill/mkdocs-image-gallery-plugin) to autogenerate a gallery based on a folder of images
- [mkdocs-img2fig-plugin](https://github.com/stuebersystems/mkdocs-img2fig-plugin) converts `<img>` to `<figure>`.
- [mkdocs-include-folders](https://github.com/hhdale/mkdocs-include-folders) that allows you to include and prioritize folders from your input.
- [mkdocs-include-markdown-plugin](https://github.com/mondeja/mkdocs-include-markdown-plugin) Mkdocs Markdown includer plugin.
- [mkdocs-include-stubs-plugin](https://github.com/ACCESS-NRI/mkdocs_include_stubs_plugin) to include stubs (single pages) from multiple GitHub branches of a repo within a mkdocs website build. A stub consists of a file in either of the supported file formats.
- [mkdocs-ipynb](https://github.com/patrick-kidger/mkdocs_ipynb) for loading Jupyter notebooks. Interoperates with all other MkDocs features.admonitions, reference links, etc.
- [mkdocs-jupyterlite](https://github.com/NickCrews/mkdocs-jupyterlite) for embedding interactive notebooks in your docs via jupyterlite.
- [mkdocs-kroki-plugin)](https://github.com/AVATEAM-IT-SYSTEMHAUS/mkdocs-kroki-plugin)
- [mkdocs-link-cards](https://pypi.org/project/mkdocs-link-cards/) Discord-style link previews for MkDocs, rendered as Material cards at build time.
- [mkdocs-link-marker](https://github.com/timmeinerzhagen/mkdocs-link-marker) for marking external or mail links in your documentation.
- [mkdocs-literate-nav](https://oprypin.github.io/mkdocs-literate-nav/) specifies the navigation in Markdown instead of YAML.
- [mkdocs-llmstxt-md](https://github.com/noklam/mkdocs-llmstxt-md) is inspired by mkdocs-llmstxt, the key difference is that mkdocs-llmstxt take the parsing HTML approach which can be used with injected HTML. This plugin focus on the raw markdown approach, which makes things simpler if you only need to work with markdown content.
- [mkdocs-llmstxt](https://pawamoy.github.io/mkdocs-llmstxt/) to generate an /llms.txt file.
- [mkdocs-macros-adr-summary](https://febus982.github.io/mkdocs-macros-adr-summary/) is a macro plugin to generates summaries from a list of a ADR documents in a directory.
- [mkdocs-macros-plugin](https://github.com/fralau/mkdocs-macros-plugin) that uses variables and macros (functions) to automate tasks, and produce richer and more beautiful pages.
- [mkdocs-markdownextradata-plugin](https://github.com/rosscdh/mkdocs-markdownextradata-plugin) injects the mkdocs.yml extra variables into the markdown template.
- [mkdocs-markupsafe-markdown-filter](https://github.com/ntno/mkdocs-markupsafe-markdown-filter) adds pallets' MarkupSafe template filter to mkdocs.
- [mkdocs-material-codeberg-source-facts](https://helge.codeberg.page/mkdocs-material-codeberg-source-facts/) allows you to display the source facts from codeberg. For example without this plugin one has
- [mkdocs-material-extensions)](https://github.com/facelessuser/mkdocs-material-extensions) extension resources for MkDocs for Material
- [mkdocs-mcq](https://pypi.org/project/mkdocs-mcq/) to create and display single and multiple-choice quizzes directly within your documentation.
- [mkdocs-md-preview](https://github.com/Paulkm2006/mkdocs-md-preview) that renders markdown code blocks with md preview syntax into side-by-side boxes, showing both the original source code and the rendered output.
- [mkdocs-media-gallery-plugin](https://github.com/APinchofDill/mkdocs-media-gallery-plugin) for that adds image and YouTube galleries with shortcodes.
- [mkdocs-merge](https://github.com/ovasquez/mkdocs-merge) allows you to merge the source of multiple MkDocs sites into a single one converting each of the specified sites to a sub-site of the master site.
- [mkdocs-mermaid-to-image](https://github.com/nuitsjp/mkdocs-mermaid-to-svg) to convert Mermaid charts to SVG images.
- [mkdocs-mermaid-zoom](https://github.com/lijma/mkdocs-mermaid-zooming) that adds zoom, pan, and lightbox functionality to Mermaid diagrams.
- [mkdocs-mermaid2-plugin](https://github.com/fralau/mkdocs-mermaid2-plugin) that renders Mermaid text descriptions into diagrams (flow charts, sequence diagrams, pie charts, etc.).
- [mkdocs-meta-descriptions-plugin](https://github.com/prcr/mkdocs-meta-descriptions-plugin) to automatically generate meta descriptions for your pages using the first paragraph of each page.
- [mkdocs-minify-html-plugin](https://github.com/monosans/mkdocs-minify-html-plugin) plugin for minification using minify-html, an extremely fast and smart HTML + JS + CSS minifier.
- [mkdocs-minify-plugin](https://github.com/byrnereese/mkdocs-minify-plugin) to minify HTML and/or JS files prior to being written to disk.
- [mkdocs-monorepo-plugin](https://github.com/spotify/mkdocs-monorepo-plugin) Build multiple documentation in a single Mkdocs. Designed for large codebases.
- [mkdocs-multirepo-plugin](https://github.com/jdoiro3/mkdocs-multirepo-plugin) Build documentation in multiple repos into one site.
- [mkdocs-nav-weight](https://github.com/shu307/mkdocs-nav-weight) enables to organize navigation in a more markdownic way
- [mkdocs-navsorted-plugin](https://github.com/idlesign/mkdocs-navsorted-plugin) to get nav sorted without yml directives.
- [mkdocs-nbconvert](https://tanbro.github.io/mkdocs-nbconvert/) provides a source parser for *.ipynb Jupyter Notebook files, based on nbconvert.
- [mkdocs-nbsync](https://github.com/daizutabi/mkdocs-nbsync/) is a MkDocs plugin that seamlessly embeds Jupyter notebook visualizations in your documentation, solving the disconnect between code development and documentation.
- [mkdocs-network-graph-plugin](https://github.com/develmusa/mkdocs-network-graph-plugin) Add an interactive knowledge network graph to your Material for MkDocs documentation project.
- [mkdocs-no-sitemap-plugin](https://github.com/leonardehrenfried/mkdocs-no-sitemap-plugin) disables the generation of a sitemap in Mkdocs sites.
- [mkdocs-nodegraph](https://yonge123.github.io/mkdocs-nodegraph/nodegraph.html) for Visualizing Network Graphs in MkDocs.
- [mkdocs-obsidian-bridge](https://github.com/GooRoo/mkdocs-obsidian-bridge) that helps exporting your Obsidian vault as an MkDocs site.
- [mkdocs-panzoom-plugin](https://github.com/PLAYG0N/mkdocs-panzoom) makes use of the panzoom (LICENCE) library by Andrei Kashcha
- [mkdocs-pipeline-visualizer](https://github.com/obegron/mkdocs-pipeline-visualizer) automates the creation of up-to-date documentation for your Tekton pipelines and tasks.
- [mkdocs-plugins](https://www.neoteroi.dev/mkdocs-plugins/)
- [mkdocs-print-site-plugin](https://timvink.github.io/mkdocs-print-site-plugin/index.html) adds a page to your site combining all pages, allowing your site visitors to `File > Print > Save as PDF` the entire site.
- [mkdocs-publish-control](https://github.com/gabrielbdornas/mkdocs-publish-control) that allows you to control page visibility based on metadata. Perfect for managing draft content or private documentation within your MkDocs site.
- [mkdocs-publisher](https://mkdocs-publisher.github.io/) is a set of plugins that extends MkDocs with a set of plugins, that help to create, edit and publish your content.
- [mkdocs-quiz](https://github.com/skyface753/mkdocs-quiz) You can also create a multiple choice quiz, by providing multiple answers as correct.
- [mkdocs-recently-updated-docs](https://github.com/jaywhj/mkdocs-recently-updated-docs) One line of code to display a list of recently updated documents in MkDocs.
- [mkdocs-redirects](https://github.com/datarobot/mkdocs-redirects) to create page redirects (e.g. for moved/renamed pages).
- [mkdocs-redoc-tag](https://blueswen.github.io/mkdocs-redoc-tag/) supports adding Redoc to the page.
- [mkdocs-rich-argparse](https://github.com/i-VRESSE/mkdocs_rich_argparse) to generate documentation for a rich argparse parser. It renders commands, sub commands and sub-sub commands which can have rich help messages.
- [mkdocs-rss-plugin](https://github.com/Guts/mkdocs-rss-plugin) A plugin for MkDocs, the static site generator, which creates RSS 2.0 and JSON Feed 1.1 feeds using the creation and modification dates from git log and page metadata (YAML frontmatter).
- [mkdocs-safe-text-plugin](https://github.com/raimon49/mkdocs-safe-text-plugin) for safe text editing with MKDocs.
- [mkdocs-same-dir](https://oprypin.github.io/mkdocs-same-dir/) allows placing mkdocs.yml in the same directory as documentation.
- [mkdocs-section-index](https://github.com/oprypin/mkdocs-section-index) to allow clickable sections that lead to an index page.
- [mkdocs-simple-hooks](https://github.com/aklajnert/mkdocs-simple-hooks) to define your own hooks for mkdocs, without having to create a new package.
- [mkdocs-simple-plugin](https://www.althack.dev/mkdocs-simple-plugin) enables you to build a documentation site from markdown interspersed within your repository using mkdocs.
- [mkdocs-site-urls](https://github.com/OctoPrint/mkdocs-site-urls) that adds support for site-relative `site:` URLs.
- [mkdocs-sitemap-exclusion](https://github.com/DmitriyReztsov/mkdocs_sitemap_exclusion) that removes specific URLs from the generated sitemap.xml based on configuration settings in mkdocs.yml.
- [mkdocs-snippets](https://github.com/BetonQuest/mkdocs-snippets) allows you to include snippets in your mkdocs documentation.
- [mkdocs-spellcheck](https://pawamoy.github.io/mkdocs-spellcheck/) can use different backends to check the spelling of words in your final HTML pages. These backends are: codespell, symspellpy.
- [mkdocs-sqlite-console](https://epithumia.github.io/mkdocs-sqlite-console/) is a plugin for MkDocs that displays an SQL IDE (SQLite) for executing code. It is primarily intended for teachers and students: teachers can enter code that students can then execute to see the results of their queries.
- [mkdocs-statistics-plugin](https://github.com/TonyCrane/mkdocs-statistics-plugin) A plugin for mkdocs documentation statistics, including total page count, word count, lines of code, average words per page, lines of code per page, number of images, and estimated reading time.
- [mkdocs-suppress-logs-plugin](https://github.com/darrelk/mkdocs-suppress-logs-plugin) allows you to silence specific log messages using customizable wildcard patterns. It's especially useful for suppressing known, non-critical log lines.
- [mkdocs-swagger-ui-tag](https://blueswen.github.io/mkdocs-swagger-ui-tag/) supports adding Swagger UI to the page.
- [mkdocs-table-of-figures](https://gitlab.com/thiti-mkdocs-plugins/mkdocs-table-of-figures) that automatically generates figures with a figcaption, and lists all figures across your documentation into a Table of Figures that can be inserted into your Markdown pages.
- [mkdocs-test](https://github.com/fralau/mkdocs-test) A testing framework (plugin + test fixture) for MkDocs projects.
- [mkdocs-to-pdf](https://github.com/domWalters/mkdocs-to-pdf) is an mkdocs plugin to generate a PDF from an MkDocs repository.
- [mkdocs-toggle-sidebar-plugin](https://github.com/six-two/mkdocs-toggle-sidebar-plugin) allows you to toggle the left (navigation) and right (table of contents) sidebars on a couple of MkDocs themes such as Material for MkDocs.
- [mkdocs-towncrier](https://github.com/davfsa/mkdocs-towncrier) An insanely small plugin to add towncrier changelog draft into mkdocs.
- [mkdocs-ultralytics-plugin](https://github.com/ultralytics/mkdocs) enhances your MkDocs-generated documentation with advanced Search Engine Optimization (SEO) features, interactive social elements, and structured data support. It automates the generation of essential meta tags, incorporates social sharing capabilities, and adds JSON-LD structured data to elevate user engagement and improve your Markdown project's visibility on the web.
- [mkdocs-video](https://github.com/soulless-viewer/mkdocs-video) allows you to embed videos on the documentation pages using a simple Markdown syntax.
- [mkdocs-wavesurfer](https://github.com/aeskildsen/mkdocs-wavesurfer) that adds a waveform display for `<audio>` elements using wavesurfer.js.
- [mkdocs-webcontext-plugin](https://github.com/darrelk/mkdocs-webcontext-plugin) MkDocs assumes absolute paths start from the root of the hosted website, like http://localhost/. For example, an absolute path like /assets/image1.jpg becomes http://localhost/assets/image1.jpg, which is correct if MkDocs is hosted at the root.When the server root is not the same as the MkDocs root, this plugin lets you define a webcontext to prepend to these absolute paths. The webcontext path (e.g., /projectname/documents) replaces the default root (/).
- [mkdocs-wikilinks-plugin](https://github.com/UtilityWorlds/mkdocs-wikilinks-plugin) for mkdocs which enables easier linking between pages.
- [mkdocs-wikipedia](https://github.com/yves-chevallier/mkdocs-wikipedia) allows you to fetch and display Wikipedia summaries in your MkDocs pages. It is compatible with MkDocs Material and MkDocs Books.
- [mkdocs-with-confluence](https://github.com/pawelsikora/mkdocs-with-confluence/) Plugin for uploading markdown documentation to Confluence via Confluence REST API
- [mkdocs-zip-folders](https://github.com/JakubAndrysek/mkdocs-zip-folders) is used to create archives (zip and tar.gz) of specified folders in your MkDocs project after the site build process. This can be helpful if you need to distribute or backup parts of your documentation.
- [Mkdocstrings](https://mkdocstrings.github.io/) automatic documentation from sources.

### Markdown extension

- [Breakless Lists Markdown Extension](https://github.com/adamb70/mdx-breakless-lists) Use lists without requiring a line break above them.
- [Customblocks](https://github.com/vokimon/markdown-customblocks) settles a common markup for parametrizable and nestable components.
- [Include](https://github.com/cmacmackin/markdown-include/) allows the inclusion of the contents of other Markdown documents.
- [Mdx Truly Sane Lists](https://github.com/radude/mdx_truly_sane_lists) that makes lists truly sane. Features custom indents for nested lists and fix for messy linebreaks and paragraphs between lists.
- [Pygments](http://pygments.org/) is a generic syntax highlighter.
- [PyMdown Extensions](https://facelessuser.github.io/pymdown-extensions/) is a collection of extensions for Python Markdown.

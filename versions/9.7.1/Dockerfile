# Build Stage
FROM python:3.14.2-slim AS builder

# Environment variables
ENV PACKAGES=/usr/local/lib/python3.14/site-packages
ENV PYTHONDONTWRITEBYTECODE=1

# Set build directory
WORKDIR /build

# Perform build and cleanup artifacts and caches
RUN apt-get update && apt-get install -y \
    gcc \
    g++ \
    tini \
    && rm -rf /var/lib/apt/lists/*

RUN pip install --no-cache-dir --upgrade pip && \
    pip install --no-cache-dir \
        anyio==4.12.0 \
        babel==2.17.0 \
        backrefs==6.1 \
        beautifulsoup4==4.14.3 \
        bleach==6.3.0 \
        bleach-allowlist==1.0.3 \
        bracex==2.6 \
        brotli==1.2.0 \
        certifi==2025.11.12 \
        cffi==2.0.0 \
        charset-normalizer==3.4.4 \
        click==8.2.1 \
        colorama==0.4.6 \
        coverage==7.13.0 \
        csscompressor==0.9.5 \
        cssselect2==0.8.0 \
        dacite==1.9.2 \
        decorator==5.2.1 \
        defusedxml==0.7.1 \
        essentials==1.1.9 \
        essentials-openapi==1.3.0 \
        fonttools==4.61.1 \
        future==1.0.0 \
        geocoder==1.38.1 \
        ghp-import==2.1.0 \
        gitdb==4.0.12 \
        gitpython==3.1.45 \
        h11==0.16.0 \
        hjson==3.1.0 \
        htmlmin2==0.1.13 \
        httpcore==1.0.9 \
        httplib2==0.31.0 \
        httpx==0.28.1 \
        idna==3.11 \
        importlib-metadata==8.7.0 \
        importlib-resources==6.5.2 \
        iniconfig==2.3.0 \
        jinja2==3.1.6 \
        jsmin==3.0.1 \
        lxml==6.0.2 \
        markdown==3.10 \
        markdown-customblocks==1.5.4 \
        markdown-include==0.8.1 \
        markdown-it-py==4.0.0 \
        markupsafe==3.0.3 \
        mdurl==0.1.2 \
        mdx-breakless-lists==1.0.1 \
        mdx-truly-sane-lists==1.3 \
        mergedeep==1.3.4 \
        mike==2.1.3 \
        mkdocs==1.6.1 \
        mkdocs-abs-rel-plugin==0.2.4 \
        mkdocs-add-number-plugin==1.2.2 \
        mkdocs-autolinks-plugin==0.7.1 \
        mkdocs-autorefs==1.4.3 \
        mkdocs-awesome-pages-plugin==2.10.1 \
        mkdocs-breadcrumbs-plugin==0.1.14 \
        mkdocs-build-plantuml-plugin==1.11.0 \
        mkdocs-categories-plugin==0.5.0 \
        mkdocs-cinder==1.2.0 \
        mkdocs-codeinclude-plugin==0.2.1 \
        mkdocs-drawio==1.12.1 \
        mkdocs-embed-external-markdown==3.0.2 \
        mkdocs-enumerate-headings-plugin==0.6.2 \
        mkdocs-exclude==1.0.2 \
        mkdocs-exclude-search==0.6.6 \
        mkdocs-exclude-unused-files==1.4.1 \
        mkdocs-extract-listings-plugin==0.2.1 \
        mkdocs-gallery==0.10.4 \
        mkdocs-gemini-chatbot==1.0.1 \
        mkdocs-gen-files==0.6.0 \
        mkdocs-get-deps==0.2.0 \
        mkdocs-git-authors-plugin==0.10.0 \
        mkdocs-git-committers-plugin-2==2.5.0 \
        mkdocs-git-revision-date-localized-plugin==1.5.0 \
        mkdocs-img2fig-plugin==0.9.3 \
        mkdocs-include-markdown-plugin==7.2.0 \
        mkdocs-kroki-plugin==1.1.0 \
        mkdocs-link-marker==0.2.0 \
        mkdocs-literate-nav==0.6.2 \
        mkdocs-localsearch==0.9.2 \
        mkdocs-macros-plugin==1.5.0 \
        mkdocs-markdownextradata-plugin==0.2.6 \
        mkdocs-material==9.7.1 \
        mkdocs-material-extensions==1.3.1 \
        mkdocs-merge==0.11.0 \
        mkdocs-minify-plugin==0.8.0 \
        mkdocs-monorepo-plugin==1.1.2 \
        mkdocs-multirepo==0.5.2 \
        mkdocs-multirepo-plugin==0.8.3 \
        mkdocs-nav-weight==0.3.0 \
        mkdocs-no-sitemap-plugin==0.0.1 \
        mkdocs-print-site-plugin==2.8 \
        mkdocs-publish-control==0.1.2 \
        mkdocs-publisher==1.4.8 \
        mkdocs-puml==2.1.0 \
        mkdocs-pymdownx-material-extras==2.8 \
        mkdocs-redirects==1.2.2 \
        mkdocs-ruby-plugin==0.0.3 \
        mkdocs-safe-text-plugin==1.6.1 \
        mkdocs-same-dir==0.1.3 \
        mkdocs-section-index==0.3.10 \
        mkdocs-simple-hooks==0.1.5 \
        mkdocs-simple-plugin==3.2.4 \
        mkdocs-swagger-ui-tag==0.7.2 \
        mkdocs-table-of-figures==0.5.7 \
        mkdocs-toggle-sidebar-plugin==0.0.9 \
        mkdocs-video==1.5.0 \
        mkdocstrings==1.0.0 \
        mkpdfs-mkdocs==1.0.1 \
        msgpack==1.1.2 \
        mypy-extensions==1.1.0 \
        natsort==8.4.0 \
        neoteroi-mkdocs==1.2.0 \
        packaging==25.0 \
        paginate==0.5.7 \
        pathspec==0.12.1 \
        pillow==12.0.0 \
        platformdirs==4.5.1 \
        pluggy==1.6.0 \
        pycparser==2.23 \
        pydyf==0.12.1 \
        pygments==2.19.2 \
        pymdown-extensions==10.19.1 \
        pyparsing==3.2.5 \
        pyphen==0.17.2 \
        pytest==9.0.2 \
        pytest-cov==3.0.0 \
        python-dateutil==2.9.0.post0 \
        python-dotenv==1.2.1 \
        python-magic==0.4.27 \
        python-slugify==8.0.4 \
        pytz==2025.2 \
        pyyaml==6.0.3 \
        pyyaml-env-tag==1.1 \
        ratelim==0.1.6 \
        requests==2.32.5 \
        responses==0.25.8 \
        result==0.17.0 \
        rich==13.9.4 \
        ruamel-yaml==0.18.17 \
        ruamel-yaml-clib==0.2.15 \
        setuptools==80.9.0 \
        six==1.17.0 \
        smmap==5.0.2 \
        sniffio==1.3.1 \
        soupsieve==2.8.1 \
        super-collections==0.6.2 \
        termcolor==3.2.0 \
        text-unidecode==1.3 \
        tinycss2==1.5.1 \
        tinyhtml5==2.0.0 \
        tqdm==4.67.1 \
        typing-extensions==4.15.0 \
        typing-inspect==0.8.0 \
        urllib3==2.6.2 \
        verspec==0.1.0 \
        watchdog==6.0.0 \
        wcmatch==10.1 \
        weasyprint==67.0 \
        webencodings==0.5.1 \
        yamlns==0.12.2 \
        zipp==3.23.0 \
        zopfli==0.4.0

RUN find . -type d -name "__pycache__" -exec rm -rf {} + 2>/dev/null || true && \
    find . -type f -name "*.pyc" -delete && \
    rm -rf venv/ && \
    rm -rf .git/ && \
    rm -rf .pytest_cache/ && \
    rm -rf *.egg-info/ && \
    rm -rf .coverage && \
    rm -rf htmlcov/

# Runtime Stage
FROM python:3.14.2-slim AS runtime

# Copy all from builder
COPY --from=builder /usr/local/lib/python3.14/site-packages /usr/local/lib/python3.14/site-packages
COPY --from=builder /usr/local/bin /usr/local/bin
COPY --from=builder /usr/bin/tini /usr/bin/tini

# Set working directory
WORKDIR /docs

# Expose MkDocs development server port
EXPOSE 8000

# Shell
CMD ["/bin/sh"]
site_name: Ultimato Wiki
site_description: Wiki oficial do servidor Ultimato
site_author: Ultimato Network
language: pt-BR

theme:
  name: material
  language: pt-BR

  # Topo + navegação mais "site de produto"
  features:
    - navigation.instant
    - navigation.instant.progress
    - navigation.tabs
    - navigation.tabs.sticky
    - navigation.sections
    - navigation.top
    - navigation.footer
    - toc.follow
    - content.code.copy
    - content.code.annotate
    - content.tabs.link
    - search.suggest
    - search.highlight
    - search.share

  # Modo escuro + (opcional) toggle
  palette:
    - scheme: slate
      primary: deep purple
      accent: purple
      toggle:
        icon: material/weather-night
        name: Modo escuro

  font:
    text: Inter
    code: JetBrains Mono

  icon:
    logo: material/book-open-page-variant
    repo: fontawesome/brands/github

# Plugins (instalar abaixo)
plugins:
  - search:
      lang: pt
  - tags
  - git-revision-date-localized:
      enable_creation_date: true
      type: timeago
      locale: pt
  - minify:
      minify_html: true

markdown_extensions:
  - admonition
  - attr_list
  - footnotes
  - tables
  - toc:
      permalink: true
  - pymdownx.details
  - pymdownx.superfences
  - pymdownx.highlight:
      anchor_linenums: true
      line_spans: __span
  - pymdownx.inlinehilite
  - pymdownx.snippets
  - pymdownx.tabbed:
      alternate_style: true
  - pymdownx.emoji:
      emoji_index: !!python/name:material.extensions.emoji.twemoji
      emoji_generator: !!python/name:material.extensions.emoji.to_svg

extra_css:
  - stylesheets/extra.css

# (Opcional) deixa o site mais "brand"
extra:
  generator: false

nav:
  - Início: index.md
  - Comandos:
      - Comandos gerais: comandos/comandos.md
      - Sub comandos: comandos/subcomandos.md
  - Dúvidas Comum:
      - Geral: duvidascomum/duvidascomum.md
  - Guia:
      - Guia: guia/inicio.md
  - Mecânicas:
      - Frascos do tempo: mecanicas/frascosdotempo.md
      - Trades: mecanicas/trade.md
      - Vitrine: mecanicas/vitrine.md

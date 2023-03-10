```bash
hexo init blog
cd blog
yarn
yarn remove hexo-renderer-marked
yarn add hexo-renderer-markdown # with markdown-it-texmath
yarn add hexo-filter-kroki
yarn add markdown-it-multimd-table
```

```bash
yarn add hexo-renderer-pug hexo-theme-butterfly
```

```yml
## https://github.com/niemingzhao/hexo-renderer-markdown
markdown:
  plugins:
    markdown-it-texmath:
      texmathDelimiters: brackets
      #katexCssSrc: "//cdn.jsdelivr.net/npm/katex/dist/katex.min.css",
      #texmathCssSrc: "//cdn.jsdelivr.net/npm/markdown-it-texmath/css/texmath.min.css",
      #throwOnError: false,
      #errorColor: "#cc0000",
      #macros: { "\\RR": "\\mathbb{R}" },
    markdown-it-multimd-table:
      multiline: true
      rowspan: true
      #headerless: false
      #multibody:  true
      #aotolabel:  true
```

在 github pages 部署 `https://hexo.io/zh-cn/docs/github-pages.html`
```bash
touch .github/workflows/pages.yml
```
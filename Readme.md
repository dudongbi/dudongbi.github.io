一定记得把分支切换到 gh-pages 去 !!!

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

`_config.yml`
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

`.github/workflows/pages.yml` 参考 <https://hexo.io/zh-cn/docs/github-pages.html>

```yml
name: Pages

on:
  push:
    branches:
      - main # default branch

jobs:
  pages:
    runs-on: ubuntu-latest
    steps:
      - uses: actions/checkout@v3
      - name: Use Node.js 18
        uses: actions/setup-node@v3
        with:
          node-version: "18.14.2"
      - name: Cache NPM dependencies
        uses: actions/cache@v3
        with:
          path: node_modules
          key: ${{ runner.OS }}-npm-cache
          restore-keys: |
            ${{ runner.OS }}-npm-cache
      - name: Install Dependencies
        run: npm install
      - name: Build
        run: npm run build
      - name: Deploy
        uses: peaceiris/actions-gh-pages@v3
        with:
          github_token: ${{ secrets.GITHUB_TOKEN }}
          publish_dir: ./public
```

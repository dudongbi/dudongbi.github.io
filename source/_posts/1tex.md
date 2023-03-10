---
title: 1tex
date: 2022-12-27 11:25:03
tags: tex
---

# 基础设置

## tlmgr

https://blog.csdn.net/qq_41437512/article/details/113917059

```bash
tlmgr --repository http://www.texlive.info/tlgpg/ install tlgpg
tlmgr repository set https://mirrors.tuna.tsinghua.edu.cn/CTAN/systems/texlive/tlnet
tlmgr repository set https://mirror.bjtu.edu.cn/CTAN/systems/texlive/tlnet/
tlmgr repository set https://mirrors.ustc.edu.cn/CTAN/systems/texlive/tlnet/
```

```bash
tlmgr list --only-installed
tlmgr install --with-doc --with-src pdfcol psnfss minifp
# tlmgr install caption environ eso-pic fancyhdr listings tcolorbox comment lipsum lettrine
tlmgr install luacode ctex chinese-jfm layouts
tlmgr install glossaries listingsutf8
tlmgr install minitoc tocloft calligra pgfornament pgfopts fdsymbol
tlmgr install multirow paralist changepage grfext
tlmgr install physics bbding trfsigns esint zhlipsum boxedminipage
```

## `.gitignore`

```
*.pdf
*.ist
*.mtc
*.mykeylist
```

# Latex Workshop

https://zhuanlan.zhihu.com/p/38178015

## `.vscode/settings.json`
```json
{
    "files.associations": {
        "*.mmd": "markdown_latex_combined"
    },
    
    // 预览和正反向搜索
    "latex-workshop.view.pdf.viewer": "tab",
    "latex-workshop.view.pdf.internal.synctex.keybinding": "ctrl-click",

    // 禁止自动编译
    "latex-workshop.latex.autoBuild.run": "never",
    "latex-workshop.message.error.show": false,
    "latex-workshop.message.warning.show": false,

    // 工具
    "latex-workshop.latex.tools": [
        {
            "name": "lualatex",
            "command": "lualatex",
            "args": [
                "-synctex=1",
                "-interaction=nonstopmode",
                "-file-line-error",
                "-shell-escape", // <pkg>plantuml
                "%DOCFILE%"
            ]
        },
        {
            "name": "bibtex",
            "command": "bibtex",
            "args": [
                "%DOCFILE%"
            ]
        }
    ],

    // 工具链
    "latex-workshop.latex.recipes": [
        {
            "name": "lualatex",
            "tools": [
                "lualatex"
            ],
        },
        {
            "name": "lua->bib->lua->lua",
            "tools": [
                "lualatex",
                "bibtex",
                "lualatex",
                "lualatex"
            ]
        },
    ],
}
```

## `.vscode/keybinding.json`
```json
[
    {
        "key": "ctrl+l alt+b",
        "command": "latex-workshop.build",
        "when": "config.latex-workshop.bind.altKeymap.enabled && !virtualWorkspace && editorLangId =~ /latex|latex-expl3|rsweave|jlweave/"
    },
    {
        "key": "ctrl+l alt+c",
        "command": "latex-workshop.clean",
        "when": "config.latex-workshop.bind.altKeymap.enabled && !virtualWorkspace && editorLangId =~ /latex|latex-expl3|rsweave|jlweave/"
    },
    {
        "key": "ctrl+l alt+v",
        "command": "latex-workshop.view",
        "when": "config.latex-workshop.bind.altKeymap.enabled && !virtualWorkspace && editorLangId =~ /latex|latex-expl3|rsweave|jlweave/"
    },
    {
        "key": "ctrl+l alt+j",
        "command": "latex-workshop.synctex",
        "when": "config.latex-workshop.bind.altKeymap.enabled && editorTextFocus && !virtualWorkspace && editorLangId == 'latex'"
    },
    {
        "key": "ctrl+l alt+r",
        "command": "latex-workshop.recipes",
        "when": "config.latex-workshop.bind.altKeymap.enabled && !virtualWorkspace && editorLangId =~ /latex|latex-expl3|rsweave|jlweave/"
    }
]
```

latex-workshop.tab

ctrl+l_alt+b: latex-workshop.build
ctrl+l_alt+c: latex-workshop.clean
ctrl+l_alt+v: latex-workshop.view
ctrl+l_alt+j: latex-workshop.synctex

# Usage

## Math

```tex
% 行内环境使用大符号
\everymath{\displaystyle}
```

# LyX

## 文档首选项

1. 文档类：CTeX

2. 字体：使用非 LaTeX 字体

3. 输出格式：

    * PDF（LuaLaTeX）

    * 允许运行外部程序

4. 程序列表

```tex
%行号
numbers=left,
%背景框
framexleftmargin=10mm,
frame=none,
%背景色
backgroundcolor=\color[RGB]{245,245,244},
%样式
keywordstyle=\bf\color{blue},
identifierstyle=\bf,
numberstyle=\color[RGB]{0,192,192},
commentstyle=\it\color[RGB]{0,96,96},
stringstyle=\rmfamily\slshape\color[RGB]{128,0,0},
%显示空格
showstringspaces=true,
xleftmargin=2em,
%边距
xrightmargin=2em,
aboveskip=1em
```

5. 导言区

```tex
\usepackage{shellesc}
\usepackage{graphicx}
```

## 网络图片

LuaLaTeX下载文件

```tex
% https://blog.csdn.net/yifan_lym/article/details/49588669 # 基本
% https://blog.csdn.net/qq_21949217/article/details/42779093 # 高级
% https://blog.csdn.net/x_iya/article/details/51494172 # 最终方案
\begin{luacode}
local http = require("socket.http")
local ltn12 = require("ltn12")
function download(dst, url)
    local req_body = ""
    local resp_body = {}
    local r, code, resp_headers = assert(http.request{
        url = url,
        method = "GET",
        headers = {
            ["Content-Length"] = #req_body
        },
        source = ltn12.source.string(req_body),
        sink = ltn12.sink.table(resp_body),
    })
    if "table" == type(resp_body) then
        tex.sprint("下载文件成功" .. code .. table.concat(resp_headers))
        local f = io.open(dst, "w+")
        f:write( table.concat(resp_body) )
        f:close()
    else
        tex.sprint("下载文件失败")
    end
end
\end{luacode}
```

直链，luatex 里是 `\ShellEscape` 而非 `\write18`

```tex
\documentclass{ctexart}
\usepackage{luacode}
\usepackage{graphicx} % svg, ifplatform, catchfile, transparent, l3experimental
\usepackage{shellesc}
\begin{document}
\ShellEscape{ curl -o 1.png https://kroki.io/graphviz/png/eNpLyUwvSizIUHBXqPZIzcnJ17ULzy_KSanlAgB1EAjQ }
\includegraphics{1.png}
\end{document}
```

## LaTeX -> LyX 乱码

https://tieba.baidu.com/p/3386581480

LyX 首选项

文件转换 转换器 LaTeX -> LyX

tex2lyx -f $$i $$o

tex2lyx -f -e "utf8" $$i $$o
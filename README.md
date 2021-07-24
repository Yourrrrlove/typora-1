<img src="https://i.snap.as/rjd6QGVp.png" alt="Typora Logo Version 2" style="zoom:33%;" />

![GitBook Slate](capture/GitBookSlate.png)

# My Darling, Typora (David Blue's Typora Configuration)

### This repo is my personal collection of themes/tricks/snippets/configuration files for Typora on Windows 10. It is *not* associated with Typora's ongoing development in any way.

I have found my perfect word processing solution. I have much to say about it, eventually, but for now, I want to share instructions you can follow that should result in you having *precisely* the same experience:

1. Download and install the latest [64-bit version](https://typora.io/#windows) for Windows.
2. Run Typora, open Preferences `Ctrl + ,` → Appearance and find "Open Themes Folder" near the bottom.
3. Download the .zip file of the GitBook theme's [latest release](https://github.com/h16nning/typora-gitbook-theme/releases/latest) and extract it to the themes folder. (As in, you should be adding one directory `/GitBook` to the themes folder along with 3 .css files.)







### My Custom Keybinds

| Action                                                  | Input            |
| ------------------------------------------------------- | ---------------- |
| Highlight selected text                                 | Ctrl + Shift + H |
| Transform selected text into Markdown pullquote `>`     | Alt + Q          |
| Show/hide legacy menu items                             | Alt + P          |
| ~~Always on Top~~                                       | Ctrl + Shift + P |
| Transform selected text into Markdown task list `- [ ]` | Ctrl + Shift + T |



```json
"keyBinding": {
    "Highlight": "Ctrl+Shift+H"
    "Quote": "Alt+Q"
    "PrintDialog:": "Alt+P"
    "Always on Top": "Ctrl+Shift+P"
    "Task List": "Ctrl+Shift+T"
},
```







<img src="https://user-images.githubusercontent.com/43663476/126875727-a314692c-76da-4803-852e-84e319098ce4.png" width="45%"></img> <img src="https://user-images.githubusercontent.com/43663476/126875730-465e8581-6ebd-4b45-ab11-b24bb1f6819d.png" width="45%"></img> <img src="https://user-images.githubusercontent.com/43663476/126875731-86461bcd-cfa0-4a59-b580-bd6e2aa2c897.png" width="45%"></img> <img src="https://user-images.githubusercontent.com/43663476/126875735-753f4924-abf2-4a4b-9d9d-9b208f302192.png" width="45%"></img> <img src="https://user-images.githubusercontent.com/43663476/126875739-5742bc27-4a52-41a2-9ff7-838f74bf0c8a.png" width="45%"></img> <img src="https://user-images.githubusercontent.com/43663476/126875740-72de1b56-93d5-48dd-a819-73d001e280ba.png" width="45%"></img> <img src="https://user-images.githubusercontent.com/43663476/126875741-8ab0b94f-00ed-445a-9304-0bc066cd60f1.png" width="45%"></img> <img src="https://user-images.githubusercontent.com/43663476/126875742-058e9307-2620-49a8-91d7-9369ad3b957a.png" width="45%"></img> 

* [**My conf.user.json file**](https://gist.github.com/extratone/bda30d19e18cd70de2fafcbde5e3322d) in GitHub Gist form. (Embedded below.)
* [**GitHub Issue**](https://github.com/extratone/bilge/issues/11) for my upcoming (and ridiculously long-awaited) "review" of Typora around 1.0's release
* GitBook theme's [Theme Library page](https://theme.typora.io/theme/Gitbook/).

<script src="https://gist.github.com/extratone/bda30d19e18cd70de2fafcbde5e3322d.js"></script>





`![Typora Tile](https://i.snap.as/3vbelEU.png)`

`https://github.com/h16nning/typora-gitbook-theme/discussions/29`

## General Resources

* [Typora Theme Gallery](https://theme.typora.io/) (Web)



***

### [GitBook Slate CSS](https://github.com/h16nning/typora-gitbook-theme/blob/main/src/gitbook-slate.css)

```css
@import "gitbook/fonts.css";
@import "gitbook/slate-colors.css";

/*by 16soundsofsilence, yes this code is an absolute mess*/

html,
.form-control,
.modal {
    font-size: 16px;
}

body {
    background: var(--bg-color);
    font-family: var(--font-family);
    font-weight: 400;
    color: white;
    line-height: 1.6rem;
    height: 100%;
}

#write {
    font-size: 0.95rem;
    max-width: 850px;
    margin: 0 auto;
    margin-top: 1rem;
    padding: 30px;
    padding-bottom: 100px;
    position: static;
    width: 100%;
}

#write > ul:first-child,
#write > ol:first-child {
    margin-top: 30px;
}

a {
    color: var(--primary-color);
    text-decoration: none !important;
    transition-duration: 0.2s;
    transition-property: color;
}

a:hover {
    color: var(--primary-color-darker);
}

mark a,
mark .md-content.md-url {
    color: var(--primary-color-darker2);
}

mark a:hover {
    color: var(--primary-color-darkest);
}

.ty-preferences a {
    color: var(--primary-color);
}

h1,
h2,
h3,
h4,
h5,
h6 {
    position: relative;
    color: var(--heading-text-color);
    cursor: text;
}

h1:hover a.anchor,
h2:hover a.anchor,
h3:hover a.anchor,
h4:hover a.anchor,
h5:hover a.anchor,
h6:hover a.anchor {
    text-decoration: none;
}

h1 tt,
h1 code {
    font-size: inherit;
}

h2 tt,
h2 code {
    font-size: inherit;
}

h3 tt,
h3 code {
    font-size: inherit;
}

h4 tt,
h4 code {
    font-size: inherit;
}

h5 tt,
h5 code {
    font-size: inherit;
}

h6 tt,
h6 code {
    font-size: inherit;
}

h1 {
    font-size: 2.2rem;
    font-weight: 700;
    line-height: 1.5;
    margin-top: 3rem;
    margin-bottom: 0.5rem;
    padding-bottom: 0.2rem;
    border-bottom: solid 1px var(--borders);
}

h2 {
    font-size: 1.7rem;
    font-weight: 700;
    line-height: 1.5;
    margin-top: 2rem;
    margin-bottom: 0.5rem;
}

h3 {
    font-size: 1.375rem;
    font-weight: 700;
    line-height: 1.5;
    margin-top: 1.5rem;
    margin-bottom: 0.5rem;
}

h4 {
    font-size: 1.15rem;
    font-weight: 700;
    line-height: 1.5;
    margin-top: 1.5rem;
    margin-bottom: 0.5rem;
}

h5 {
    font-size: 0.95rem;
    font-weight: 700;
    line-height: 1.5;
    margin-top: 1.5rem;
    margin-bottom: 0.5rem;
}

h6 {
    font-size: 0.95rem;
    font-weight: 400;
    line-height: 1.5;
    margin-top: 1.5rem;
    margin-bottom: 0.5rem;
}

#write > h1.md-focus:before,
#write > h2.md-focus:before,
#write > h3.md-focus:before,
#write > h4.md-focus:before,
#write > h5.md-focus:before,
#write > h6.md-focus:before {
    color: var(--light-text-color);
    border: none;
    position: absolute;
    font-size: 0.9rem;
    font-weight: 500;
    padding: 0px;
    line-height: 1;
}

#write > h1.md-focus:before {
    content: "h1";
    top: 1.15rem;
    left: -1.75rem;
}

#write > h2.md-focus:before {
    content: "h2";
    top: 0.75rem;
    left: -1.75rem;
}

#write > h3.md-focus:before {
    content: "h3";
    top: 0.575rem;
    left: -1.75rem;
}

#write > h4.md-focus:before {
    content: "h4";
    top: 0.4rem;
    left: -1.75rem;
}

#write > h5.md-focus:before {
    content: "h5";
    top: 0.25rem;
    left: -1.75rem;
}

#write > h6.md-focus:before {
    content: "h6";
    top: 0.25rem;
    left: -1.75rem;
}

h1:first-child,
h2:first-child,
h3:first-child,
h4:first-child,
h5:first-child,
h6:first-child,
blockquote h1,
blockquote h2,
blockquote h3,
blockquote h4,
blockquote h5,
blockquote h6 {
    margin-top: 0rem;
}

p,
blockquote,
ul,
ol,
dl {
    margin: 0.5rem 0rem 1.5rem 0rem;
}

li > ol,
li > ul {
    margin: 0 0;
}

hr {
    height: 1px;
    padding: 0;
    margin: 16px 0;
    background-color: var(--borders);
    border: 0 none;
    overflow: hidden;
    box-sizing: content-box;
}

li p.first {
    display: inline-block;
}

ul,
ol {
    padding-left: 30px;
}

ul:first-child,
ol:first-child {
    margin-top: 0;
}

ul:last-child,
ol:last-child {
    margin-bottom: 0;
}

.md-blockmeta {
    color: var(--md-char-color);
}

mark {
    background-color: var(--primary-color);
    color: white;
    padding: 0.2rem 0.4rem;
    border-radius: 0.2rem;
    box-decoration-break: clone;
    -webkit-box-decoration-break: clone;
}

/*BLOCKQUOTE*/

blockquote {
    width: 100%;
    background-color: var(--boxes);
    border-left: 4px solid var(--primary-color);
    border-radius: 0.3em;
    padding: 1rem;
}

blockquote blockquote {
    padding-right: 0;
}

table {
    font-size: 0.875rem;
    padding: 0;
    margin: 1.5rem 0;
    word-break: initial;
}

/*TABLE*/

table tr {
    border-top: 1px solid var(--borders);
    border-bottom: 1px solid var(--borders);
    margin: 0;
    padding: 0;
}

table tr.md-end-block {
    border-top: none;
}

table tbody tr:last-child {
    border-bottom: none;
}

table tr th {
    font-weight: bold;
    border: none;
    border-bottom: solid 2px var(--borders);
    margin: 0;
    padding: 10px 16px;
    transition-duration: 0.1s;
    transition-property: background-color;
}

table tr td {
    border: none;
    margin: 0;
    padding: 10px 16px;
    transition-duration: 0.1s;
    transition-property: background-color;
}

#write table tr td:hover,
#write table tr th:hover {
    background-color: var(--boxes);
}

table tr th:first-child,
table tr td:first-child {
    margin-top: 0;
}

table tr th:last-child,
table tr td:last-child {
    margin-bottom: 0;
}

/*OTHER TABLE THINGS*/

.ty-table-edit {
    background-color: var(--boxes);
    padding: 0.3rem;
    border-radius: 0.3rem;
    box-shadow: none;
    transform: translateY(2.5rem);
    transition-duration: 0.3s;
    transition-property: opacity;
}

.ty-table-edit + .md-table {
    margin-top: 3rem;
}

.ty-table-edit:active,
.ty-table-edit:focus {
    box-shadow: none;
}

.popover,
.popover:active,
.popover:focus {
    border: solid 1px var(--borders);
    box-shadow: rgba(0, 0, 0, 0.2) 0px 3px 8px 0px;
    border-radius: 0.3rem;
}

.popover .arrow {
    border-bottom-color: var(--borders);
}

.md-grid-board a {
    background-color: transparent;
    border-color: var(--borders);
    border-radius: 2px;
}

.md-grid-board .md-grid-ext {
    background-color: var(--borders);
    border-radius: 2px;
}

.md-grid-board tr[row="1"] .md-grid-ext {
    background: none;
    border-radius: 6px;
}

.md-grid-board tr[row="1"] .md-grid-ext a {
    background-color: var(--boxes-darker2);
    border-color: var(--boxes-darker2);
}

.md-grid-board tr[row="1"] td {
    background-color: var(--bg-color);
    border-color: var(--borders);
}

.md-grid-board a.md-active,
.md-grid-board a:hover {
    background-color: var(--primary-color);
    border-color: var(--primary-color);
}

.md-grid-board tr[row="1"] a.md-active,
.md-grid-board tr[row="1"] a:hover {
    background-color: var(--primary-color-darker);
    border-color: var(--primary-color-darker);
}

#md-grid-width,
#md-grid-height {
    border-radius: 0.3rem;
    border-color: var(--borders);
    transition-duration: 0.3s;
    transition-property: border-color;
}

#md-grid-width:focus,
#md-grid-height:focus {
    border-radius: 0.3rem;
    border-color: var(--primary-color);
}

/*CODE*/

.CodeMirror {
    padding: 1rem;
    font-family: var(--code-font-family);
}

.cm-s-inner .CodeMirror-gutters {
    background-color: none;
    border-right: none;
    border-radius: 0px;
    width: 2rem;
    color: white;
    height: 100%;
    white-space: nowrap;
    overflow: hidden;
}

.cm-s-inner .CodeMirror-gutter-wrapper {
    left: -2.75rem !important;
}

.CodeMirror.cm-s-typora-default div.CodeMirror-cursor {
    border-left: solid 2px var(--light-text-color-brighter);
}

.CodeMirror.cm-s-typora-default .CodeMirror-activeline-background {
    background-color: var(--codeboxes-lighter);
}

.cm-s-inner .CodeMirror-cursor {
    color: white;
    border-left: solid 1px white;
}

.CodeMirror-linenumber {
    color: white;
    opacity: 0.6;
    width: 1.9532rem !important /*required*/;
}

.cm-s-inner .CodeMirror-line::selection,
.cm-s-inner .CodeMirror-line::-moz-selection,
.cm-s-inner .CodeMirror-line > span::selection,
.cm-s-inner .CodeMirror-line > span::-moz-selection,
.cm-s-inner .CodeMirror-line > span > span::selection,
.cm-s-inner .CodeMirror-line > span > span::-moz-selection {
    background-color: rgba(255, 255, 255, 0.1);
}

.cm-error {
    color: var(--danger-color);
}

.cm-s-inner span.cm-comment,
.cm-s-typora-default span.cm-comment,
.cm-s-typora-default span.cm-code {
    color: #9daab6;
}

.cm-s-inner span.cm-string,
.cm-s-inner span.cm-string-2 {
    color: #71a7ff;
}

.cm-s-inner span.cm-number {
    color: #ff9d3d;
}

.cm-s-inner span.cm-variable,
.cm-s-inner span.cm-variable-2 {
    color: white;
}

.cm-s-inner span.cm-def {
    color: white;
}

.cm-s-inner span.cm-operator {
    color: #ff9d3d;
}

.cm-s-inner span.cm-keyword {
    color: #61e3a5;
}

.cm-s-inner span.cm-atom {
    color: #bd93f9;
}

.cm-s-inner span.cm-meta {
    color: #f8f8f2;
}

.cm-s-inner span.cm-link,
.cm-s-typora-default .cm-link {
    color: var(--primary-color);
}

.cm-s-inner span.cm-tag,
.cm-s-inner .cm-header {
    color: #b4f6d6;
}

.cm-s-inner span.cm-attribute {
    color: #ff9d3d;
}

.cm-s-inner span.cm-qualifier,
.cm-s-inner span.cm-type,
.cm-s-inner span.cm-variable-3 {
    color: #82ee9d;
}

.cm-s-inner span.cm-property {
    color: #ffd6ad;
}

.cm-s-inner span.cm-builtin {
    color: #8ffaaa;
}

.md-fences.md-focus .cm-s-inner .CodeMirror-activeline-background {
    background: none;
}

.cm-s-inner .CodeMirror-selected,
.cm-s-inner .CodeMirror-selectedtext {
    background-color: rgba(255, 255, 255, 0.1);
}

.cm-s-typora-default .cm-header,
.cm-s-typora-default .cm-property {
    color: white;
    font-weight: 400;
}

.md-fences .code-tooltip {
    box-shadow: rgba(0, 0, 0, 0.2) 0px 3px 8px 0px;
    border: solid 1px var(--borders);
    border-radius: 0.3rem;
    background-color: var(--bg-color);
    color: var(--text-color);
    width: 15rem;
    height: 2.5rem;
    bottom: -3rem;
    padding: 0.1875rem;
}

.md-fences .code-tooltip .ty-input {
    border: solid 1px var(--borders);
    height: 2rem;
    line-height: 2rem;
    margin: 0rem;
    padding-left: 0.5rem !important;
    text-align: left;
    display: block;
    font-size: 0.8rem;
    font-weight: 600;
    font-family: var(--font-family);
    transition-duration: 0.3s;
    transition-property: border;
}

.md-fences .code-tooltip .ty-input:focus {
    border-color: var(--primary-color);
}

.html-for-mac .ty-cm-lang-input:empty:after {
    left: 0.5rem;
}

.autoComplt-list li,
.fences-auto-suggest li {
    font-weight: 500;
    transition-duration: 0.3s;
    transition-property: background-color, color;
}

.autoComplt-list li.active,
.fences-auto-suggest li:hover {
    background-color: var(--boxes);
    color: var(--primary-color);
}

.md-fences,
tt {
    border-radius: 0.3rem;
    color: #ffffff;
    padding: 1.5rem;
    font-size: 0.8rem;
}

code {
    padding: 0.2rem 0.4rem;
    background-color: var(--borders);
    font-size: 0.9rem;
    border-radius: 0.2rem;
    box-decoration-break: clone;
    -webkit-box-decoration-break: clone;
}

.md-fences .CodeMirror div.CodeMirror-cursor,
.md-htmlblock-panel .CodeMirror div.CodeMirror-cursor,
#typora-source div.CodeMirror-cursor {
    border-left: solid 1px white;
}

.md-fences {
    margin-bottom: 1.5rem;
    margin-top: 1.5rem;
    padding-top: 8px;
    padding-bottom: 6px;
    background-color: var(--codeboxes);
}

#typora-source {
    background-color: var(--codeboxes);
    color: white;
    font-size: 0.9rem;
}

/*DIAGRAMS*/

.md-diagram-panel {
    color: var(--text-color);
    border: solid 1px var(--borders);
    border-radius: 0.3rem;
}

.md-diagram-panel text,
.md-diagram-panel .label {
    color: var(--text-color);
}

.md-diagram-panel text {
    fill: var(--text-color) !important /*required*/;
}

.md-diagram-panel-error {
    color: var(--danger-color);
}
/*CHECKBOXES*/

.md-task-list-item > input:before,
input[type="checkbox"]:before {
    border-radius: 0.2rem;
    margin-top: -0.08rem;
    margin-left: -0.1rem;
    width: 1rem;
    height: 1rem;
    background-color: var(--borders);
    content: " ";
    display: block;
    transition-duration: 0.3s;
    transition-property: background-color;
}

.md-task-list-item:hover > input:before,
input[type="checkbox"]:hover:before {
    background-color: var(--boxes-darker);
}

.md-task-list-item > input:checked:before,
.md-task-list-item > input[checked]:before,
input[type="checkbox"]:checked:before {
    background-color: var(--primary-color);
}

.md-task-list-item:hover > input:checked:before,
.md-task-list-item:hover > input[checked]:before,
input[type="checkbox"]:hover:checked:before {
    background-color: var(--primary-color-darker);
}

.md-task-list-item > input:after,
.md-task-list-item > input:after,
input[type="checkbox"]:after {
    transform: rotate(-45deg);
    position: absolute;
    border: 2px solid white;
    border-top: 0;
    border-right: 0;
    top: 0.16rem;
    left: 0.1rem;
    width: 0.6rem;
    height: 0.375rem;
    content: " ";
    opacity: 0;
    transition-duration: 0.3s;
    transition-property: opacity;
}

.md-task-list-item > input:checked:after,
.md-task-list-item > input[checked]:after,
input[type="checkbox"]:checked:after {
    opacity: 1;
}

.ty-preferences input[type="checkbox"]:before {
    width: 1.2rem;
    height: 1.2rem;
}

.ty-preferences input[type="checkbox"]:after {
    width: 0.5rem;
    height: 0.32rem;
    top: 0.19rem;
    left: 0.14rem;
}

@media print {
    html {
        font-size: 13px;
    }

    table,
    pre {
        page-break-inside: avoid;
    }

    pre {
        word-wrap: break-word;
    }
}

#write pre.md-meta-block {
    padding: 1rem;
    line-height: 1.45;
    background-color: var(--boxes);
    border: 0;
    border-radius: 0.3rem;
    color: var(--text-color);
    border-left: solid 4px var(--boxes-darkest);
}

#write pre.md-meta-block:empty:before {
    color: var(--light-text-color);
}

.md-image > .md-meta {
    border-radius: 3px;
    padding: 2px 0px 0px 4px;
    font-size: 0.9em;
    color: inherit;
}

.md-tag {
    color: var(--md-char-color);
    opacity: 1;
}

/*TOC*/

.md-toc {
    margin: 1.5rem 0rem;
}

.md-toc:focus .md-toc-content {
    border: none;
}

#write div.md-toc-tooltip {
    background-color: var(--boxes);
    line-height: 1.6rem;
    padding: 0.3rem 0.75rem;
    border-top: none;
    border-radius: 0.3rem;
}

.md-toc.md-focus {
    margin-top: 4.5rem;
}

#write div.md-toc-tooltip + .md-toc-content {
    padding-top: 1rem;
}

.md-delete-toc {
    padding: 0px;
}

/*MATH*/

.md-rawblock-container {
    padding: 1rem;
    border-radius: 0.3rem;
    cursor: pointer;
    transition-duration: 0.2s;
}

.md-rawblock:hover .md-rawblock-container {
    background-color: var(--boxes);
}

.md-rawblock:active .md-rawblock-container {
    background-color: var(--boxes-darker);
}

.MathJax_SVG:focus {
    outline: none;
}

.md-rawblock-panel,
.md-rawblock-control:not(.md-rawblock-tooltip) {
    border-radius: 0.3rem;
    background-color: var(--boxes);
}

.md-rawblock-panel .code-tooltip {
    box-shadow: none;
    border-bottom-left-radius: 0.3rem;
    border-bottom-right-radius: 0.3rem;
}

.md-rawblock-panel .CodeMirror-linenumber {
    color: var(--light-text-color);
    opacity: 1;
}

.md-rawblock-panel .CodeMirror div.CodeMirror-cursor {
    border-left: solid 1px var(--text-color);
}

.md-mathblock-panel .md-mathjax-preview,
.mathjax-candidate {
    border-top: solid 1px var(--borders);
}

.md-rawblock-after,
.md-rawblock-before {
    cursor: default;
    color: var(--light-text-color);
    user-select: none;
    -webkit-user-select: none;
}

.md-rawblock-tooltip-name {
    font-size: 13px;
    color: var(--light-text-color);
    opacity: 1;
}

.md-rawblock-on-edit > .md-rawblock-tooltip {
    padding-right: 0px;
}

.md-rawblock-input span.cm-tag {
    color: #0bb6ad;
}

.md-rawblock-input span.cm-atom,
.md-inline-math script {
    color: #b61ed4;
}

.md-rawblock-input span.cm-number {
    color: #ec7200;
}

.md-rawblock-input span.cm-keyword {
    color: #156db6;
}

.md-mathblock-input span.cm-bracket {
    color: var(--light-text-color);
}

.code-tooltip.md-hover-tip {
    border-radius: 0.3rem;
    background-color: var(--bg-color);
    box-shadow: (0, 0, 0, 0.2) 0px 3px 8px 0px;
    color: var(--text-color);
    opacity: 1;
}

#math-inline-preview.code-tooltip .code-tooltip-content {
    border: solid 1px var(--borders);
}

#math-inline-preview.code-tooltip .md-arrow:after {
    background-color: var(--bg-color);
    border: solid 1px var(--borders);
    box-shadow: none;
}

/*FOOTER*/

.footer-item {
    opacity: 1 !important;
    color: var(--light-text-color);
    transition: 0.3s;
    background: none !important;
}

.footer-item:hover {
    color: var(--light-text-color-brighter) !important;
}

#outline-btn:hover {
    color: var(--light-text-color-brighter) !important;
}

/*SIDEBAR*/

#typora-sidebar {
    border-right: solid 1px var(--borders);
}

.info-panel-tab {
    opacity: 1;
}

.sidebar-tab {
    text-transform: capitalize;
    color: var(--light-text-color);
}

.info-panel-tab-border {
    color: var(--primary-color);
    border-radius: 2px;
}

#ty-sidebar-search-back-btn {
    margin: auto;
}

.ty-show-outline-filter #file-library-search,
.ty-show-search #file-library-search {
    height: 4rem;
}

#file-library-search-input {
    height: 2rem;
}

#file-library-search-panel input {
    margin-top: 8px !important;
}

.ty-sidebar-search-panel .searchpanel-search-option-btn,
#ty-sidebar-search-tabs .searchpanel-search-option-btn {
    top: 15px;
}

#typora-sidebar #filesearch-case-ion-btn,
#typora-sidebar #filesearch-word-ion-btn {
    background: none;
    margin-top: 0.45rem;
    transition-duration: 0.2s;
    transition-property: background-color;
}

#typora-sidebar #filesearch-case-ion-btn:hover,
#typora-sidebar #filesearch-word-ion-btn:hover {
    color: var(--primary-color);
}

/*sidebar loading*/

#typora-sidebar #sidebar-loading-template {
    padding: 0px;
}

#typora-sidebar #sidebar-loading-template .typora-search-spinner {
    opacity: 1;
    color: var(--light-text-color-darker);
}

#typora-sidebar #sidebar-loading-template .typora-quick-open-info {
    color: var(--light-text-color-darker);
    font-size: 0.9rem;
    font-weight: 500;
}

/*sidebar outline*/

#close-outline-filter-btn {
    top: 15px;
    opacity: 1;
    color: var(--light-text-color) !important;
}

#close-outline-filter-btn:hover {
    color: var(--primary-color) !important;
    background-color: transparent !important;
}

#close-outline-filter-btn:active {
    background-color: transparent !important;
}

#outline-content {
    padding-right: 0px;
    line-height: 1rem;
}

.outline-item {
    display: flex;
    padding-top: 0px;
    padding-bottom: 0px;
}

.outline-item .outline-label {
    display: block;
    width: 100%;
    padding-top: 0.4rem;
    padding-bottom: 0.4rem;
    border-right: solid 2px transparent;
    font-size: 0.8rem;
    font-weight: 500;
    color: var(--light-text-color-darker);
}

.outline-item:hover {
    background: none;
}

.outline-item:hover .outline-label {
    color: var(--primary-color);
}

.outline-label:hover {
    text-decoration: none;
}

.outline-active.outline-label {
    border-right: solid 2px var(--primary-color);
    font-weight: 500;
    color: var(--primary-color);
}

.outline-expander {
    padding-top: 0.4rem;
    padding-right: 0.5rem;
}

#toc-dropmenu .outline-label {
    line-height: 1rem;
}

#toc .outline-title {
    margin-top: 9px;
    font-size: 1rem;
    font-weight: 500;
    user-select: none;
}

#pin-outline-btn {
    padding: 14px 18px 0px 0px;
}

/*sidebar file-list and search results*/

#file-library-list[data-state="complete"] #sidebar-loading-template {
    padding: 0rem;
}

#typora-sidebar .file-list-item,
.ty-search-item {
    border: none;
    padding: 1rem;
}

body.html-for-mac #typora-sidebar .file-list-item,
body.html-for-mac .ty-search-item {
    transition-duration: 0.3s !important;
    transition-property: background-color, border, color, height !important;
}

#typora-sidebar .file-list-item:hover,
.ty-search-item:hover {
    background: var(--borders);
}

#typora-sidebar .ty-search-item-line {
    font-family: var(--font-family);
    font-size: 0.8rem;
    font-weight: 400;
    padding: 0.3rem;
    border-radius: 0.3rem;
    margin-left: 24px;
}

body.html-for-mac #typora-sidebar .ty-search-item-line {
    transition-duration: 0.2s;
}

#typora-sidebar .ty-search-item-line * {
    opacity: 1;
}

#typora-sidebar .ty-search-item .ty-search-item-line:hover,
#typora-sidebar .ty-search-item-line.active {
    background-color: transparent;
    color: var(--primary-color);
}

#typora-sidebar .file-list-item-file-name {
    font-weight: 800;
    font-size: 0.9rem;
    margin-bottom: 0rem;
    line-height: 1.8rem;
    float: right;
}

#typora-sidebar .file-list-item-file-ext-part {
    font-weight: 800;
    opacity: 0.7;
}

#typora-sidebar .file-list-item-parent-loc,
#typora-sidebar .file-list-item-time {
    font-family: var(--font-family);
    font-weight: 400;
    opacity: 0.7;
    display: block;
}

#typora-sidebar .file-list-item-summary {
    float: left;
    font-size: 0.8rem;
    opacity: 1;
}

#typora-sidebar input.file-list-item-file-name {
    margin: 0.5rem 0rem 0.5rem 0.7rem;
    padding: 0.4rem !important;
    line-height: 1rem;
    float: right;
    border-radius: 0.3rem;
    font-weight: 500;
    background-color: var(--boxes) !important;
}

#typora-sidebar .file-list-item-count {
    font-size: 0.75rem;
    background-color: var(--primary-color);
    color: white;
    border-radius: 0.2rem;
    min-width: 1.25rem;
    height: 1.25rem;
    text-align: center;
    line-height: 1.25rem;
    position: relative;
    top: 0.3rem;
}

#typora-sidebar .file-list-item.file-library-file-node {
    border: none;
}

#typora-sidebar .file-tree-node.active .file-node-background,
#typora-sidebar .file-list-item.active,
#typora-sidebar .ty-search-item.active {
    background-color: var(--borders);
    outline: 1px solid var(--boxes-darker);
    border: none;
    color: var(--primary-color) !important;
}

#typora-sidebar .file-tree-node.active .file-node-content {
    color: var(--primary-color) !important;
}

#typora-sidebar .file-tree-node {
    padding: 0rem;
    font-weight: 500;
    font-size: 0.9rem;
    margin-left: 0.8rem;
}

#typora-sidebar .file-tree-node .file-node-content {
    padding: 0rem;
    line-height: 2.2rem;
    height: 2.2rem;
    background: none;
    margin-bottom: 0px;
}

#typora-sidebar .file-tree-node .file-node-background {
    padding: 0rem;
    height: 2.2rem;
}

#typora-sidebar .file-tree-node .file-node-icon {
    margin-right: 0.5rem;
}

#typora-sidebar .file-tree-node .file-node-icon.fa-file-text-o {
    margin-top: 0.33rem;
}

#typora-sidebar .file-tree-node .file-node-icon.fa-folder {
    margin-top: 0.36rem;
}

#typora-sidebar .file-tree-node .fa-caret-down,
#typora-sidebar .file-tree-node .fa-caret-right {
    position: relative;
    top: 5px;
}

#typora-sidebar .file-tree-node .file-tree-rename-input {
    height: 2.2rem;
    background: none;
    border: none;
    font-size: 0.9rem;
    font-weight: 500;
    margin: 0rem;
    padding-left: 0rem;
}

/*no left border*/
#typora-sidebar .file-tree-node.active > .file-node-background {
    border: none;
}

/*no dotted highlighting*/
.file-library-node:not(.file-node-root):focus > .file-node-content {
    outline: none;
}

#typora-sidebar #sidebar-files-menu {
    border: solid 1px var(--borders);
    border-radius: 0.3rem;
    box-shadow: rgba(0, 0, 0, 0.2) 0px 3px 8px 0px;
}

#typora-sidebar #ty-sidebar-footer {
    border-top: solid 1px var(--borders);
    background-color: var(--bg-color);
    font-weight: 500;
}

#typora-sidebar #ty-sidebar-footer li {
    transition-duration: 0.2s;
    transition-property: background-color, color;
}

#typora-sidebar
    #ty-sidebar-footer
    li:not(.file-sort-item):not(:first-child):not(.empty-menu-group):not(.folder-menu-group):hover {
    color: var(--primary-color);
    background-color: var(--boxes);
}

#typora-sidebar
    #ty-sidebar-footer
    .file-action-item.file-sort-item
    > span:first-of-type {
    line-height: 2rem;
}

#typora-sidebar .ty-search-item-collapse-icon {
    top: 9px;
}

/*cursor*/
.file-node-content:hover {
    cursor: pointer;
}

body.html-for-mac
    .file-tree-node:not(.file-node-root):not(.file-node-expanded)
    .file-node-background {
    transition-duration: 0.2s;
    transition-property: background-color;
}

.file-tree-node:not(.file-node-root):not(.file-node-expanded):hover
    .file-node-background {
    background-color: var(--borders);
}

/*sidebar footer*/
#typora-sidebar .sidebar-footer-item {
    transition-duration: 0.2s;
    transition-property: background-color, color;
    font-weight: 700;
}

#typora-sidebar .sidebar-footer-item:hover {
    color: var(--primary-color);
    background-color: var(--boxes);
}

#typora-quick-open {
    background-color: var(--bg-color);
    border: 1px solid var(--borders);
    border-radius: 0.3rem;
    padding: 0rem;
    box-shadow: rgba(0, 0, 0, 0.25) 0px 3px 16px 0px;
    overflow: hidden;
}

#typora-quick-open-input {
    margin-right: 20px;
}

#typora-quick-open-input .input {
    box-shadow: none !important /*required*/;
    border: none !important /*required*/;
    font-weight: 400 !important /*required*/;
    margin: 0.5rem;
    margin-left: 0.8rem;
}

.typora-quick-open-item {
    background-color: var(--bg-color);
    border: none;
    font-weight: 500;
    transition-duration: 0.2s;
    transition-property: background-color;
}

.typora-quick-open-item:hover {
    background-color: var(--boxes);
    color: var(--primary-color);
}

.typora-quick-open-item.active {
    background-color: var(--boxes);
    border: none;
}

.typora-quick-open-item-path {
    opacity: 1;
    color: var(--light-text-color);
}

.typora-quick-open-item:hover .typora-quick-open-item-path {
    opacity: 0.7;
    color: var(--primary-color);
}

.ty-quick-open-category-title {
    font-size: 10px;
    font-weight: 700;
    letter-spacing: 1.2px;
    text-transform: uppercase;
    opacity: 1;
    color: var(--light-text-color);
    line-height: 32px;
    padding-top: 6px;
    height: 32px;
}

/** focus mode */
.on-focus-mode blockquote {
    border-left-color: rgba(85, 85, 85, 0.12);
}

.md-lang {
    color: var(--primary-color);
}

/*NOTIFICATION*/

#md-notification {
    border-bottom: solid 1px var(--borders);
    box-shadow: rgba(0, 0, 0, 0.2) 0px 3px 8px 0px;
}

#md-notifcation .btn {
    border: 0;
}

/*PREFERENCES*/

.ty-preferences {
    font-family: var(--font-family);
}

.ty-preferences .window-header {
    justify-content: space-between;
    box-shadow: rgba(0, 0, 0, 0.2) 0px 3px 8px 0px;
    border-bottom: solid 1px var(--borders);
}

.ty-preferences .window-header-content {
    background-color: var(--bg-color);
    margin: 0rem;
}

.ty-preferences .window-header h2 {
    font-weight: 600;
    font-size: 1.5rem;
    margin: 0rem;
    margin-left: 1rem;
}

.unibody-window .ty-preferences .window-header h2 {
    margin-left: 1rem !important;
}

.ty-preferences .window-header-back {
    margin-left: 1.2rem;
}

.ty-preferences .window-header-back .icon {
    border-right: none;
}

/*preferences sidebar*/
.ty-preferences .window-content {
    background-color: var(--bg-color);
}

.ty-preferences .nav-group-item {
    color: var(--text-color);
    height: 2.5rem;
    line-height: 2.6rem;
    font-weight: 500;
    padding: 0px 0px 0px 2rem;
    font-size: 1rem;
    transition-duration: 0.2s;
    transition-property: background-color;
}

.ty-preferences .nav-group-item:hover {
    background-color: var(--borders);
    border-radius: 0px;
}

.ty-preferences .nav-group-item.active {
    border-radius: 0rem;
    border: none;
    outline: 1px solid var(--borders);
    background-color: var(--bg-color);
    color: var(--primary-color);
}

.ty-preferences .pane-sm {
    background: var(--boxes);
    flex-basis: 240px;
    flex-grow: 0;
    justify-content: center;
    border-right: 1px solid var(--borders);
    margin: 0rem;
    padding: 0rem;
}

.ty-preferences .pane-sm .list-group {
    width: 100%;
    max-width: 30rem;
}

.ty-preferences .list-group-header {
    display: flex;
    justify-content: space-around;
}

.ty-preferences .list-group-header div {
    width: 100%;
    margin-right: 18px;
    margin-left: 18px;
}

.ty-preferences .pane-sm .search-input {
    margin: 0rem !important;
    width: 100%;
    font-size: 1rem !important;
    height: 2.75rem;
}

.ty-preferences .pane-sm .search-input:active,
.ty-preferences .pane-sm .search-input:focus {
    border: solid 1px var(--primary-color) !important;
    outline: none;
}

/*preferences main*/
.ty-preferences .panel-header {
    font-weight: 600;
    font-size: 1.6rem;
}

/*preferences stuff*/
.ty-preferences .dropdown-menu > li,
.dropdown-item {
    font-weight: 500;
    font-size: 1rem;
    transition-duration: 0.2s;
    transition-property: all;
}

.ty-preferences .dropdown-menu .active,
.ty-preferences .dropdown-menu li:hover,
.dropdown-item:hover {
    background-color: var(--boxes);
    color: var(--primary-color);
}

#ty-spell-check-dict-missing-secondary-btn:hover {
    color: var(--primary-color) !important;
}

.header-close .icon {
    border: none !important;
}

/*preferences export*/

.export-detail {
    background-color: transparent !important /*required*/;
}

.export-items-list .separator {
    margin: 0.4rem;
    border-top: 1px solid var(--borders);
}

.export-items-list-control {
    background-color: var(--boxes) !important /*required*/;
}

.export-item {
    padding: 0.4rem !important /*required*/;
    color: var(--light-text-color-darker);
    font-weight: 500;
    cursor: pointer;
}

.export-item.active {
    background-color: transparent !important /*required*/;
    color: var(--primary-color);
    font-weight: 500 !important /*required*/;
}

/*DROPDOWN*/

.dropdown-menu:not(.megamenu-menu-list),
.auto-suggest-container {
    background-color: var(--bg-color);
    border: solid 1px var(--borders) !important;
    box-shadow: rgba(0, 0, 0, 0.2) 0px 3px 8px 0px;
    user-select: none;
}

.dropdown-menu > li > a,
.auto-suggest-container li {
    font-weight: 500;
    font-size: 0.8rem;
    transition-duration: 0.2s;
    transition-property: all;
}

.dropdown-menu > .active > a,
.dropdown-menu > li > a:hover,
.menu-style-btn.active,
.auto-suggest-container li:hover,
.auto-suggest-container li.active,
.context-menu.dropdown-menu > .active > a,
.context-menu.dropdown-menu > li > a:hover {
    color: var(--primary-color);
    background-color: var(--boxes);
}

.menu-style-btn {
    color: var(--text-color);
    border: none;
    transition-duration: 0.2s;
    transition-property: all;
}

.menu-style-btn:hover {
    color: var(--primary-color);
    background-color: var(--boxes);
    border: none;
}

header .menu-style-btn:hover {
    background-color: transparent;
}

.menu-item-container {
    padding: 0 12px 0 4px;
}

.menu-item-container a.menu-style-btn {
    padding: 0.3rem 0.6rem;
    margin: 0;
}

.dropdown-menu .divider {
    border-color: var(--borders);
    opacity: 1;
}

/*BUTTON*/

.btn,
button,
.md-image-btn {
    border: none !important;
    border-radius: 0.3rem !important;
    color: var(--text-color) !important;
    transition-duration: 0.2s;
    transition-property: all;
    font-size: 0.9rem !important;
    font-weight: 500;
    outline: none;
}

.btn-default,
.md-image-btn {
    border: none !important;
    border-radius: 0.3rem !important;
    background-color: var(--boxes) !important;
}

.btn:hover,
.button-hover,
.md-image-btn:hover {
    border: none;
    border-radius: 0.3rem;
    background-color: var(--borders) !important;
    color: var(--text-color);
}

button:active,
button.active,
.btn:active,
.btn-default:active,
.md-image-btn:active {
    border: none;
    border-radius: 0.3rem;
    background-color: var(--boxes-darker) !important;
    box-shadow: none;
    outline: none;
    color: var(--text-color);
}

.btn:focus,
.md-image-btn:focus {
    border: none !important;
    outline: none !important;
    background-color: var(--boxes-darker);
}

.btn-primary {
    border: none;
    border-radius: 0.3rem;
    background-color: var(--primary-color);
    color: white !important;
}

.btn-primary:hover,
.btn-primary:focus {
    color: white;
    background-color: var(--primary-color-darker) !important;
}

.btn.dropdown-toggle-split,
.btn.dropdown-toggle-split:hover {
    border-radius: 0rem 0.3rem 0.3rem 0rem;
}

#ty-spell-check-dict-missing-primary-btn {
    border-radius: 0.3rem 0rem 0rem 0.3rem;
}

.open > .dropdown-toggle.btn-primary {
    background-color: var(--primary-color);
    border-color: transparent;
}

/*GHOST BUTTON*/

.window-header button,
#close-sidebar-menu-btn,
.html-for-mac .sidebar-tab-btn,
.label-hint,
.ty-table-edit .btn,
.zoom-hint-button,
.md-rawblock-tooltip-btn,
.md-delete-toc,
#md-searchpanel .input-group-addon.btn,
#pin-outline-btn,
.icon-button {
    background-color: transparent !important;
    color: var(--light-text-color) !important;
    opacity: 1 !important;
    transition-duration: 0.2s;
    transition-property: color;
}

.window-header button:hover,
.window-header button:focus,
#close-sidebar-menu-btn:hover,
#close-sidebar-menu-btn:focus,
.html-for-mac .sidebar-tab-btn:hover,
.html-for-mac .sidebar-tab-btn:focus,
.label-hint:hover,
.label-hint:focus,
.ty-table-edit .btn:hover,
.ty-table-edit .btn:focus,
.zoom-hint-button:hover,
.zoom-hint-button:focus,
.md-rawblock-tooltip-btn:hover,
.md-rawblock-tooltip-btn:focus,
.md-delete-toc:hover,
.md-delete-toc:focus,
#md-searchpanel .input-group-addon.btn:hover,
#md-searchpanel .input-group-addon.btn:focus,
#pin-outline-btn:hover,
#pin-outline-btn:focus,
.icon-button:hover,
.icon-button:focus {
    color: var(--primary-color) !important;
    background: none !important;
}

.ty-table-edit .btn.active {
    color: var(--primary-color) !important;
    box-shadow: none;
}

/*IMAGE BUTTON*/

.md-image-btn {
    background-color: var(--boxes);
    transition-duration: 0.2s;
    transition-property: background-color;
}

.md-image-btn:before {
    color: var(--text-color);
    transition-duration: 0.2s;
    transition-property: color;
}

.md-image-btn:hover {
    background-color: var(--borders);
}

.md-image-btn:hover:before {
    color: var(--primary-color);
}

.md-image-input-src-btn {
    border-radius: 0.3rem 0rem 0rem 0.3rem !important;
}

.md-image-pick-file-btn {
    border-left: none;
    border-radius: 0rem 0.3rem 0.3rem 0rem !important;
}

/*SEARCH-INPUTS*/

.search-input,
.search,
.form-control,
#file-library-search-input {
    background-color: transparent !important;
    border-radius: 0.3rem !important;
    border: solid 1px var(--boxes-darker) !important;
    box-shadow: none !important;
    color: var(---heading-text-color) !important;
    font-size: 0.9rem !important;
    font-weight: 400;
    padding: 0.7rem !important;
    height: 2rem;
    transition-duration: 0.2s;
    transition-property: border, box-shadow;
}

.search-input:hover,
.search:hover,
.form-control:hover,
#file-library-search-input:hover {
    border: solid 1px var(--boxes-darker2) !important;
    box-shadow: 0 2px 12px rgba(0, 0, 0, 0.15) !important;
}

.search-input:focus,
.search:focus,
.form-control:focus,
#file-library-search-input:focus {
    background-color: transparent !important;
    border-color: var(--primary-color) !important;
    box-shadow: 0 2px 12px rgba(0, 0, 0, 0.15) !important;
    color: var(--heading-text-color) !important;
    font-size: 0.9rem !important;
    padding: 0.7rem !important;
}

.clear-btn-icon {
    top: 9px !important /*required*/;
    right: 9px !important /*required*/;
}

.content tr.search-hit,
.search-hit,
.md-search-hit,
.md-search-hit.md-search-select,
.md-search-select,
.ty-file-search-match-text {
    background-color: var(--boxes-darkest);
    color: white;
    padding: 0.2rem 0.1rem;
    border-radius: 0.2rem;
}

/*ZOOM HINT*/

#zoom-hint {
    border-radius: 0.3rem;
    border: solid 1px var(--borders);
    user-select: none;
    box-shadow: rgba(0, 0, 0, 0.2) 0px 3px 8px 0px;
}

#zoom-hint #zoom-hint-reset {
    border-left: none;
    font-weight: 600;
}

/*SEARCHPANEL*/

#md-searchpanel {
    border-bottom: 1px solid var(--borders);
    box-shadow: rgba(0, 0, 0, 0.2) 0px 3px 8px 0px;
    max-height: 46px;
}

.mac-seamless-mode #md-searchpanel {
    max-height: 70px;
}

#md-searchpanel.searchpanel-replace-mode {
    max-height: 84px;
}

.mac-seamless-mode #md-searchpanel.searchpanel-replace-mode {
    max-height: 108px;
}

#md-searchpanel input {
    height: 2rem;
    margin: 0rem !important;
    padding: 6px 12px !important;
    font-size: 12px !important;
}

#md-searchpanel .input-group-addon {
    height: 2rem;
}

#md-searchpanel .input-group-addon.close-btn {
    padding-left: 8px;
}

.unibody-window #md-searchpanel .btn {
    line-height: 2rem;
}

.searchpanel-search-option-btn {
    top: 9px;
    border: none;
    color: var(--light-text-color-brighter) !important /*required*/;
    transition-duration: 0.3s;
}

.searchpanel-search-option-btn:hover {
    color: var(--primary-color) !important /*required*/;
    background-color: transparent !important /*required*/;
}

.searchpanel-search-option-btn.select,
.searchpanel-search-option-btn.active {
    color: white !important;
    background-color: var(--primary-color) !important;
}

#searchpanel-case-option-btn {
    right: 33px;
}

#searchpanel-word-option-btn {
    right: 9px;
}

#searchpanel-word-option-btn,
#searchpanel-case-option-btn {
    background: none;
}

#md-searchpanel .btn:not(.close-btn):hover {
    box-shadow: none;
}

/*SELECT*/
/*TEXT INPUT*/
/*NUMBER INPUT*/

/* the input #md-grid-height doesn't have a type attached for some reason and needs to be adressed seperately */

html select,
html input[type="text"],
html input[type="number"],
#md-grid-height {
    background-color: var(--bg-color) !important;
    border-radius: 0.3rem !important;
    border: solid 1px var(--boxes-darker) !important;
    box-shadow: none !important;
    color: var(--text-color) !important;
    font-size: 0.9rem !important;
    font-weight: 500 !important;
    padding: 0.3rem !important;
    height: 2.1rem !important;
    transition-duration: 0.2s;
    transition-property: border;
    cursor: text;
}

select {
    cursor: pointer !important;
}

input[type="text"],
input[type="number"] {
    cursor: text;
}

html select:hover,
html input[type="text"]:hover,
html input[type="number"]:hover,
#md-grid-height:hover {
    background-color: var(--bg-color) !important;
    border-radius: 0.3rem !important;
    border-color: var(--boxes-darker2) !important;
    box-shadow: 0 2px 12px rgba(0, 0, 0, 0.04) !important;
    color: var(--text-color) !important;
    font-size: 0.9rem !important;
}

html select:focus,
html input[type="text"]:focus,
html input[type="number"]:focus,
#md-grid-height:focus {
    border-color: var(--primary-color) !important;
    box-shadow: 0 2px 12px rgba(0, 0, 0, 0.04) !important;
}

input[type="text"]::placeholder,
input[type="number"]::placeholder,
#md-grid-height::placeholder {
    color: var(--light-text-color-brighter) !important;
}

input[disabled],
input[disabled]:hover,
input[disabled]:focus {
    cursor: not-allowed;
}

/*TEXTAREA*/

textarea {
    background-color: transparent;
    border: solid 1px var(--boxes-darker);
    border-radius: 0.3rem;
    transition-duration: 0.2s;
}

textarea:hover {
    border-color: var(--boxes-darker2);
    box-shadow: 0 2px 12px rgba(0, 0, 0, 0.04);
}

textarea:focus {
    border-color: var(--primary-color);
    box-shadow: 0 2px 12px rgba(0, 0, 0, 0.04);
    outline: none;
}

/*MODAL*/

.modal-header,
#common-dialog .modal-header {
    border-bottom: solid 1px var(--borders);
    padding-bottom: 15px;
}

.modal-title {
    font-size: 1.25rem;
    font-weight: 500;
    user-select: none;
}

.modal-body {
    font-size: 0.9rem;
    color: var(--light-text-color-brighter);
    user-select: none;
}

.modal-content {
    box-shadow: rgba(0, 0, 0, 0.2) 0px 3px 10px 0px;
    border: solid 1px var(--boxes-darker);
    border-radius: 0.3rem;
}

.modal-footer {
    border-top: solid 1px var(--borders);
}

.modal-open .modal.fade.in {
    background: none;
    backdrop-filter: blur(5px);
    -webkit-backdrop-filter: blur(5px);
}

/*LANGS*/

.ty-spell-check-panel-item {
    font-weight: 500;
    transition-duration: 0.2s;
    transition-property: background-color, color;
}

.ty-spell-check-panel-item:hover {
    color: var(--primary-color);
    background-color: var(--boxes);
}

.ty-spell-check-panel-item.ty-active {
    background-color: var(--boxes);
}

/*TOOLTIP*/

.ty-tooltip {
    color: var(--text-color) !important;
    background-color: var(--boxes) !important;
    border-radius: 0.3rem !important;
    border: 1px solid var(--borders) !important;
    -webkit-filter: none !important;
    filter: none;
    box-shadow: rgba(0, 0, 0, 0.2) 0px 3px 8px 0px;
}

/*FOOTER*/

footer.ty-footer {
    border: none;
}

.footer-item:hover {
    background-color: var(--boxes) !important;
}

#footer-word-count-info {
    padding: 4px 0;
}

.footer-word-count-info-line {
    padding: 0.25rem;
    line-height: 1.6rem;
}

#footer-word-count-info tr {
    font-weight: 500;
    font-size: 0.8rem;
    transition-duration: 0.2s;
    transition-property: all;
}

#footer-word-count-info tr td:nth-child(1) {
    padding: 0rem;
    padding-right: 1rem;
}

#footer-word-count-info .ty-footer-word-count-all tr:hover {
    color: var(--primary-color) !important;
    background-color: var(--boxes) !important;
}

/*MEGAMENU*/

.megamenu-menu {
    box-shadow: none;
    background-color: var(--boxes);
    border-right: 1px solid var(--borders);
}

.megamenu-opened .megamenu-menu {
    left: 0px;
}

#megamenu-content {
    top: 0px;
    left: 0px;
    right: 0px;
    bottom: 0px;
}

#megamenu-menu-list {
    box-shadow: none;
    border: none;
    background-color: transparent;
}

#megamenu-menu-list li a {
    color: var(--text-color);
    height: 2rem;
    line-height: 1.8rem;
    transition-duration: 0.2s;
    transition-property: background-color;
}

#megamenu-menu-list li a:hover {
    background-color: var(--borders);
}

#megamenu-menu-list li a.active {
    color: var(--primary-color);
    background-color: var(--bg-color);
    outline: solid 1px var(--borders);
}

#megamenu-menu-list .divider {
    background-color: var(--borders);
    margin: 16px 0 0 0;
}

.megamenu-menu-list .saved #m-saved {
    cursor: default;
}

.megamenu-menu-list .saved #m-saved .fa {
    color: var(--primary-color);
}

.megamenu-menu-list .saved #m-saved:hover {
    background-color: transparent;
}

.megamenu-menu-list #m-close:hover {
    color: var(--danger-color);
}

.megamenu-menu-header {
    border-bottom: solid 1px var(--borders);
    margin-bottom: 1.2rem;
    height: 74px;
    transition-duration: 0.3s;
}

.megamenu-menu-header:hover {
    background-color: var(--borders);
}

.megamenu-menu-header #megamenu-menu-header-title {
    color: var(--text-color);
    font-weight: 700;
    font-size: 16px;
    left: 56px;
    top: 24px;
}

#megamenu-back-btn {
    color: var(--text-color);
    font-size: 16px;
    left: 24px;
    top: 24px;
}

.megamenu-opened header {
    background-color: var(--bg-color);
    background-image: none;
}

.megamenu-content {
    background-color: var(--bg-color);
    background-image: none;
}

.megamenu-menu-panel:not(:first-of-type) {
    margin-top: 2rem;
}

.megamenu-menu-panel h1 {
    font-weight: 900;
    font-size: 1.8rem;
    margin: 1rem 0rem 0.4rem 0rem;
}

.megamenu-menu-panel h2 {
    font-weight: 800;
    font-size: 1.3rem;
    margin: 1rem 0rem 0.4rem 0rem;
}

/*recent files*/

#recent-file-panel tbody tr {
    font-weight: 600;
    transition-duration: 0.4s;
}

#recent-file-panel tbody tr:hover,
.megamenu-menu-panel tbody tr:hover td:nth-child(1) {
    color: var(--primary-color);
}

#recent-file-panel tbody tr:nth-child(2n-1) {
    background-color: var(--boxes);
}

/*about help*/

.about-content-slogon {
    color: var(--light-text-color);
}

/*for the god himself*/
.about-content-slogon span {
    color: var(--primary-color) !important;
}

#about-content tbody tr {
    font-weight: 500;
    transition-duration: 0.4s;
}

#about-content tbody tr:hover {
    color: var(--primary-color);
    background-color: var(--boxes) !important /*required important*/;
}

.long-btn {
    margin-bottom: 12px;
    margin-left: 2px;
    box-shadow: rgba(0, 0, 0, 0.2) 2px 2px 6px;
    background-color: var(--bg-color);
    border: 1px solid var(--borders);
    border-radius: 0.3rem;
    padding: 1rem;

    font-weight: 700;
    font-size: 1rem;

    transition: background 0.2s, color 0.2s, box-shadow 0.2s;
}

.long-btn:hover {
    background-color: var(--primary-color);
    color: white !important /*important required*/;
    border: 1px solid transparent;
    box-shadow: rgba(0, 0, 0, 0.2) 2px 2px 6px,
        rgba(56, 132, 255, 0.2) 0px 0px 10px;
}

#m-import-local:hover .preference-item-hint {
    color: white;
    opacity: 0.7;
}

#recent-file-panel-action-btn {
    height: 34px;
    border: none;
    background-color: var(--boxes);
}

#theme-preview-grid {
    max-width: none;
    padding: 1.5rem;
    background-color: var(--boxes);
    border-radius: 0.5rem;
    display: grid;
    grid-template-columns: repeat(auto-fill, minmax(300px, 1fr));
    grid-gap: 1.5rem;
}

.theme-preview-div {
    border: none;
    border-radius: 0.4rem;
    box-shadow: rgba(0, 0, 0, 0.2) 0px 0px 15px;
    margin: 0rem;
    transition-duration: 0.3s;
}

.theme-preview-div:hover {
    box-shadow: rgba(0, 0, 0, 0.6) 3px 8px 15px;
    cursor: pointer;
    transform: rotate3d(1, -0.2, 0.2, 15deg);
}

.theme-preview-content {
    width: 100%;
    height: 100%;
    border-radius: 0.4rem;
}

.theme-preview-content html {
    width: 100%;
    height: 100%;
}

.theme-preview-div.active .fa {
    color: var(--primary-color);
    bottom: 4px;
    left: 4px;
}

.theme-preview-div .fa-check-circle:before {
    background-color: var(--bg-color);
    padding: 0px 2px;
    border-radius: 1rem;
}

.megamenu-menu-panel tbody tr {
    border-radius: 0.3rem;
    transition-duration: 0.2s;
    transition-property: background-color;
}

.megamenu-menu-panel tbody tr:hover {
    background-color: var(--borders) !important /*required important*/;
}

/*MIN MAX CLOSE*/
#w-min,
#w-max,
#w-restore,
#w-close {
    border-radius: 0px !important;
    font-size: 10px !important;
    width: 46px !important;
    height: 29px !important;
}

.btn.toolbar-icon svg,
.btn.toolbar-icon .ty-icon {
    position: relative;
    top: 2px;
}

#w-close.btn.toolbar-icon .ty-icon {
    left: 1px;
}

#w-close:hover {
    background-color: var(--danger-color) !important;
    color: white !important;
}

/*EXTRA STUFF*/

a[type="page-link"] {
    display: block;
    background-color: var(--bg-color);
    box-shadow: rgba(0, 0, 0, 0.2) 0px 3px 8px 0px;
    border: 1px solid var(--borders);
    border-radius: 0.3rem;
    padding: 1rem;

    font-weight: 600;

    transition-duration: 0.2s;
    transition-property: border, box-shadow;
}

a[type="page-link"]:hover {
    box-shadow: rgba(0, 0, 0.2, 0.2) 0px 3px 8px 0px;
    border: 1px solid var(--primary-color);
}

p[type="description"] {
    color: var(--light-text-color);
}

/*kbd*/

kbd {
    font-family: var(--font-family);
}
```


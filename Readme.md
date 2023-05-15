



TedTalk

 pre { line-height: 125%; }
td.linenos .normal { color: inherit; background-color: transparent; padding-left: 5px; padding-right: 5px; }
span.linenos { color: inherit; background-color: transparent; padding-left: 5px; padding-right: 5px; }
td.linenos .special { color: #000000; background-color: #ffffc0; padding-left: 5px; padding-right: 5px; }
span.linenos.special { color: #000000; background-color: #ffffc0; padding-left: 5px; padding-right: 5px; }
.highlight .hll { background-color: var(--jp-cell-editor-active-background) }
.highlight { background: var(--jp-cell-editor-background); color: var(--jp-mirror-editor-variable-color) }
.highlight .c { color: var(--jp-mirror-editor-comment-color); font-style: italic } /\* Comment \*/
.highlight .err { color: var(--jp-mirror-editor-error-color) } /\* Error \*/
.highlight .k { color: var(--jp-mirror-editor-keyword-color); font-weight: bold } /\* Keyword \*/
.highlight .o { color: var(--jp-mirror-editor-operator-color); font-weight: bold } /\* Operator \*/
.highlight .p { color: var(--jp-mirror-editor-punctuation-color) } /\* Punctuation \*/
.highlight .ch { color: var(--jp-mirror-editor-comment-color); font-style: italic } /\* Comment.Hashbang \*/
.highlight .cm { color: var(--jp-mirror-editor-comment-color); font-style: italic } /\* Comment.Multiline \*/
.highlight .cp { color: var(--jp-mirror-editor-comment-color); font-style: italic } /\* Comment.Preproc \*/
.highlight .cpf { color: var(--jp-mirror-editor-comment-color); font-style: italic } /\* Comment.PreprocFile \*/
.highlight .c1 { color: var(--jp-mirror-editor-comment-color); font-style: italic } /\* Comment.Single \*/
.highlight .cs { color: var(--jp-mirror-editor-comment-color); font-style: italic } /\* Comment.Special \*/
.highlight .kc { color: var(--jp-mirror-editor-keyword-color); font-weight: bold } /\* Keyword.Constant \*/
.highlight .kd { color: var(--jp-mirror-editor-keyword-color); font-weight: bold } /\* Keyword.Declaration \*/
.highlight .kn { color: var(--jp-mirror-editor-keyword-color); font-weight: bold } /\* Keyword.Namespace \*/
.highlight .kp { color: var(--jp-mirror-editor-keyword-color); font-weight: bold } /\* Keyword.Pseudo \*/
.highlight .kr { color: var(--jp-mirror-editor-keyword-color); font-weight: bold } /\* Keyword.Reserved \*/
.highlight .kt { color: var(--jp-mirror-editor-keyword-color); font-weight: bold } /\* Keyword.Type \*/
.highlight .m { color: var(--jp-mirror-editor-number-color) } /\* Literal.Number \*/
.highlight .s { color: var(--jp-mirror-editor-string-color) } /\* Literal.String \*/
.highlight .ow { color: var(--jp-mirror-editor-operator-color); font-weight: bold } /\* Operator.Word \*/
.highlight .pm { color: var(--jp-mirror-editor-punctuation-color) } /\* Punctuation.Marker \*/
.highlight .w { color: var(--jp-mirror-editor-variable-color) } /\* Text.Whitespace \*/
.highlight .mb { color: var(--jp-mirror-editor-number-color) } /\* Literal.Number.Bin \*/
.highlight .mf { color: var(--jp-mirror-editor-number-color) } /\* Literal.Number.Float \*/
.highlight .mh { color: var(--jp-mirror-editor-number-color) } /\* Literal.Number.Hex \*/
.highlight .mi { color: var(--jp-mirror-editor-number-color) } /\* Literal.Number.Integer \*/
.highlight .mo { color: var(--jp-mirror-editor-number-color) } /\* Literal.Number.Oct \*/
.highlight .sa { color: var(--jp-mirror-editor-string-color) } /\* Literal.String.Affix \*/
.highlight .sb { color: var(--jp-mirror-editor-string-color) } /\* Literal.String.Backtick \*/
.highlight .sc { color: var(--jp-mirror-editor-string-color) } /\* Literal.String.Char \*/
.highlight .dl { color: var(--jp-mirror-editor-string-color) } /\* Literal.String.Delimiter \*/
.highlight .sd { color: var(--jp-mirror-editor-string-color) } /\* Literal.String.Doc \*/
.highlight .s2 { color: var(--jp-mirror-editor-string-color) } /\* Literal.String.Double \*/
.highlight .se { color: var(--jp-mirror-editor-string-color) } /\* Literal.String.Escape \*/
.highlight .sh { color: var(--jp-mirror-editor-string-color) } /\* Literal.String.Heredoc \*/
.highlight .si { color: var(--jp-mirror-editor-string-color) } /\* Literal.String.Interpol \*/
.highlight .sx { color: var(--jp-mirror-editor-string-color) } /\* Literal.String.Other \*/
.highlight .sr { color: var(--jp-mirror-editor-string-color) } /\* Literal.String.Regex \*/
.highlight .s1 { color: var(--jp-mirror-editor-string-color) } /\* Literal.String.Single \*/
.highlight .ss { color: var(--jp-mirror-editor-string-color) } /\* Literal.String.Symbol \*/
.highlight .il { color: var(--jp-mirror-editor-number-color) } /\* Literal.Number.Integer.Long \*/
 

/\*-----------------------------------------------------------------------------
| Copyright (c) Jupyter Development Team.
| Distributed under the terms of the Modified BSD License.
|----------------------------------------------------------------------------\*/

/\*
 \* Mozilla scrollbar styling
 \*/

/\* use standard opaque scrollbars for most nodes \*/
[data-jp-theme-scrollbars='true'] {
 scrollbar-color: rgb(var(--jp-scrollbar-thumb-color))
 var(--jp-scrollbar-background-color);
}

/\* for code nodes, use a transparent style of scrollbar. These selectors
 \* will match lower in the tree, and so will override the above \*/
[data-jp-theme-scrollbars='true'] .CodeMirror-hscrollbar,
[data-jp-theme-scrollbars='true'] .CodeMirror-vscrollbar {
 scrollbar-color: rgba(var(--jp-scrollbar-thumb-color), 0.5) transparent;
}

/\* tiny scrollbar \*/

.jp-scrollbar-tiny {
 scrollbar-color: rgba(var(--jp-scrollbar-thumb-color), 0.5) transparent;
 scrollbar-width: thin;
}

/\*
 \* Webkit scrollbar styling
 \*/

/\* use standard opaque scrollbars for most nodes \*/

[data-jp-theme-scrollbars='true'] ::-webkit-scrollbar,
[data-jp-theme-scrollbars='true'] ::-webkit-scrollbar-corner {
 background: var(--jp-scrollbar-background-color);
}

[data-jp-theme-scrollbars='true'] ::-webkit-scrollbar-thumb {
 background: rgb(var(--jp-scrollbar-thumb-color));
 border: var(--jp-scrollbar-thumb-margin) solid transparent;
 background-clip: content-box;
 border-radius: var(--jp-scrollbar-thumb-radius);
}

[data-jp-theme-scrollbars='true'] ::-webkit-scrollbar-track:horizontal {
 border-left: var(--jp-scrollbar-endpad) solid
 var(--jp-scrollbar-background-color);
 border-right: var(--jp-scrollbar-endpad) solid
 var(--jp-scrollbar-background-color);
}

[data-jp-theme-scrollbars='true'] ::-webkit-scrollbar-track:vertical {
 border-top: var(--jp-scrollbar-endpad) solid
 var(--jp-scrollbar-background-color);
 border-bottom: var(--jp-scrollbar-endpad) solid
 var(--jp-scrollbar-background-color);
}

/\* for code nodes, use a transparent style of scrollbar \*/

[data-jp-theme-scrollbars='true'] .CodeMirror-hscrollbar::-webkit-scrollbar,
[data-jp-theme-scrollbars='true'] .CodeMirror-vscrollbar::-webkit-scrollbar,
[data-jp-theme-scrollbars='true']
 .CodeMirror-hscrollbar::-webkit-scrollbar-corner,
[data-jp-theme-scrollbars='true']
 .CodeMirror-vscrollbar::-webkit-scrollbar-corner {
 background-color: transparent;
}

[data-jp-theme-scrollbars='true']
 .CodeMirror-hscrollbar::-webkit-scrollbar-thumb,
[data-jp-theme-scrollbars='true']
 .CodeMirror-vscrollbar::-webkit-scrollbar-thumb {
 background: rgba(var(--jp-scrollbar-thumb-color), 0.5);
 border: var(--jp-scrollbar-thumb-margin) solid transparent;
 background-clip: content-box;
 border-radius: var(--jp-scrollbar-thumb-radius);
}

[data-jp-theme-scrollbars='true']
 .CodeMirror-hscrollbar::-webkit-scrollbar-track:horizontal {
 border-left: var(--jp-scrollbar-endpad) solid transparent;
 border-right: var(--jp-scrollbar-endpad) solid transparent;
}

[data-jp-theme-scrollbars='true']
 .CodeMirror-vscrollbar::-webkit-scrollbar-track:vertical {
 border-top: var(--jp-scrollbar-endpad) solid transparent;
 border-bottom: var(--jp-scrollbar-endpad) solid transparent;
}

/\* tiny scrollbar \*/

.jp-scrollbar-tiny::-webkit-scrollbar,
.jp-scrollbar-tiny::-webkit-scrollbar-corner {
 background-color: transparent;
 height: 4px;
 width: 4px;
}

.jp-scrollbar-tiny::-webkit-scrollbar-thumb {
 background: rgba(var(--jp-scrollbar-thumb-color), 0.5);
}

.jp-scrollbar-tiny::-webkit-scrollbar-track:horizontal {
 border-left: 0px solid transparent;
 border-right: 0px solid transparent;
}

.jp-scrollbar-tiny::-webkit-scrollbar-track:vertical {
 border-top: 0px solid transparent;
 border-bottom: 0px solid transparent;
}

/\*
 \* Phosphor
 \*/

.lm-ScrollBar[data-orientation='horizontal'] {
 min-height: 16px;
 max-height: 16px;
 min-width: 45px;
 border-top: 1px solid #a0a0a0;
}

.lm-ScrollBar[data-orientation='vertical'] {
 min-width: 16px;
 max-width: 16px;
 min-height: 45px;
 border-left: 1px solid #a0a0a0;
}

.lm-ScrollBar-button {
 background-color: #f0f0f0;
 background-position: center center;
 min-height: 15px;
 max-height: 15px;
 min-width: 15px;
 max-width: 15px;
}

.lm-ScrollBar-button:hover {
 background-color: #dadada;
}

.lm-ScrollBar-button.lm-mod-active {
 background-color: #cdcdcd;
}

.lm-ScrollBar-track {
 background: #f0f0f0;
}

.lm-ScrollBar-thumb {
 background: #cdcdcd;
}

.lm-ScrollBar-thumb:hover {
 background: #bababa;
}

.lm-ScrollBar-thumb.lm-mod-active {
 background: #a0a0a0;
}

.lm-ScrollBar[data-orientation='horizontal'] .lm-ScrollBar-thumb {
 height: 100%;
 min-width: 15px;
 border-left: 1px solid #a0a0a0;
 border-right: 1px solid #a0a0a0;
}

.lm-ScrollBar[data-orientation='vertical'] .lm-ScrollBar-thumb {
 width: 100%;
 min-height: 15px;
 border-top: 1px solid #a0a0a0;
 border-bottom: 1px solid #a0a0a0;
}

.lm-ScrollBar[data-orientation='horizontal']
 .lm-ScrollBar-button[data-action='decrement'] {
 background-image: var(--jp-icon-caret-left);
 background-size: 17px;
}

.lm-ScrollBar[data-orientation='horizontal']
 .lm-ScrollBar-button[data-action='increment'] {
 background-image: var(--jp-icon-caret-right);
 background-size: 17px;
}

.lm-ScrollBar[data-orientation='vertical']
 .lm-ScrollBar-button[data-action='decrement'] {
 background-image: var(--jp-icon-caret-up);
 background-size: 17px;
}

.lm-ScrollBar[data-orientation='vertical']
 .lm-ScrollBar-button[data-action='increment'] {
 background-image: var(--jp-icon-caret-down);
 background-size: 17px;
}

/\*-----------------------------------------------------------------------------
| Copyright (c) Jupyter Development Team.
| Copyright (c) 2014-2017, PhosphorJS Contributors
|
| Distributed under the terms of the BSD 3-Clause License.
|
| The full license is in the file LICENSE, distributed with this software.
|----------------------------------------------------------------------------\*/


/\* <DEPRECATED> \*/ .p-Widget, /\* </DEPRECATED> \*/
.lm-Widget {
 box-sizing: border-box;
 position: relative;
 overflow: hidden;
 cursor: default;
}


/\* <DEPRECATED> \*/ .p-Widget.p-mod-hidden, /\* </DEPRECATED> \*/
.lm-Widget.lm-mod-hidden {
 display: none !important;
}

/\*-----------------------------------------------------------------------------
| Copyright (c) Jupyter Development Team.
| Copyright (c) 2014-2017, PhosphorJS Contributors
|
| Distributed under the terms of the BSD 3-Clause License.
|
| The full license is in the file LICENSE, distributed with this software.
|----------------------------------------------------------------------------\*/


/\* <DEPRECATED> \*/ .p-CommandPalette, /\* </DEPRECATED> \*/
.lm-CommandPalette {
 display: flex;
 flex-direction: column;
 -webkit-user-select: none;
 -moz-user-select: none;
 -ms-user-select: none;
 user-select: none;
}


/\* <DEPRECATED> \*/ .p-CommandPalette-search, /\* </DEPRECATED> \*/
.lm-CommandPalette-search {
 flex: 0 0 auto;
}


/\* <DEPRECATED> \*/ .p-CommandPalette-content, /\* </DEPRECATED> \*/
.lm-CommandPalette-content {
 flex: 1 1 auto;
 margin: 0;
 padding: 0;
 min-height: 0;
 overflow: auto;
 list-style-type: none;
}


/\* <DEPRECATED> \*/ .p-CommandPalette-header, /\* </DEPRECATED> \*/
.lm-CommandPalette-header {
 overflow: hidden;
 white-space: nowrap;
 text-overflow: ellipsis;
}


/\* <DEPRECATED> \*/ .p-CommandPalette-item, /\* </DEPRECATED> \*/
.lm-CommandPalette-item {
 display: flex;
 flex-direction: row;
}


/\* <DEPRECATED> \*/ .p-CommandPalette-itemIcon, /\* </DEPRECATED> \*/
.lm-CommandPalette-itemIcon {
 flex: 0 0 auto;
}


/\* <DEPRECATED> \*/ .p-CommandPalette-itemContent, /\* </DEPRECATED> \*/
.lm-CommandPalette-itemContent {
 flex: 1 1 auto;
 overflow: hidden;
}


/\* <DEPRECATED> \*/ .p-CommandPalette-itemShortcut, /\* </DEPRECATED> \*/
.lm-CommandPalette-itemShortcut {
 flex: 0 0 auto;
}


/\* <DEPRECATED> \*/ .p-CommandPalette-itemLabel, /\* </DEPRECATED> \*/
.lm-CommandPalette-itemLabel {
 overflow: hidden;
 white-space: nowrap;
 text-overflow: ellipsis;
}

.lm-close-icon {
 border:1px solid transparent;
 background-color: transparent;
 position: absolute;
 z-index:1;
 right:3%;
 top: 0;
 bottom: 0;
 margin: auto;
 padding: 7px 0;
 display: none;
 vertical-align: middle;
 outline: 0;
 cursor: pointer;
}
.lm-close-icon:after {
 content: "X";
 display: block;
 width: 15px;
 height: 15px;
 text-align: center;
 color:#000;
 font-weight: normal;
 font-size: 12px;
 cursor: pointer;
}

/\*-----------------------------------------------------------------------------
| Copyright (c) Jupyter Development Team.
| Copyright (c) 2014-2017, PhosphorJS Contributors
|
| Distributed under the terms of the BSD 3-Clause License.
|
| The full license is in the file LICENSE, distributed with this software.
|----------------------------------------------------------------------------\*/


/\* <DEPRECATED> \*/ .p-DockPanel, /\* </DEPRECATED> \*/
.lm-DockPanel {
 z-index: 0;
}


/\* <DEPRECATED> \*/ .p-DockPanel-widget, /\* </DEPRECATED> \*/
.lm-DockPanel-widget {
 z-index: 0;
}


/\* <DEPRECATED> \*/ .p-DockPanel-tabBar, /\* </DEPRECATED> \*/
.lm-DockPanel-tabBar {
 z-index: 1;
}


/\* <DEPRECATED> \*/ .p-DockPanel-handle, /\* </DEPRECATED> \*/
.lm-DockPanel-handle {
 z-index: 2;
}


/\* <DEPRECATED> \*/ .p-DockPanel-handle.p-mod-hidden, /\* </DEPRECATED> \*/
.lm-DockPanel-handle.lm-mod-hidden {
 display: none !important;
}


/\* <DEPRECATED> \*/ .p-DockPanel-handle:after, /\* </DEPRECATED> \*/
.lm-DockPanel-handle:after {
 position: absolute;
 top: 0;
 left: 0;
 width: 100%;
 height: 100%;
 content: '';
}


/\* <DEPRECATED> \*/
.p-DockPanel-handle[data-orientation='horizontal'],
/\* </DEPRECATED> \*/
.lm-DockPanel-handle[data-orientation='horizontal'] {
 cursor: ew-resize;
}


/\* <DEPRECATED> \*/
.p-DockPanel-handle[data-orientation='vertical'],
/\* </DEPRECATED> \*/
.lm-DockPanel-handle[data-orientation='vertical'] {
 cursor: ns-resize;
}


/\* <DEPRECATED> \*/
.p-DockPanel-handle[data-orientation='horizontal']:after,
/\* </DEPRECATED> \*/
.lm-DockPanel-handle[data-orientation='horizontal']:after {
 left: 50%;
 min-width: 8px;
 transform: translateX(-50%);
}


/\* <DEPRECATED> \*/
.p-DockPanel-handle[data-orientation='vertical']:after,
/\* </DEPRECATED> \*/
.lm-DockPanel-handle[data-orientation='vertical']:after {
 top: 50%;
 min-height: 8px;
 transform: translateY(-50%);
}


/\* <DEPRECATED> \*/ .p-DockPanel-overlay, /\* </DEPRECATED> \*/
.lm-DockPanel-overlay {
 z-index: 3;
 box-sizing: border-box;
 pointer-events: none;
}


/\* <DEPRECATED> \*/ .p-DockPanel-overlay.p-mod-hidden, /\* </DEPRECATED> \*/
.lm-DockPanel-overlay.lm-mod-hidden {
 display: none !important;
}

/\*-----------------------------------------------------------------------------
| Copyright (c) Jupyter Development Team.
| Copyright (c) 2014-2017, PhosphorJS Contributors
|
| Distributed under the terms of the BSD 3-Clause License.
|
| The full license is in the file LICENSE, distributed with this software.
|----------------------------------------------------------------------------\*/


/\* <DEPRECATED> \*/ .p-Menu, /\* </DEPRECATED> \*/
.lm-Menu {
 z-index: 10000;
 position: absolute;
 white-space: nowrap;
 overflow-x: hidden;
 overflow-y: auto;
 outline: none;
 -webkit-user-select: none;
 -moz-user-select: none;
 -ms-user-select: none;
 user-select: none;
}


/\* <DEPRECATED> \*/ .p-Menu-content, /\* </DEPRECATED> \*/
.lm-Menu-content {
 margin: 0;
 padding: 0;
 display: table;
 list-style-type: none;
}


/\* <DEPRECATED> \*/ .p-Menu-item, /\* </DEPRECATED> \*/
.lm-Menu-item {
 display: table-row;
}


/\* <DEPRECATED> \*/
.p-Menu-item.p-mod-hidden,
.p-Menu-item.p-mod-collapsed,
/\* </DEPRECATED> \*/
.lm-Menu-item.lm-mod-hidden,
.lm-Menu-item.lm-mod-collapsed {
 display: none !important;
}


/\* <DEPRECATED> \*/
.p-Menu-itemIcon,
.p-Menu-itemSubmenuIcon,
/\* </DEPRECATED> \*/
.lm-Menu-itemIcon,
.lm-Menu-itemSubmenuIcon {
 display: table-cell;
 text-align: center;
}


/\* <DEPRECATED> \*/ .p-Menu-itemLabel, /\* </DEPRECATED> \*/
.lm-Menu-itemLabel {
 display: table-cell;
 text-align: left;
}


/\* <DEPRECATED> \*/ .p-Menu-itemShortcut, /\* </DEPRECATED> \*/
.lm-Menu-itemShortcut {
 display: table-cell;
 text-align: right;
}

/\*-----------------------------------------------------------------------------
| Copyright (c) Jupyter Development Team.
| Copyright (c) 2014-2017, PhosphorJS Contributors
|
| Distributed under the terms of the BSD 3-Clause License.
|
| The full license is in the file LICENSE, distributed with this software.
|----------------------------------------------------------------------------\*/


/\* <DEPRECATED> \*/ .p-MenuBar, /\* </DEPRECATED> \*/
.lm-MenuBar {
 outline: none;
 -webkit-user-select: none;
 -moz-user-select: none;
 -ms-user-select: none;
 user-select: none;
}


/\* <DEPRECATED> \*/ .p-MenuBar-content, /\* </DEPRECATED> \*/
.lm-MenuBar-content {
 margin: 0;
 padding: 0;
 display: flex;
 flex-direction: row;
 list-style-type: none;
}


/\* <DEPRECATED> \*/ .p--MenuBar-item, /\* </DEPRECATED> \*/
.lm-MenuBar-item {
 box-sizing: border-box;
}


/\* <DEPRECATED> \*/
.p-MenuBar-itemIcon,
.p-MenuBar-itemLabel,
/\* </DEPRECATED> \*/
.lm-MenuBar-itemIcon,
.lm-MenuBar-itemLabel {
 display: inline-block;
}

/\*-----------------------------------------------------------------------------
| Copyright (c) Jupyter Development Team.
| Copyright (c) 2014-2017, PhosphorJS Contributors
|
| Distributed under the terms of the BSD 3-Clause License.
|
| The full license is in the file LICENSE, distributed with this software.
|----------------------------------------------------------------------------\*/


/\* <DEPRECATED> \*/ .p-ScrollBar, /\* </DEPRECATED> \*/
.lm-ScrollBar {
 display: flex;
 -webkit-user-select: none;
 -moz-user-select: none;
 -ms-user-select: none;
 user-select: none;
}


/\* <DEPRECATED> \*/
.p-ScrollBar[data-orientation='horizontal'],
/\* </DEPRECATED> \*/
.lm-ScrollBar[data-orientation='horizontal'] {
 flex-direction: row;
}


/\* <DEPRECATED> \*/
.p-ScrollBar[data-orientation='vertical'],
/\* </DEPRECATED> \*/
.lm-ScrollBar[data-orientation='vertical'] {
 flex-direction: column;
}


/\* <DEPRECATED> \*/ .p-ScrollBar-button, /\* </DEPRECATED> \*/
.lm-ScrollBar-button {
 box-sizing: border-box;
 flex: 0 0 auto;
}


/\* <DEPRECATED> \*/ .p-ScrollBar-track, /\* </DEPRECATED> \*/
.lm-ScrollBar-track {
 box-sizing: border-box;
 position: relative;
 overflow: hidden;
 flex: 1 1 auto;
}


/\* <DEPRECATED> \*/ .p-ScrollBar-thumb, /\* </DEPRECATED> \*/
.lm-ScrollBar-thumb {
 box-sizing: border-box;
 position: absolute;
}

/\*-----------------------------------------------------------------------------
| Copyright (c) Jupyter Development Team.
| Copyright (c) 2014-2017, PhosphorJS Contributors
|
| Distributed under the terms of the BSD 3-Clause License.
|
| The full license is in the file LICENSE, distributed with this software.
|----------------------------------------------------------------------------\*/


/\* <DEPRECATED> \*/ .p-SplitPanel-child, /\* </DEPRECATED> \*/
.lm-SplitPanel-child {
 z-index: 0;
}


/\* <DEPRECATED> \*/ .p-SplitPanel-handle, /\* </DEPRECATED> \*/
.lm-SplitPanel-handle {
 z-index: 1;
}


/\* <DEPRECATED> \*/ .p-SplitPanel-handle.p-mod-hidden, /\* </DEPRECATED> \*/
.lm-SplitPanel-handle.lm-mod-hidden {
 display: none !important;
}


/\* <DEPRECATED> \*/ .p-SplitPanel-handle:after, /\* </DEPRECATED> \*/
.lm-SplitPanel-handle:after {
 position: absolute;
 top: 0;
 left: 0;
 width: 100%;
 height: 100%;
 content: '';
}


/\* <DEPRECATED> \*/
.p-SplitPanel[data-orientation='horizontal'] > .p-SplitPanel-handle,
/\* </DEPRECATED> \*/
.lm-SplitPanel[data-orientation='horizontal'] > .lm-SplitPanel-handle {
 cursor: ew-resize;
}


/\* <DEPRECATED> \*/
.p-SplitPanel[data-orientation='vertical'] > .p-SplitPanel-handle,
/\* </DEPRECATED> \*/
.lm-SplitPanel[data-orientation='vertical'] > .lm-SplitPanel-handle {
 cursor: ns-resize;
}


/\* <DEPRECATED> \*/
.p-SplitPanel[data-orientation='horizontal'] > .p-SplitPanel-handle:after,
/\* </DEPRECATED> \*/
.lm-SplitPanel[data-orientation='horizontal'] > .lm-SplitPanel-handle:after {
 left: 50%;
 min-width: 8px;
 transform: translateX(-50%);
}


/\* <DEPRECATED> \*/
.p-SplitPanel[data-orientation='vertical'] > .p-SplitPanel-handle:after,
/\* </DEPRECATED> \*/
.lm-SplitPanel[data-orientation='vertical'] > .lm-SplitPanel-handle:after {
 top: 50%;
 min-height: 8px;
 transform: translateY(-50%);
}

/\*-----------------------------------------------------------------------------
| Copyright (c) Jupyter Development Team.
| Copyright (c) 2014-2017, PhosphorJS Contributors
|
| Distributed under the terms of the BSD 3-Clause License.
|
| The full license is in the file LICENSE, distributed with this software.
|----------------------------------------------------------------------------\*/


/\* <DEPRECATED> \*/ .p-TabBar, /\* </DEPRECATED> \*/
.lm-TabBar {
 display: flex;
 -webkit-user-select: none;
 -moz-user-select: none;
 -ms-user-select: none;
 user-select: none;
}


/\* <DEPRECATED> \*/ .p-TabBar[data-orientation='horizontal'], /\* </DEPRECATED> \*/
.lm-TabBar[data-orientation='horizontal'] {
 flex-direction: row;
 align-items: flex-end;
}


/\* <DEPRECATED> \*/ .p-TabBar[data-orientation='vertical'], /\* </DEPRECATED> \*/
.lm-TabBar[data-orientation='vertical'] {
 flex-direction: column;
 align-items: flex-end;
}


/\* <DEPRECATED> \*/ .p-TabBar-content, /\* </DEPRECATED> \*/
.lm-TabBar-content {
 margin: 0;
 padding: 0;
 display: flex;
 flex: 1 1 auto;
 list-style-type: none;
}


/\* <DEPRECATED> \*/
.p-TabBar[data-orientation='horizontal'] > .p-TabBar-content,
/\* </DEPRECATED> \*/
.lm-TabBar[data-orientation='horizontal'] > .lm-TabBar-content {
 flex-direction: row;
}


/\* <DEPRECATED> \*/
.p-TabBar[data-orientation='vertical'] > .p-TabBar-content,
/\* </DEPRECATED> \*/
.lm-TabBar[data-orientation='vertical'] > .lm-TabBar-content {
 flex-direction: column;
}


/\* <DEPRECATED> \*/ .p-TabBar-tab, /\* </DEPRECATED> \*/
.lm-TabBar-tab {
 display: flex;
 flex-direction: row;
 box-sizing: border-box;
 overflow: hidden;
}


/\* <DEPRECATED> \*/
.p-TabBar-tabIcon,
.p-TabBar-tabCloseIcon,
/\* </DEPRECATED> \*/
.lm-TabBar-tabIcon,
.lm-TabBar-tabCloseIcon {
 flex: 0 0 auto;
}


/\* <DEPRECATED> \*/ .p-TabBar-tabLabel, /\* </DEPRECATED> \*/
.lm-TabBar-tabLabel {
 flex: 1 1 auto;
 overflow: hidden;
 white-space: nowrap;
}


.lm-TabBar-tabInput {
 user-select: all;
 width: 100%;
 box-sizing : border-box;
}


/\* <DEPRECATED> \*/ .p-TabBar-tab.p-mod-hidden, /\* </DEPRECATED> \*/
.lm-TabBar-tab.lm-mod-hidden {
 display: none !important;
}


.lm-TabBar-addButton.lm-mod-hidden {
 display: none !important;
}


/\* <DEPRECATED> \*/ .p-TabBar.p-mod-dragging .p-TabBar-tab, /\* </DEPRECATED> \*/
.lm-TabBar.lm-mod-dragging .lm-TabBar-tab {
 position: relative;
}


/\* <DEPRECATED> \*/
.p-TabBar.p-mod-dragging[data-orientation='horizontal'] .p-TabBar-tab,
/\* </DEPRECATED> \*/
.lm-TabBar.lm-mod-dragging[data-orientation='horizontal'] .lm-TabBar-tab {
 left: 0;
 transition: left 150ms ease;
}


/\* <DEPRECATED> \*/
.p-TabBar.p-mod-dragging[data-orientation='vertical'] .p-TabBar-tab,
/\* </DEPRECATED> \*/
.lm-TabBar.lm-mod-dragging[data-orientation='vertical'] .lm-TabBar-tab {
 top: 0;
 transition: top 150ms ease;
}


/\* <DEPRECATED> \*/
.p-TabBar.p-mod-dragging .p-TabBar-tab.p-mod-dragging,
/\* </DEPRECATED> \*/
.lm-TabBar.lm-mod-dragging .lm-TabBar-tab.lm-mod-dragging {
 transition: none;
}

.lm-TabBar-tabLabel .lm-TabBar-tabInput {
 user-select: all;
 width: 100%;
 box-sizing : border-box;
 background: inherit;
}

/\*-----------------------------------------------------------------------------
| Copyright (c) Jupyter Development Team.
| Copyright (c) 2014-2017, PhosphorJS Contributors
|
| Distributed under the terms of the BSD 3-Clause License.
|
| The full license is in the file LICENSE, distributed with this software.
|----------------------------------------------------------------------------\*/


/\* <DEPRECATED> \*/ .p-TabPanel-tabBar, /\* </DEPRECATED> \*/
.lm-TabPanel-tabBar {
 z-index: 1;
}


/\* <DEPRECATED> \*/ .p-TabPanel-stackedPanel, /\* </DEPRECATED> \*/
.lm-TabPanel-stackedPanel {
 z-index: 0;
}

/\*-----------------------------------------------------------------------------
| Copyright (c) Jupyter Development Team.
| Copyright (c) 2014-2017, PhosphorJS Contributors
|
| Distributed under the terms of the BSD 3-Clause License.
|
| The full license is in the file LICENSE, distributed with this software.
|----------------------------------------------------------------------------\*/

@charset "UTF-8";
html{
 -webkit-box-sizing:border-box;
 box-sizing:border-box; }

\*,
\*::before,
\*::after{
 -webkit-box-sizing:inherit;
 box-sizing:inherit; }

body{
 font-size:14px;
 font-weight:400;
 letter-spacing:0;
 line-height:1.28581;
 text-transform:none;
 color:#182026;
 font-family:-apple-system, "BlinkMacSystemFont", "Segoe UI", "Roboto", "Oxygen", "Ubuntu", "Cantarell", "Open Sans", "Helvetica Neue", "Icons16", sans-serif; }

p{
 margin-bottom:10px;
 margin-top:0; }

small{
 font-size:12px; }

strong{
 font-weight:600; }

::-moz-selection{
 background:rgba(125, 188, 255, 0.6); }

::selection{
 background:rgba(125, 188, 255, 0.6); }
.bp3-heading{
 color:#182026;
 font-weight:600;
 margin:0 0 10px;
 padding:0; }
 .bp3-dark .bp3-heading{
 color:#f5f8fa; }

h1.bp3-heading, .bp3-running-text h1{
 font-size:36px;
 line-height:40px; }

h2.bp3-heading, .bp3-running-text h2{
 font-size:28px;
 line-height:32px; }

h3.bp3-heading, .bp3-running-text h3{
 font-size:22px;
 line-height:25px; }

h4.bp3-heading, .bp3-running-text h4{
 font-size:18px;
 line-height:21px; }

h5.bp3-heading, .bp3-running-text h5{
 font-size:16px;
 line-height:19px; }

h6.bp3-heading, .bp3-running-text h6{
 font-size:14px;
 line-height:16px; }
.bp3-ui-text{
 font-size:14px;
 font-weight:400;
 letter-spacing:0;
 line-height:1.28581;
 text-transform:none; }

.bp3-monospace-text{
 font-family:monospace;
 text-transform:none; }

.bp3-text-muted{
 color:#5c7080; }
 .bp3-dark .bp3-text-muted{
 color:#a7b6c2; }

.bp3-text-disabled{
 color:rgba(92, 112, 128, 0.6); }
 .bp3-dark .bp3-text-disabled{
 color:rgba(167, 182, 194, 0.6); }

.bp3-text-overflow-ellipsis{
 overflow:hidden;
 text-overflow:ellipsis;
 white-space:nowrap;
 word-wrap:normal; }
.bp3-running-text{
 font-size:14px;
 line-height:1.5; }
 .bp3-running-text h1{
 color:#182026;
 font-weight:600;
 margin-bottom:20px;
 margin-top:40px; }
 .bp3-dark .bp3-running-text h1{
 color:#f5f8fa; }
 .bp3-running-text h2{
 color:#182026;
 font-weight:600;
 margin-bottom:20px;
 margin-top:40px; }
 .bp3-dark .bp3-running-text h2{
 color:#f5f8fa; }
 .bp3-running-text h3{
 color:#182026;
 font-weight:600;
 margin-bottom:20px;
 margin-top:40px; }
 .bp3-dark .bp3-running-text h3{
 color:#f5f8fa; }
 .bp3-running-text h4{
 color:#182026;
 font-weight:600;
 margin-bottom:20px;
 margin-top:40px; }
 .bp3-dark .bp3-running-text h4{
 color:#f5f8fa; }
 .bp3-running-text h5{
 color:#182026;
 font-weight:600;
 margin-bottom:20px;
 margin-top:40px; }
 .bp3-dark .bp3-running-text h5{
 color:#f5f8fa; }
 .bp3-running-text h6{
 color:#182026;
 font-weight:600;
 margin-bottom:20px;
 margin-top:40px; }
 .bp3-dark .bp3-running-text h6{
 color:#f5f8fa; }
 .bp3-running-text hr{
 border:none;
 border-bottom:1px solid rgba(16, 22, 26, 0.15);
 margin:20px 0; }
 .bp3-dark .bp3-running-text hr{
 border-color:rgba(255, 255, 255, 0.15); }
 .bp3-running-text p{
 margin:0 0 10px;
 padding:0; }

.bp3-text-large{
 font-size:16px; }

.bp3-text-small{
 font-size:12px; }
a{
 color:#106ba3;
 text-decoration:none; }
 a:hover{
 color:#106ba3;
 cursor:pointer;
 text-decoration:underline; }
 a .bp3-icon, a .bp3-icon-standard, a .bp3-icon-large{
 color:inherit; }
 a code,
 .bp3-dark a code{
 color:inherit; }
 .bp3-dark a,
 .bp3-dark a:hover{
 color:#48aff0; }
 .bp3-dark a .bp3-icon, .bp3-dark a .bp3-icon-standard, .bp3-dark a .bp3-icon-large,
 .bp3-dark a:hover .bp3-icon,
 .bp3-dark a:hover .bp3-icon-standard,
 .bp3-dark a:hover .bp3-icon-large{
 color:inherit; }
.bp3-running-text code, .bp3-code{
 font-family:monospace;
 text-transform:none;
 background:rgba(255, 255, 255, 0.7);
 border-radius:3px;
 -webkit-box-shadow:inset 0 0 0 1px rgba(16, 22, 26, 0.2);
 box-shadow:inset 0 0 0 1px rgba(16, 22, 26, 0.2);
 color:#5c7080;
 font-size:smaller;
 padding:2px 5px; }
 .bp3-dark .bp3-running-text code, .bp3-running-text .bp3-dark code, .bp3-dark .bp3-code{
 background:rgba(16, 22, 26, 0.3);
 -webkit-box-shadow:inset 0 0 0 1px rgba(16, 22, 26, 0.4);
 box-shadow:inset 0 0 0 1px rgba(16, 22, 26, 0.4);
 color:#a7b6c2; }
 .bp3-running-text a > code, a > .bp3-code{
 color:#137cbd; }
 .bp3-dark .bp3-running-text a > code, .bp3-running-text .bp3-dark a > code, .bp3-dark a > .bp3-code{
 color:inherit; }

.bp3-running-text pre, .bp3-code-block{
 font-family:monospace;
 text-transform:none;
 background:rgba(255, 255, 255, 0.7);
 border-radius:3px;
 -webkit-box-shadow:inset 0 0 0 1px rgba(16, 22, 26, 0.15);
 box-shadow:inset 0 0 0 1px rgba(16, 22, 26, 0.15);
 color:#182026;
 display:block;
 font-size:13px;
 line-height:1.4;
 margin:10px 0;
 padding:13px 15px 12px;
 word-break:break-all;
 word-wrap:break-word; }
 .bp3-dark .bp3-running-text pre, .bp3-running-text .bp3-dark pre, .bp3-dark .bp3-code-block{
 background:rgba(16, 22, 26, 0.3);
 -webkit-box-shadow:inset 0 0 0 1px rgba(16, 22, 26, 0.4);
 box-shadow:inset 0 0 0 1px rgba(16, 22, 26, 0.4);
 color:#f5f8fa; }
 .bp3-running-text pre > code, .bp3-code-block > code{
 background:none;
 -webkit-box-shadow:none;
 box-shadow:none;
 color:inherit;
 font-size:inherit;
 padding:0; }

.bp3-running-text kbd, .bp3-key{
 -webkit-box-align:center;
 -ms-flex-align:center;
 align-items:center;
 background:#ffffff;
 border-radius:3px;
 -webkit-box-shadow:0 0 0 1px rgba(16, 22, 26, 0.1), 0 0 0 rgba(16, 22, 26, 0), 0 1px 1px rgba(16, 22, 26, 0.2);
 box-shadow:0 0 0 1px rgba(16, 22, 26, 0.1), 0 0 0 rgba(16, 22, 26, 0), 0 1px 1px rgba(16, 22, 26, 0.2);
 color:#5c7080;
 display:-webkit-inline-box;
 display:-ms-inline-flexbox;
 display:inline-flex;
 font-family:inherit;
 font-size:12px;
 height:24px;
 -webkit-box-pack:center;
 -ms-flex-pack:center;
 justify-content:center;
 line-height:24px;
 min-width:24px;
 padding:3px 6px;
 vertical-align:middle; }
 .bp3-running-text kbd .bp3-icon, .bp3-key .bp3-icon, .bp3-running-text kbd .bp3-icon-standard, .bp3-key .bp3-icon-standard, .bp3-running-text kbd .bp3-icon-large, .bp3-key .bp3-icon-large{
 margin-right:5px; }
 .bp3-dark .bp3-running-text kbd, .bp3-running-text .bp3-dark kbd, .bp3-dark .bp3-key{
 background:#394b59;
 -webkit-box-shadow:0 0 0 1px rgba(16, 22, 26, 0.2), 0 0 0 rgba(16, 22, 26, 0), 0 1px 1px rgba(16, 22, 26, 0.4);
 box-shadow:0 0 0 1px rgba(16, 22, 26, 0.2), 0 0 0 rgba(16, 22, 26, 0), 0 1px 1px rgba(16, 22, 26, 0.4);
 color:#a7b6c2; }
.bp3-running-text blockquote, .bp3-blockquote{
 border-left:solid 4px rgba(167, 182, 194, 0.5);
 margin:0 0 10px;
 padding:0 20px; }
 .bp3-dark .bp3-running-text blockquote, .bp3-running-text .bp3-dark blockquote, .bp3-dark .bp3-blockquote{
 border-color:rgba(115, 134, 148, 0.5); }
.bp3-running-text ul,
.bp3-running-text ol, .bp3-list{
 margin:10px 0;
 padding-left:30px; }
 .bp3-running-text ul li:not(:last-child), .bp3-running-text ol li:not(:last-child), .bp3-list li:not(:last-child){
 margin-bottom:5px; }
 .bp3-running-text ul ol, .bp3-running-text ol ol, .bp3-list ol,
 .bp3-running-text ul ul,
 .bp3-running-text ol ul,
 .bp3-list ul{
 margin-top:5px; }

.bp3-list-unstyled{
 list-style:none;
 margin:0;
 padding:0; }
 .bp3-list-unstyled li{
 padding:0; }
.bp3-rtl{
 text-align:right; }

.bp3-dark{
 color:#f5f8fa; }

:focus{
 outline:rgba(19, 124, 189, 0.6) auto 2px;
 outline-offset:2px;
 -moz-outline-radius:6px; }

.bp3-focus-disabled :focus{
 outline:none !important; }
 .bp3-focus-disabled :focus ~ .bp3-control-indicator{
 outline:none !important; }

.bp3-alert{
 max-width:400px;
 padding:20px; }

.bp3-alert-body{
 display:-webkit-box;
 display:-ms-flexbox;
 display:flex; }
 .bp3-alert-body .bp3-icon{
 font-size:40px;
 margin-right:20px;
 margin-top:0; }

.bp3-alert-contents{
 word-break:break-word; }

.bp3-alert-footer{
 display:-webkit-box;
 display:-ms-flexbox;
 display:flex;
 -webkit-box-orient:horizontal;
 -webkit-box-direction:reverse;
 -ms-flex-direction:row-reverse;
 flex-direction:row-reverse;
 margin-top:10px; }
 .bp3-alert-footer .bp3-button{
 margin-left:10px; }
.bp3-breadcrumbs{
 -webkit-box-align:center;
 -ms-flex-align:center;
 align-items:center;
 cursor:default;
 display:-webkit-box;
 display:-ms-flexbox;
 display:flex;
 -ms-flex-wrap:wrap;
 flex-wrap:wrap;
 height:30px;
 list-style:none;
 margin:0;
 padding:0; }
 .bp3-breadcrumbs > li{
 -webkit-box-align:center;
 -ms-flex-align:center;
 align-items:center;
 display:-webkit-box;
 display:-ms-flexbox;
 display:flex; }
 .bp3-breadcrumbs > li::after{
 background:url("data:image/svg+xml,%3csvg xmlns='http://www.w3.org/2000/svg' viewBox='0 0 16 16'%3e%3cpath fill-rule='evenodd' clip-rule='evenodd' d='M10.71 7.29l-4-4a1.003 1.003 0 00-1.42 1.42L8.59 8 5.3 11.29c-.19.18-.3.43-.3.71a1.003 1.003 0 001.71.71l4-4c.18-.18.29-.43.29-.71 0-.28-.11-.53-.29-.71z' fill='%235C7080'/%3e%3c/svg%3e");
 content:"";
 display:block;
 height:16px;
 margin:0 5px;
 width:16px; }
 .bp3-breadcrumbs > li:last-of-type::after{
 display:none; }

.bp3-breadcrumb,
.bp3-breadcrumb-current,
.bp3-breadcrumbs-collapsed{
 -webkit-box-align:center;
 -ms-flex-align:center;
 align-items:center;
 display:-webkit-inline-box;
 display:-ms-inline-flexbox;
 display:inline-flex;
 font-size:16px; }

.bp3-breadcrumb,
.bp3-breadcrumbs-collapsed{
 color:#5c7080; }

.bp3-breadcrumb:hover{
 text-decoration:none; }

.bp3-breadcrumb.bp3-disabled{
 color:rgba(92, 112, 128, 0.6);
 cursor:not-allowed; }

.bp3-breadcrumb .bp3-icon{
 margin-right:5px; }

.bp3-breadcrumb-current{
 color:inherit;
 font-weight:600; }
 .bp3-breadcrumb-current .bp3-input{
 font-size:inherit;
 font-weight:inherit;
 vertical-align:baseline; }

.bp3-breadcrumbs-collapsed{
 background:#ced9e0;
 border:none;
 border-radius:3px;
 cursor:pointer;
 margin-right:2px;
 padding:1px 5px;
 vertical-align:text-bottom; }
 .bp3-breadcrumbs-collapsed::before{
 background:url("data:image/svg+xml,%3csvg xmlns='http://www.w3.org/2000/svg' viewBox='0 0 16 16'%3e%3cg fill='%235C7080'%3e%3ccircle cx='2' cy='8.03' r='2'/%3e%3ccircle cx='14' cy='8.03' r='2'/%3e%3ccircle cx='8' cy='8.03' r='2'/%3e%3c/g%3e%3c/svg%3e") center no-repeat;
 content:"";
 display:block;
 height:16px;
 width:16px; }
 .bp3-breadcrumbs-collapsed:hover{
 background:#bfccd6;
 color:#182026;
 text-decoration:none; }

.bp3-dark .bp3-breadcrumb,
.bp3-dark .bp3-breadcrumbs-collapsed{
 color:#a7b6c2; }

.bp3-dark .bp3-breadcrumbs > li::after{
 color:#a7b6c2; }

.bp3-dark .bp3-breadcrumb.bp3-disabled{
 color:rgba(167, 182, 194, 0.6); }

.bp3-dark .bp3-breadcrumb-current{
 color:#f5f8fa; }

.bp3-dark .bp3-breadcrumbs-collapsed{
 background:rgba(16, 22, 26, 0.4); }
 .bp3-dark .bp3-breadcrumbs-collapsed:hover{
 background:rgba(16, 22, 26, 0.6);
 color:#f5f8fa; }
.bp3-button{
 display:-webkit-inline-box;
 display:-ms-inline-flexbox;
 display:inline-flex;
 -webkit-box-orient:horizontal;
 -webkit-box-direction:normal;
 -ms-flex-direction:row;
 flex-direction:row;
 -webkit-box-align:center;
 -ms-flex-align:center;
 align-items:center;
 border:none;
 border-radius:3px;
 cursor:pointer;
 font-size:14px;
 -webkit-box-pack:center;
 -ms-flex-pack:center;
 justify-content:center;
 padding:5px 10px;
 text-align:left;
 vertical-align:middle;
 min-height:30px;
 min-width:30px; }
 .bp3-button > \*{
 -webkit-box-flex:0;
 -ms-flex-positive:0;
 flex-grow:0;
 -ms-flex-negative:0;
 flex-shrink:0; }
 .bp3-button > .bp3-fill{
 -webkit-box-flex:1;
 -ms-flex-positive:1;
 flex-grow:1;
 -ms-flex-negative:1;
 flex-shrink:1; }
 .bp3-button::before,
 .bp3-button > \*{
 margin-right:7px; }
 .bp3-button:empty::before,
 .bp3-button > :last-child{
 margin-right:0; }
 .bp3-button:empty{
 padding:0 !important; }
 .bp3-button:disabled, .bp3-button.bp3-disabled{
 cursor:not-allowed; }
 .bp3-button.bp3-fill{
 display:-webkit-box;
 display:-ms-flexbox;
 display:flex;
 width:100%; }
 .bp3-button.bp3-align-right,
 .bp3-align-right .bp3-button{
 text-align:right; }
 .bp3-button.bp3-align-left,
 .bp3-align-left .bp3-button{
 text-align:left; }
 .bp3-button:not([class\*="bp3-intent-"]){
 background-color:#f5f8fa;
 background-image:-webkit-gradient(linear, left top, left bottom, from(rgba(255, 255, 255, 0.8)), to(rgba(255, 255, 255, 0)));
 background-image:linear-gradient(to bottom, rgba(255, 255, 255, 0.8), rgba(255, 255, 255, 0));
 -webkit-box-shadow:inset 0 0 0 1px rgba(16, 22, 26, 0.2), inset 0 -1px 0 rgba(16, 22, 26, 0.1);
 box-shadow:inset 0 0 0 1px rgba(16, 22, 26, 0.2), inset 0 -1px 0 rgba(16, 22, 26, 0.1);
 color:#182026; }
 .bp3-button:not([class\*="bp3-intent-"]):hover{
 background-clip:padding-box;
 background-color:#ebf1f5;
 -webkit-box-shadow:inset 0 0 0 1px rgba(16, 22, 26, 0.2), inset 0 -1px 0 rgba(16, 22, 26, 0.1);
 box-shadow:inset 0 0 0 1px rgba(16, 22, 26, 0.2), inset 0 -1px 0 rgba(16, 22, 26, 0.1); }
 .bp3-button:not([class\*="bp3-intent-"]):active, .bp3-button:not([class\*="bp3-intent-"]).bp3-active{
 background-color:#d8e1e8;
 background-image:none;
 -webkit-box-shadow:inset 0 0 0 1px rgba(16, 22, 26, 0.2), inset 0 1px 2px rgba(16, 22, 26, 0.2);
 box-shadow:inset 0 0 0 1px rgba(16, 22, 26, 0.2), inset 0 1px 2px rgba(16, 22, 26, 0.2); }
 .bp3-button:not([class\*="bp3-intent-"]):disabled, .bp3-button:not([class\*="bp3-intent-"]).bp3-disabled{
 background-color:rgba(206, 217, 224, 0.5);
 background-image:none;
 -webkit-box-shadow:none;
 box-shadow:none;
 color:rgba(92, 112, 128, 0.6);
 cursor:not-allowed;
 outline:none; }
 .bp3-button:not([class\*="bp3-intent-"]):disabled.bp3-active, .bp3-button:not([class\*="bp3-intent-"]):disabled.bp3-active:hover, .bp3-button:not([class\*="bp3-intent-"]).bp3-disabled.bp3-active, .bp3-button:not([class\*="bp3-intent-"]).bp3-disabled.bp3-active:hover{
 background:rgba(206, 217, 224, 0.7); }
 .bp3-button.bp3-intent-primary{
 background-color:#137cbd;
 background-image:-webkit-gradient(linear, left top, left bottom, from(rgba(255, 255, 255, 0.1)), to(rgba(255, 255, 255, 0)));
 background-image:linear-gradient(to bottom, rgba(255, 255, 255, 0.1), rgba(255, 255, 255, 0));
 -webkit-box-shadow:inset 0 0 0 1px rgba(16, 22, 26, 0.4), inset 0 -1px 0 rgba(16, 22, 26, 0.2);
 box-shadow:inset 0 0 0 1px rgba(16, 22, 26, 0.4), inset 0 -1px 0 rgba(16, 22, 26, 0.2);
 color:#ffffff; }
 .bp3-button.bp3-intent-primary:hover, .bp3-button.bp3-intent-primary:active, .bp3-button.bp3-intent-primary.bp3-active{
 color:#ffffff; }
 .bp3-button.bp3-intent-primary:hover{
 background-color:#106ba3;
 -webkit-box-shadow:inset 0 0 0 1px rgba(16, 22, 26, 0.4), inset 0 -1px 0 rgba(16, 22, 26, 0.2);
 box-shadow:inset 0 0 0 1px rgba(16, 22, 26, 0.4), inset 0 -1px 0 rgba(16, 22, 26, 0.2); }
 .bp3-button.bp3-intent-primary:active, .bp3-button.bp3-intent-primary.bp3-active{
 background-color:#0e5a8a;
 background-image:none;
 -webkit-box-shadow:inset 0 0 0 1px rgba(16, 22, 26, 0.4), inset 0 1px 2px rgba(16, 22, 26, 0.2);
 box-shadow:inset 0 0 0 1px rgba(16, 22, 26, 0.4), inset 0 1px 2px rgba(16, 22, 26, 0.2); }
 .bp3-button.bp3-intent-primary:disabled, .bp3-button.bp3-intent-primary.bp3-disabled{
 background-color:rgba(19, 124, 189, 0.5);
 background-image:none;
 border-color:transparent;
 -webkit-box-shadow:none;
 box-shadow:none;
 color:rgba(255, 255, 255, 0.6); }
 .bp3-button.bp3-intent-success{
 background-color:#0f9960;
 background-image:-webkit-gradient(linear, left top, left bottom, from(rgba(255, 255, 255, 0.1)), to(rgba(255, 255, 255, 0)));
 background-image:linear-gradient(to bottom, rgba(255, 255, 255, 0.1), rgba(255, 255, 255, 0));
 -webkit-box-shadow:inset 0 0 0 1px rgba(16, 22, 26, 0.4), inset 0 -1px 0 rgba(16, 22, 26, 0.2);
 box-shadow:inset 0 0 0 1px rgba(16, 22, 26, 0.4), inset 0 -1px 0 rgba(16, 22, 26, 0.2);
 color:#ffffff; }
 .bp3-button.bp3-intent-success:hover, .bp3-button.bp3-intent-success:active, .bp3-button.bp3-intent-success.bp3-active{
 color:#ffffff; }
 .bp3-button.bp3-intent-success:hover{
 background-color:#0d8050;
 -webkit-box-shadow:inset 0 0 0 1px rgba(16, 22, 26, 0.4), inset 0 -1px 0 rgba(16, 22, 26, 0.2);
 box-shadow:inset 0 0 0 1px rgba(16, 22, 26, 0.4), inset 0 -1px 0 rgba(16, 22, 26, 0.2); }
 .bp3-button.bp3-intent-success:active, .bp3-button.bp3-intent-success.bp3-active{
 background-color:#0a6640;
 background-image:none;
 -webkit-box-shadow:inset 0 0 0 1px rgba(16, 22, 26, 0.4), inset 0 1px 2px rgba(16, 22, 26, 0.2);
 box-shadow:inset 0 0 0 1px rgba(16, 22, 26, 0.4), inset 0 1px 2px rgba(16, 22, 26, 0.2); }
 .bp3-button.bp3-intent-success:disabled, .bp3-button.bp3-intent-success.bp3-disabled{
 background-color:rgba(15, 153, 96, 0.5);
 background-image:none;
 border-color:transparent;
 -webkit-box-shadow:none;
 box-shadow:none;
 color:rgba(255, 255, 255, 0.6); }
 .bp3-button.bp3-intent-warning{
 background-color:#d9822b;
 background-image:-webkit-gradient(linear, left top, left bottom, from(rgba(255, 255, 255, 0.1)), to(rgba(255, 255, 255, 0)));
 background-image:linear-gradient(to bottom, rgba(255, 255, 255, 0.1), rgba(255, 255, 255, 0));
 -webkit-box-shadow:inset 0 0 0 1px rgba(16, 22, 26, 0.4), inset 0 -1px 0 rgba(16, 22, 26, 0.2);
 box-shadow:inset 0 0 0 1px rgba(16, 22, 26, 0.4), inset 0 -1px 0 rgba(16, 22, 26, 0.2);
 color:#ffffff; }
 .bp3-button.bp3-intent-warning:hover, .bp3-button.bp3-intent-warning:active, .bp3-button.bp3-intent-warning.bp3-active{
 color:#ffffff; }
 .bp3-button.bp3-intent-warning:hover{
 background-color:#bf7326;
 -webkit-box-shadow:inset 0 0 0 1px rgba(16, 22, 26, 0.4), inset 0 -1px 0 rgba(16, 22, 26, 0.2);
 box-shadow:inset 0 0 0 1px rgba(16, 22, 26, 0.4), inset 0 -1px 0 rgba(16, 22, 26, 0.2); }
 .bp3-button.bp3-intent-warning:active, .bp3-button.bp3-intent-warning.bp3-active{
 background-color:#a66321;
 background-image:none;
 -webkit-box-shadow:inset 0 0 0 1px rgba(16, 22, 26, 0.4), inset 0 1px 2px rgba(16, 22, 26, 0.2);
 box-shadow:inset 0 0 0 1px rgba(16, 22, 26, 0.4), inset 0 1px 2px rgba(16, 22, 26, 0.2); }
 .bp3-button.bp3-intent-warning:disabled, .bp3-button.bp3-intent-warning.bp3-disabled{
 background-color:rgba(217, 130, 43, 0.5);
 background-image:none;
 border-color:transparent;
 -webkit-box-shadow:none;
 box-shadow:none;
 color:rgba(255, 255, 255, 0.6); }
 .bp3-button.bp3-intent-danger{
 background-color:#db3737;
 background-image:-webkit-gradient(linear, left top, left bottom, from(rgba(255, 255, 255, 0.1)), to(rgba(255, 255, 255, 0)));
 background-image:linear-gradient(to bottom, rgba(255, 255, 255, 0.1), rgba(255, 255, 255, 0));
 -webkit-box-shadow:inset 0 0 0 1px rgba(16, 22, 26, 0.4), inset 0 -1px 0 rgba(16, 22, 26, 0.2);
 box-shadow:inset 0 0 0 1px rgba(16, 22, 26, 0.4), inset 0 -1px 0 rgba(16, 22, 26, 0.2);
 color:#ffffff; }
 .bp3-button.bp3-intent-danger:hover, .bp3-button.bp3-intent-danger:active, .bp3-button.bp3-intent-danger.bp3-active{
 color:#ffffff; }
 .bp3-button.bp3-intent-danger:hover{
 background-color:#c23030;
 -webkit-box-shadow:inset 0 0 0 1px rgba(16, 22, 26, 0.4), inset 0 -1px 0 rgba(16, 22, 26, 0.2);
 box-shadow:inset 0 0 0 1px rgba(16, 22, 26, 0.4), inset 0 -1px 0 rgba(16, 22, 26, 0.2); }
 .bp3-button.bp3-intent-danger:active, .bp3-button.bp3-intent-danger.bp3-active{
 background-color:#a82a2a;
 background-image:none;
 -webkit-box-shadow:inset 0 0 0 1px rgba(16, 22, 26, 0.4), inset 0 1px 2px rgba(16, 22, 26, 0.2);
 box-shadow:inset 0 0 0 1px rgba(16, 22, 26, 0.4), inset 0 1px 2px rgba(16, 22, 26, 0.2); }
 .bp3-button.bp3-intent-danger:disabled, .bp3-button.bp3-intent-danger.bp3-disabled{
 background-color:rgba(219, 55, 55, 0.5);
 background-image:none;
 border-color:transparent;
 -webkit-box-shadow:none;
 box-shadow:none;
 color:rgba(255, 255, 255, 0.6); }
 .bp3-button[class\*="bp3-intent-"] .bp3-button-spinner .bp3-spinner-head{
 stroke:#ffffff; }
 .bp3-button.bp3-large,
 .bp3-large .bp3-button{
 min-height:40px;
 min-width:40px;
 font-size:16px;
 padding:5px 15px; }
 .bp3-button.bp3-large::before,
 .bp3-button.bp3-large > \*,
 .bp3-large .bp3-button::before,
 .bp3-large .bp3-button > \*{
 margin-right:10px; }
 .bp3-button.bp3-large:empty::before,
 .bp3-button.bp3-large > :last-child,
 .bp3-large .bp3-button:empty::before,
 .bp3-large .bp3-button > :last-child{
 margin-right:0; }
 .bp3-button.bp3-small,
 .bp3-small .bp3-button{
 min-height:24px;
 min-width:24px;
 padding:0 7px; }
 .bp3-button.bp3-loading{
 position:relative; }
 .bp3-button.bp3-loading[class\*="bp3-icon-"]::before{
 visibility:hidden; }
 .bp3-button.bp3-loading .bp3-button-spinner{
 margin:0;
 position:absolute; }
 .bp3-button.bp3-loading > :not(.bp3-button-spinner){
 visibility:hidden; }
 .bp3-button[class\*="bp3-icon-"]::before{
 font-family:"Icons16", sans-serif;
 font-size:16px;
 font-style:normal;
 font-weight:400;
 line-height:1;
 -moz-osx-font-smoothing:grayscale;
 -webkit-font-smoothing:antialiased;
 color:#5c7080; }
 .bp3-button .bp3-icon, .bp3-button .bp3-icon-standard, .bp3-button .bp3-icon-large{
 color:#5c7080; }
 .bp3-button .bp3-icon.bp3-align-right, .bp3-button .bp3-icon-standard.bp3-align-right, .bp3-button .bp3-icon-large.bp3-align-right{
 margin-left:7px; }
 .bp3-button .bp3-icon:first-child:last-child,
 .bp3-button .bp3-spinner + .bp3-icon:last-child{
 margin:0 -7px; }
 .bp3-dark .bp3-button:not([class\*="bp3-intent-"]){
 background-color:#394b59;
 background-image:-webkit-gradient(linear, left top, left bottom, from(rgba(255, 255, 255, 0.05)), to(rgba(255, 255, 255, 0)));
 background-image:linear-gradient(to bottom, rgba(255, 255, 255, 0.05), rgba(255, 255, 255, 0));
 -webkit-box-shadow:0 0 0 1px rgba(16, 22, 26, 0.4);
 box-shadow:0 0 0 1px rgba(16, 22, 26, 0.4);
 color:#f5f8fa; }
 .bp3-dark .bp3-button:not([class\*="bp3-intent-"]):hover, .bp3-dark .bp3-button:not([class\*="bp3-intent-"]):active, .bp3-dark .bp3-button:not([class\*="bp3-intent-"]).bp3-active{
 color:#f5f8fa; }
 .bp3-dark .bp3-button:not([class\*="bp3-intent-"]):hover{
 background-color:#30404d;
 -webkit-box-shadow:0 0 0 1px rgba(16, 22, 26, 0.4);
 box-shadow:0 0 0 1px rgba(16, 22, 26, 0.4); }
 .bp3-dark .bp3-button:not([class\*="bp3-intent-"]):active, .bp3-dark .bp3-button:not([class\*="bp3-intent-"]).bp3-active{
 background-color:#202b33;
 background-image:none;
 -webkit-box-shadow:0 0 0 1px rgba(16, 22, 26, 0.6), inset 0 1px 2px rgba(16, 22, 26, 0.2);
 box-shadow:0 0 0 1px rgba(16, 22, 26, 0.6), inset 0 1px 2px rgba(16, 22, 26, 0.2); }
 .bp3-dark .bp3-button:not([class\*="bp3-intent-"]):disabled, .bp3-dark .bp3-button:not([class\*="bp3-intent-"]).bp3-disabled{
 background-color:rgba(57, 75, 89, 0.5);
 background-image:none;
 -webkit-box-shadow:none;
 box-shadow:none;
 color:rgba(167, 182, 194, 0.6); }
 .bp3-dark .bp3-button:not([class\*="bp3-intent-"]):disabled.bp3-active, .bp3-dark .bp3-button:not([class\*="bp3-intent-"]).bp3-disabled.bp3-active{
 background:rgba(57, 75, 89, 0.7); }
 .bp3-dark .bp3-button:not([class\*="bp3-intent-"]) .bp3-button-spinner .bp3-spinner-head{
 background:rgba(16, 22, 26, 0.5);
 stroke:#8a9ba8; }
 .bp3-dark .bp3-button:not([class\*="bp3-intent-"])[class\*="bp3-icon-"]::before{
 color:#a7b6c2; }
 .bp3-dark .bp3-button:not([class\*="bp3-intent-"]) .bp3-icon, .bp3-dark .bp3-button:not([class\*="bp3-intent-"]) .bp3-icon-standard, .bp3-dark .bp3-button:not([class\*="bp3-intent-"]) .bp3-icon-large{
 color:#a7b6c2; }
 .bp3-dark .bp3-button[class\*="bp3-intent-"]{
 -webkit-box-shadow:0 0 0 1px rgba(16, 22, 26, 0.4);
 box-shadow:0 0 0 1px rgba(16, 22, 26, 0.4); }
 .bp3-dark .bp3-button[class\*="bp3-intent-"]:hover{
 -webkit-box-shadow:0 0 0 1px rgba(16, 22, 26, 0.4);
 box-shadow:0 0 0 1px rgba(16, 22, 26, 0.4); }
 .bp3-dark .bp3-button[class\*="bp3-intent-"]:active, .bp3-dark .bp3-button[class\*="bp3-intent-"].bp3-active{
 -webkit-box-shadow:0 0 0 1px rgba(16, 22, 26, 0.4), inset 0 1px 2px rgba(16, 22, 26, 0.2);
 box-shadow:0 0 0 1px rgba(16, 22, 26, 0.4), inset 0 1px 2px rgba(16, 22, 26, 0.2); }
 .bp3-dark .bp3-button[class\*="bp3-intent-"]:disabled, .bp3-dark .bp3-button[class\*="bp3-intent-"].bp3-disabled{
 background-image:none;
 -webkit-box-shadow:none;
 box-shadow:none;
 color:rgba(255, 255, 255, 0.3); }
 .bp3-dark .bp3-button[class\*="bp3-intent-"] .bp3-button-spinner .bp3-spinner-head{
 stroke:#8a9ba8; }
 .bp3-button:disabled::before,
 .bp3-button:disabled .bp3-icon, .bp3-button:disabled .bp3-icon-standard, .bp3-button:disabled .bp3-icon-large, .bp3-button.bp3-disabled::before,
 .bp3-button.bp3-disabled .bp3-icon, .bp3-button.bp3-disabled .bp3-icon-standard, .bp3-button.bp3-disabled .bp3-icon-large, .bp3-button[class\*="bp3-intent-"]::before,
 .bp3-button[class\*="bp3-intent-"] .bp3-icon, .bp3-button[class\*="bp3-intent-"] .bp3-icon-standard, .bp3-button[class\*="bp3-intent-"] .bp3-icon-large{
 color:inherit !important; }
 .bp3-button.bp3-minimal{
 background:none;
 -webkit-box-shadow:none;
 box-shadow:none; }
 .bp3-button.bp3-minimal:hover{
 background:rgba(167, 182, 194, 0.3);
 -webkit-box-shadow:none;
 box-shadow:none;
 color:#182026;
 text-decoration:none; }
 .bp3-button.bp3-minimal:active, .bp3-button.bp3-minimal.bp3-active{
 background:rgba(115, 134, 148, 0.3);
 -webkit-box-shadow:none;
 box-shadow:none;
 color:#182026; }
 .bp3-button.bp3-minimal:disabled, .bp3-button.bp3-minimal:disabled:hover, .bp3-button.bp3-minimal.bp3-disabled, .bp3-button.bp3-minimal.bp3-disabled:hover{
 background:none;
 color:rgba(92, 112, 128, 0.6);
 cursor:not-allowed; }
 .bp3-button.bp3-minimal:disabled.bp3-active, .bp3-button.bp3-minimal:disabled:hover.bp3-active, .bp3-button.bp3-minimal.bp3-disabled.bp3-active, .bp3-button.bp3-minimal.bp3-disabled:hover.bp3-active{
 background:rgba(115, 134, 148, 0.3); }
 .bp3-dark .bp3-button.bp3-minimal{
 background:none;
 -webkit-box-shadow:none;
 box-shadow:none;
 color:inherit; }
 .bp3-dark .bp3-button.bp3-minimal:hover, .bp3-dark .bp3-button.bp3-minimal:active, .bp3-dark .bp3-button.bp3-minimal.bp3-active{
 background:none;
 -webkit-box-shadow:none;
 box-shadow:none; }
 .bp3-dark .bp3-button.bp3-minimal:hover{
 background:rgba(138, 155, 168, 0.15); }
 .bp3-dark .bp3-button.bp3-minimal:active, .bp3-dark .bp3-button.bp3-minimal.bp3-active{
 background:rgba(138, 155, 168, 0.3);
 color:#f5f8fa; }
 .bp3-dark .bp3-button.bp3-minimal:disabled, .bp3-dark .bp3-button.bp3-minimal:disabled:hover, .bp3-dark .bp3-button.bp3-minimal.bp3-disabled, .bp3-dark .bp3-button.bp3-minimal.bp3-disabled:hover{
 background:none;
 color:rgba(167, 182, 194, 0.6);
 cursor:not-allowed; }
 .bp3-dark .bp3-button.bp3-minimal:disabled.bp3-active, .bp3-dark .bp3-button.bp3-minimal:disabled:hover.bp3-active, .bp3-dark .bp3-button.bp3-minimal.bp3-disabled.bp3-active, .bp3-dark .bp3-button.bp3-minimal.bp3-disabled:hover.bp3-active{
 background:rgba(138, 155, 168, 0.3); }
 .bp3-button.bp3-minimal.bp3-intent-primary{
 color:#106ba3; }
 .bp3-button.bp3-minimal.bp3-intent-primary:hover, .bp3-button.bp3-minimal.bp3-intent-primary:active, .bp3-button.bp3-minimal.bp3-intent-primary.bp3-active{
 background:none;
 -webkit-box-shadow:none;
 box-shadow:none;
 color:#106ba3; }
 .bp3-button.bp3-minimal.bp3-intent-primary:hover{
 background:rgba(19, 124, 189, 0.15);
 color:#106ba3; }
 .bp3-button.bp3-minimal.bp3-intent-primary:active, .bp3-button.bp3-minimal.bp3-intent-primary.bp3-active{
 background:rgba(19, 124, 189, 0.3);
 color:#106ba3; }
 .bp3-button.bp3-minimal.bp3-intent-primary:disabled, .bp3-button.bp3-minimal.bp3-intent-primary.bp3-disabled{
 background:none;
 color:rgba(16, 107, 163, 0.5); }
 .bp3-button.bp3-minimal.bp3-intent-primary:disabled.bp3-active, .bp3-button.bp3-minimal.bp3-intent-primary.bp3-disabled.bp3-active{
 background:rgba(19, 124, 189, 0.3); }
 .bp3-button.bp3-minimal.bp3-intent-primary .bp3-button-spinner .bp3-spinner-head{
 stroke:#106ba3; }
 .bp3-dark .bp3-button.bp3-minimal.bp3-intent-primary{
 color:#48aff0; }
 .bp3-dark .bp3-button.bp3-minimal.bp3-intent-primary:hover{
 background:rgba(19, 124, 189, 0.2);
 color:#48aff0; }
 .bp3-dark .bp3-button.bp3-minimal.bp3-intent-primary:active, .bp3-dark .bp3-button.bp3-minimal.bp3-intent-primary.bp3-active{
 background:rgba(19, 124, 189, 0.3);
 color:#48aff0; }
 .bp3-dark .bp3-button.bp3-minimal.bp3-intent-primary:disabled, .bp3-dark .bp3-button.bp3-minimal.bp3-intent-primary.bp3-disabled{
 background:none;
 color:rgba(72, 175, 240, 0.5); }
 .bp3-dark .bp3-button.bp3-minimal.bp3-intent-primary:disabled.bp3-active, .bp3-dark .bp3-button.bp3-minimal.bp3-intent-primary.bp3-disabled.bp3-active{
 background:rgba(19, 124, 189, 0.3); }
 .bp3-button.bp3-minimal.bp3-intent-success{
 color:#0d8050; }
 .bp3-button.bp3-minimal.bp3-intent-success:hover, .bp3-button.bp3-minimal.bp3-intent-success:active, .bp3-button.bp3-minimal.bp3-intent-success.bp3-active{
 background:none;
 -webkit-box-shadow:none;
 box-shadow:none;
 color:#0d8050; }
 .bp3-button.bp3-minimal.bp3-intent-success:hover{
 background:rgba(15, 153, 96, 0.15);
 color:#0d8050; }
 .bp3-button.bp3-minimal.bp3-intent-success:active, .bp3-button.bp3-minimal.bp3-intent-success.bp3-active{
 background:rgba(15, 153, 96, 0.3);
 color:#0d8050; }
 .bp3-button.bp3-minimal.bp3-intent-success:disabled, .bp3-button.bp3-minimal.bp3-intent-success.bp3-disabled{
 background:none;
 color:rgba(13, 128, 80, 0.5); }
 .bp3-button.bp3-minimal.bp3-intent-success:disabled.bp3-active, .bp3-button.bp3-minimal.bp3-intent-success.bp3-disabled.bp3-active{
 background:rgba(15, 153, 96, 0.3); }
 .bp3-button.bp3-minimal.bp3-intent-success .bp3-button-spinner .bp3-spinner-head{
 stroke:#0d8050; }
 .bp3-dark .bp3-button.bp3-minimal.bp3-intent-success{
 color:#3dcc91; }
 .bp3-dark .bp3-button.bp3-minimal.bp3-intent-success:hover{
 background:rgba(15, 153, 96, 0.2);
 color:#3dcc91; }
 .bp3-dark .bp3-button.bp3-minimal.bp3-intent-success:active, .bp3-dark .bp3-button.bp3-minimal.bp3-intent-success.bp3-active{
 background:rgba(15, 153, 96, 0.3);
 color:#3dcc91; }
 .bp3-dark .bp3-button.bp3-minimal.bp3-intent-success:disabled, .bp3-dark .bp3-button.bp3-minimal.bp3-intent-success.bp3-disabled{
 background:none;
 color:rgba(61, 204, 145, 0.5); }
 .bp3-dark .bp3-button.bp3-minimal.bp3-intent-success:disabled.bp3-active, .bp3-dark .bp3-button.bp3-minimal.bp3-intent-success.bp3-disabled.bp3-active{
 background:rgba(15, 153, 96, 0.3); }
 .bp3-button.bp3-minimal.bp3-intent-warning{
 color:#bf7326; }
 .bp3-button.bp3-minimal.bp3-intent-warning:hover, .bp3-button.bp3-minimal.bp3-intent-warning:active, .bp3-button.bp3-minimal.bp3-intent-warning.bp3-active{
 background:none;
 -webkit-box-shadow:none;
 box-shadow:none;
 color:#bf7326; }
 .bp3-button.bp3-minimal.bp3-intent-warning:hover{
 background:rgba(217, 130, 43, 0.15);
 color:#bf7326; }
 .bp3-button.bp3-minimal.bp3-intent-warning:active, .bp3-button.bp3-minimal.bp3-intent-warning.bp3-active{
 background:rgba(217, 130, 43, 0.3);
 color:#bf7326; }
 .bp3-button.bp3-minimal.bp3-intent-warning:disabled, .bp3-button.bp3-minimal.bp3-intent-warning.bp3-disabled{
 background:none;
 color:rgba(191, 115, 38, 0.5); }
 .bp3-button.bp3-minimal.bp3-intent-warning:disabled.bp3-active, .bp3-button.bp3-minimal.bp3-intent-warning.bp3-disabled.bp3-active{
 background:rgba(217, 130, 43, 0.3); }
 .bp3-button.bp3-minimal.bp3-intent-warning .bp3-button-spinner .bp3-spinner-head{
 stroke:#bf7326; }
 .bp3-dark .bp3-button.bp3-minimal.bp3-intent-warning{
 color:#ffb366; }
 .bp3-dark .bp3-button.bp3-minimal.bp3-intent-warning:hover{
 background:rgba(217, 130, 43, 0.2);
 color:#ffb366; }
 .bp3-dark .bp3-button.bp3-minimal.bp3-intent-warning:active, .bp3-dark .bp3-button.bp3-minimal.bp3-intent-warning.bp3-active{
 background:rgba(217, 130, 43, 0.3);
 color:#ffb366; }
 .bp3-dark .bp3-button.bp3-minimal.bp3-intent-warning:disabled, .bp3-dark .bp3-button.bp3-minimal.bp3-intent-warning.bp3-disabled{
 background:none;
 color:rgba(255, 179, 102, 0.5); }
 .bp3-dark .bp3-button.bp3-minimal.bp3-intent-warning:disabled.bp3-active, .bp3-dark .bp3-button.bp3-minimal.bp3-intent-warning.bp3-disabled.bp3-active{
 background:rgba(217, 130, 43, 0.3); }
 .bp3-button.bp3-minimal.bp3-intent-danger{
 color:#c23030; }
 .bp3-button.bp3-minimal.bp3-intent-danger:hover, .bp3-button.bp3-minimal.bp3-intent-danger:active, .bp3-button.bp3-minimal.bp3-intent-danger.bp3-active{
 background:none;
 -webkit-box-shadow:none;
 box-shadow:none;
 color:#c23030; }
 .bp3-button.bp3-minimal.bp3-intent-danger:hover{
 background:rgba(219, 55, 55, 0.15);
 color:#c23030; }
 .bp3-button.bp3-minimal.bp3-intent-danger:active, .bp3-button.bp3-minimal.bp3-intent-danger.bp3-active{
 background:rgba(219, 55, 55, 0.3);
 color:#c23030; }
 .bp3-button.bp3-minimal.bp3-intent-danger:disabled, .bp3-button.bp3-minimal.bp3-intent-danger.bp3-disabled{
 background:none;
 color:rgba(194, 48, 48, 0.5); }
 .bp3-button.bp3-minimal.bp3-intent-danger:disabled.bp3-active, .bp3-button.bp3-minimal.bp3-intent-danger.bp3-disabled.bp3-active{
 background:rgba(219, 55, 55, 0.3); }
 .bp3-button.bp3-minimal.bp3-intent-danger .bp3-button-spinner .bp3-spinner-head{
 stroke:#c23030; }
 .bp3-dark .bp3-button.bp3-minimal.bp3-intent-danger{
 color:#ff7373; }
 .bp3-dark .bp3-button.bp3-minimal.bp3-intent-danger:hover{
 background:rgba(219, 55, 55, 0.2);
 color:#ff7373; }
 .bp3-dark .bp3-button.bp3-minimal.bp3-intent-danger:active, .bp3-dark .bp3-button.bp3-minimal.bp3-intent-danger.bp3-active{
 background:rgba(219, 55, 55, 0.3);
 color:#ff7373; }
 .bp3-dark .bp3-button.bp3-minimal.bp3-intent-danger:disabled, .bp3-dark .bp3-button.bp3-minimal.bp3-intent-danger.bp3-disabled{
 background:none;
 color:rgba(255, 115, 115, 0.5); }
 .bp3-dark .bp3-button.bp3-minimal.bp3-intent-danger:disabled.bp3-active, .bp3-dark .bp3-button.bp3-minimal.bp3-intent-danger.bp3-disabled.bp3-active{
 background:rgba(219, 55, 55, 0.3); }
 .bp3-button.bp3-outlined{
 background:none;
 -webkit-box-shadow:none;
 box-shadow:none;
 border:1px solid rgba(24, 32, 38, 0.2);
 -webkit-box-sizing:border-box;
 box-sizing:border-box; }
 .bp3-button.bp3-outlined:hover{
 background:rgba(167, 182, 194, 0.3);
 -webkit-box-shadow:none;
 box-shadow:none;
 color:#182026;
 text-decoration:none; }
 .bp3-button.bp3-outlined:active, .bp3-button.bp3-outlined.bp3-active{
 background:rgba(115, 134, 148, 0.3);
 -webkit-box-shadow:none;
 box-shadow:none;
 color:#182026; }
 .bp3-button.bp3-outlined:disabled, .bp3-button.bp3-outlined:disabled:hover, .bp3-button.bp3-outlined.bp3-disabled, .bp3-button.bp3-outlined.bp3-disabled:hover{
 background:none;
 color:rgba(92, 112, 128, 0.6);
 cursor:not-allowed; }
 .bp3-button.bp3-outlined:disabled.bp3-active, .bp3-button.bp3-outlined:disabled:hover.bp3-active, .bp3-button.bp3-outlined.bp3-disabled.bp3-active, .bp3-button.bp3-outlined.bp3-disabled:hover.bp3-active{
 background:rgba(115, 134, 148, 0.3); }
 .bp3-dark .bp3-button.bp3-outlined{
 background:none;
 -webkit-box-shadow:none;
 box-shadow:none;
 color:inherit; }
 .bp3-dark .bp3-button.bp3-outlined:hover, .bp3-dark .bp3-button.bp3-outlined:active, .bp3-dark .bp3-button.bp3-outlined.bp3-active{
 background:none;
 -webkit-box-shadow:none;
 box-shadow:none; }
 .bp3-dark .bp3-button.bp3-outlined:hover{
 background:rgba(138, 155, 168, 0.15); }
 .bp3-dark .bp3-button.bp3-outlined:active, .bp3-dark .bp3-button.bp3-outlined.bp3-active{
 background:rgba(138, 155, 168, 0.3);
 color:#f5f8fa; }
 .bp3-dark .bp3-button.bp3-outlined:disabled, .bp3-dark .bp3-button.bp3-outlined:disabled:hover, .bp3-dark .bp3-button.bp3-outlined.bp3-disabled, .bp3-dark .bp3-button.bp3-outlined.bp3-disabled:hover{
 background:none;
 color:rgba(167, 182, 194, 0.6);
 cursor:not-allowed; }
 .bp3-dark .bp3-button.bp3-outlined:disabled.bp3-active, .bp3-dark .bp3-button.bp3-outlined:disabled:hover.bp3-active, .bp3-dark .bp3-button.bp3-outlined.bp3-disabled.bp3-active, .bp3-dark .bp3-button.bp3-outlined.bp3-disabled:hover.bp3-active{
 background:rgba(138, 155, 168, 0.3); }
 .bp3-button.bp3-outlined.bp3-intent-primary{
 color:#106ba3; }
 .bp3-button.bp3-outlined.bp3-intent-primary:hover, .bp3-button.bp3-outlined.bp3-intent-primary:active, .bp3-button.bp3-outlined.bp3-intent-primary.bp3-active{
 background:none;
 -webkit-box-shadow:none;
 box-shadow:none;
 color:#106ba3; }
 .bp3-button.bp3-outlined.bp3-intent-primary:hover{
 background:rgba(19, 124, 189, 0.15);
 color:#106ba3; }
 .bp3-button.bp3-outlined.bp3-intent-primary:active, .bp3-button.bp3-outlined.bp3-intent-primary.bp3-active{
 background:rgba(19, 124, 189, 0.3);
 color:#106ba3; }
 .bp3-button.bp3-outlined.bp3-intent-primary:disabled, .bp3-button.bp3-outlined.bp3-intent-primary.bp3-disabled{
 background:none;
 color:rgba(16, 107, 163, 0.5); }
 .bp3-button.bp3-outlined.bp3-intent-primary:disabled.bp3-active, .bp3-button.bp3-outlined.bp3-intent-primary.bp3-disabled.bp3-active{
 background:rgba(19, 124, 189, 0.3); }
 .bp3-button.bp3-outlined.bp3-intent-primary .bp3-button-spinner .bp3-spinner-head{
 stroke:#106ba3; }
 .bp3-dark .bp3-button.bp3-outlined.bp3-intent-primary{
 color:#48aff0; }
 .bp3-dark .bp3-button.bp3-outlined.bp3-intent-primary:hover{
 background:rgba(19, 124, 189, 0.2);
 color:#48aff0; }
 .bp3-dark .bp3-button.bp3-outlined.bp3-intent-primary:active, .bp3-dark .bp3-button.bp3-outlined.bp3-intent-primary.bp3-active{
 background:rgba(19, 124, 189, 0.3);
 color:#48aff0; }
 .bp3-dark .bp3-button.bp3-outlined.bp3-intent-primary:disabled, .bp3-dark .bp3-button.bp3-outlined.bp3-intent-primary.bp3-disabled{
 background:none;
 color:rgba(72, 175, 240, 0.5); }
 .bp3-dark .bp3-button.bp3-outlined.bp3-intent-primary:disabled.bp3-active, .bp3-dark .bp3-button.bp3-outlined.bp3-intent-primary.bp3-disabled.bp3-active{
 background:rgba(19, 124, 189, 0.3); }
 .bp3-button.bp3-outlined.bp3-intent-success{
 color:#0d8050; }
 .bp3-button.bp3-outlined.bp3-intent-success:hover, .bp3-button.bp3-outlined.bp3-intent-success:active, .bp3-button.bp3-outlined.bp3-intent-success.bp3-active{
 background:none;
 -webkit-box-shadow:none;
 box-shadow:none;
 color:#0d8050; }
 .bp3-button.bp3-outlined.bp3-intent-success:hover{
 background:rgba(15, 153, 96, 0.15);
 color:#0d8050; }
 .bp3-button.bp3-outlined.bp3-intent-success:active, .bp3-button.bp3-outlined.bp3-intent-success.bp3-active{
 background:rgba(15, 153, 96, 0.3);
 color:#0d8050; }
 .bp3-button.bp3-outlined.bp3-intent-success:disabled, .bp3-button.bp3-outlined.bp3-intent-success.bp3-disabled{
 background:none;
 color:rgba(13, 128, 80, 0.5); }
 .bp3-button.bp3-outlined.bp3-intent-success:disabled.bp3-active, .bp3-button.bp3-outlined.bp3-intent-success.bp3-disabled.bp3-active{
 background:rgba(15, 153, 96, 0.3); }
 .bp3-button.bp3-outlined.bp3-intent-success .bp3-button-spinner .bp3-spinner-head{
 stroke:#0d8050; }
 .bp3-dark .bp3-button.bp3-outlined.bp3-intent-success{
 color:#3dcc91; }
 .bp3-dark .bp3-button.bp3-outlined.bp3-intent-success:hover{
 background:rgba(15, 153, 96, 0.2);
 color:#3dcc91; }
 .bp3-dark .bp3-button.bp3-outlined.bp3-intent-success:active, .bp3-dark .bp3-button.bp3-outlined.bp3-intent-success.bp3-active{
 background:rgba(15, 153, 96, 0.3);
 color:#3dcc91; }
 .bp3-dark .bp3-button.bp3-outlined.bp3-intent-success:disabled, .bp3-dark .bp3-button.bp3-outlined.bp3-intent-success.bp3-disabled{
 background:none;
 color:rgba(61, 204, 145, 0.5); }
 .bp3-dark .bp3-button.bp3-outlined.bp3-intent-success:disabled.bp3-active, .bp3-dark .bp3-button.bp3-outlined.bp3-intent-success.bp3-disabled.bp3-active{
 background:rgba(15, 153, 96, 0.3); }
 .bp3-button.bp3-outlined.bp3-intent-warning{
 color:#bf7326; }
 .bp3-button.bp3-outlined.bp3-intent-warning:hover, .bp3-button.bp3-outlined.bp3-intent-warning:active, .bp3-button.bp3-outlined.bp3-intent-warning.bp3-active{
 background:none;
 -webkit-box-shadow:none;
 box-shadow:none;
 color:#bf7326; }
 .bp3-button.bp3-outlined.bp3-intent-warning:hover{
 background:rgba(217, 130, 43, 0.15);
 color:#bf7326; }
 .bp3-button.bp3-outlined.bp3-intent-warning:active, .bp3-button.bp3-outlined.bp3-intent-warning.bp3-active{
 background:rgba(217, 130, 43, 0.3);
 color:#bf7326; }
 .bp3-button.bp3-outlined.bp3-intent-warning:disabled, .bp3-button.bp3-outlined.bp3-intent-warning.bp3-disabled{
 background:none;
 color:rgba(191, 115, 38, 0.5); }
 .bp3-button.bp3-outlined.bp3-intent-warning:disabled.bp3-active, .bp3-button.bp3-outlined.bp3-intent-warning.bp3-disabled.bp3-active{
 background:rgba(217, 130, 43, 0.3); }
 .bp3-button.bp3-outlined.bp3-intent-warning .bp3-button-spinner .bp3-spinner-head{
 stroke:#bf7326; }
 .bp3-dark .bp3-button.bp3-outlined.bp3-intent-warning{
 color:#ffb366; }
 .bp3-dark .bp3-button.bp3-outlined.bp3-intent-warning:hover{
 background:rgba(217, 130, 43, 0.2);
 color:#ffb366; }
 .bp3-dark .bp3-button.bp3-outlined.bp3-intent-warning:active, .bp3-dark .bp3-button.bp3-outlined.bp3-intent-warning.bp3-active{
 background:rgba(217, 130, 43, 0.3);
 color:#ffb366; }
 .bp3-dark .bp3-button.bp3-outlined.bp3-intent-warning:disabled, .bp3-dark .bp3-button.bp3-outlined.bp3-intent-warning.bp3-disabled{
 background:none;
 color:rgba(255, 179, 102, 0.5); }
 .bp3-dark .bp3-button.bp3-outlined.bp3-intent-warning:disabled.bp3-active, .bp3-dark .bp3-button.bp3-outlined.bp3-intent-warning.bp3-disabled.bp3-active{
 background:rgba(217, 130, 43, 0.3); }
 .bp3-button.bp3-outlined.bp3-intent-danger{
 color:#c23030; }
 .bp3-button.bp3-outlined.bp3-intent-danger:hover, .bp3-button.bp3-outlined.bp3-intent-danger:active, .bp3-button.bp3-outlined.bp3-intent-danger.bp3-active{
 background:none;
 -webkit-box-shadow:none;
 box-shadow:none;
 color:#c23030; }
 .bp3-button.bp3-outlined.bp3-intent-danger:hover{
 background:rgba(219, 55, 55, 0.15);
 color:#c23030; }
 .bp3-button.bp3-outlined.bp3-intent-danger:active, .bp3-button.bp3-outlined.bp3-intent-danger.bp3-active{
 background:rgba(219, 55, 55, 0.3);
 color:#c23030; }
 .bp3-button.bp3-outlined.bp3-intent-danger:disabled, .bp3-button.bp3-outlined.bp3-intent-danger.bp3-disabled{
 background:none;
 color:rgba(194, 48, 48, 0.5); }
 .bp3-button.bp3-outlined.bp3-intent-danger:disabled.bp3-active, .bp3-button.bp3-outlined.bp3-intent-danger.bp3-disabled.bp3-active{
 background:rgba(219, 55, 55, 0.3); }
 .bp3-button.bp3-outlined.bp3-intent-danger .bp3-button-spinner .bp3-spinner-head{
 stroke:#c23030; }
 .bp3-dark .bp3-button.bp3-outlined.bp3-intent-danger{
 color:#ff7373; }
 .bp3-dark .bp3-button.bp3-outlined.bp3-intent-danger:hover{
 background:rgba(219, 55, 55, 0.2);
 color:#ff7373; }
 .bp3-dark .bp3-button.bp3-outlined.bp3-intent-danger:active, .bp3-dark .bp3-button.bp3-outlined.bp3-intent-danger.bp3-active{
 background:rgba(219, 55, 55, 0.3);
 color:#ff7373; }
 .bp3-dark .bp3-button.bp3-outlined.bp3-intent-danger:disabled, .bp3-dark .bp3-button.bp3-outlined.bp3-intent-danger.bp3-disabled{
 background:none;
 color:rgba(255, 115, 115, 0.5); }
 .bp3-dark .bp3-button.bp3-outlined.bp3-intent-danger:disabled.bp3-active, .bp3-dark .bp3-button.bp3-outlined.bp3-intent-danger.bp3-disabled.bp3-active{
 background:rgba(219, 55, 55, 0.3); }
 .bp3-button.bp3-outlined:disabled, .bp3-button.bp3-outlined.bp3-disabled, .bp3-button.bp3-outlined:disabled:hover, .bp3-button.bp3-outlined.bp3-disabled:hover{
 border-color:rgba(92, 112, 128, 0.1); }
 .bp3-dark .bp3-button.bp3-outlined{
 border-color:rgba(255, 255, 255, 0.4); }
 .bp3-dark .bp3-button.bp3-outlined:disabled, .bp3-dark .bp3-button.bp3-outlined:disabled:hover, .bp3-dark .bp3-button.bp3-outlined.bp3-disabled, .bp3-dark .bp3-button.bp3-outlined.bp3-disabled:hover{
 border-color:rgba(255, 255, 255, 0.2); }
 .bp3-button.bp3-outlined.bp3-intent-primary{
 border-color:rgba(16, 107, 163, 0.6); }
 .bp3-button.bp3-outlined.bp3-intent-primary:disabled, .bp3-button.bp3-outlined.bp3-intent-primary.bp3-disabled{
 border-color:rgba(16, 107, 163, 0.2); }
 .bp3-dark .bp3-button.bp3-outlined.bp3-intent-primary{
 border-color:rgba(72, 175, 240, 0.6); }
 .bp3-dark .bp3-button.bp3-outlined.bp3-intent-primary:disabled, .bp3-dark .bp3-button.bp3-outlined.bp3-intent-primary.bp3-disabled{
 border-color:rgba(72, 175, 240, 0.2); }
 .bp3-button.bp3-outlined.bp3-intent-success{
 border-color:rgba(13, 128, 80, 0.6); }
 .bp3-button.bp3-outlined.bp3-intent-success:disabled, .bp3-button.bp3-outlined.bp3-intent-success.bp3-disabled{
 border-color:rgba(13, 128, 80, 0.2); }
 .bp3-dark .bp3-button.bp3-outlined.bp3-intent-success{
 border-color:rgba(61, 204, 145, 0.6); }
 .bp3-dark .bp3-button.bp3-outlined.bp3-intent-success:disabled, .bp3-dark .bp3-button.bp3-outlined.bp3-intent-success.bp3-disabled{
 border-color:rgba(61, 204, 145, 0.2); }
 .bp3-button.bp3-outlined.bp3-intent-warning{
 border-color:rgba(191, 115, 38, 0.6); }
 .bp3-button.bp3-outlined.bp3-intent-warning:disabled, .bp3-button.bp3-outlined.bp3-intent-warning.bp3-disabled{
 border-color:rgba(191, 115, 38, 0.2); }
 .bp3-dark .bp3-button.bp3-outlined.bp3-intent-warning{
 border-color:rgba(255, 179, 102, 0.6); }
 .bp3-dark .bp3-button.bp3-outlined.bp3-intent-warning:disabled, .bp3-dark .bp3-button.bp3-outlined.bp3-intent-warning.bp3-disabled{
 border-color:rgba(255, 179, 102, 0.2); }
 .bp3-button.bp3-outlined.bp3-intent-danger{
 border-color:rgba(194, 48, 48, 0.6); }
 .bp3-button.bp3-outlined.bp3-intent-danger:disabled, .bp3-button.bp3-outlined.bp3-intent-danger.bp3-disabled{
 border-color:rgba(194, 48, 48, 0.2); }
 .bp3-dark .bp3-button.bp3-outlined.bp3-intent-danger{
 border-color:rgba(255, 115, 115, 0.6); }
 .bp3-dark .bp3-button.bp3-outlined.bp3-intent-danger:disabled, .bp3-dark .bp3-button.bp3-outlined.bp3-intent-danger.bp3-disabled{
 border-color:rgba(255, 115, 115, 0.2); }

a.bp3-button{
 text-align:center;
 text-decoration:none;
 -webkit-transition:none;
 transition:none; }
 a.bp3-button, a.bp3-button:hover, a.bp3-button:active{
 color:#182026; }
 a.bp3-button.bp3-disabled{
 color:rgba(92, 112, 128, 0.6); }

.bp3-button-text{
 -webkit-box-flex:0;
 -ms-flex:0 1 auto;
 flex:0 1 auto; }

.bp3-button.bp3-align-left .bp3-button-text, .bp3-button.bp3-align-right .bp3-button-text,
.bp3-button-group.bp3-align-left .bp3-button-text,
.bp3-button-group.bp3-align-right .bp3-button-text{
 -webkit-box-flex:1;
 -ms-flex:1 1 auto;
 flex:1 1 auto; }
.bp3-button-group{
 display:-webkit-inline-box;
 display:-ms-inline-flexbox;
 display:inline-flex; }
 .bp3-button-group .bp3-button{
 -webkit-box-flex:0;
 -ms-flex:0 0 auto;
 flex:0 0 auto;
 position:relative;
 z-index:4; }
 .bp3-button-group .bp3-button:focus{
 z-index:5; }
 .bp3-button-group .bp3-button:hover{
 z-index:6; }
 .bp3-button-group .bp3-button:active, .bp3-button-group .bp3-button.bp3-active{
 z-index:7; }
 .bp3-button-group .bp3-button:disabled, .bp3-button-group .bp3-button.bp3-disabled{
 z-index:3; }
 .bp3-button-group .bp3-button[class\*="bp3-intent-"]{
 z-index:9; }
 .bp3-button-group .bp3-button[class\*="bp3-intent-"]:focus{
 z-index:10; }
 .bp3-button-group .bp3-button[class\*="bp3-intent-"]:hover{
 z-index:11; }
 .bp3-button-group .bp3-button[class\*="bp3-intent-"]:active, .bp3-button-group .bp3-button[class\*="bp3-intent-"].bp3-active{
 z-index:12; }
 .bp3-button-group .bp3-button[class\*="bp3-intent-"]:disabled, .bp3-button-group .bp3-button[class\*="bp3-intent-"].bp3-disabled{
 z-index:8; }
 .bp3-button-group:not(.bp3-minimal) > .bp3-popover-wrapper:not(:first-child) .bp3-button,
 .bp3-button-group:not(.bp3-minimal) > .bp3-button:not(:first-child){
 border-bottom-left-radius:0;
 border-top-left-radius:0; }
 .bp3-button-group:not(.bp3-minimal) > .bp3-popover-wrapper:not(:last-child) .bp3-button,
 .bp3-button-group:not(.bp3-minimal) > .bp3-button:not(:last-child){
 border-bottom-right-radius:0;
 border-top-right-radius:0;
 margin-right:-1px; }
 .bp3-button-group.bp3-minimal .bp3-button{
 background:none;
 -webkit-box-shadow:none;
 box-shadow:none; }
 .bp3-button-group.bp3-minimal .bp3-button:hover{
 background:rgba(167, 182, 194, 0.3);
 -webkit-box-shadow:none;
 box-shadow:none;
 color:#182026;
 text-decoration:none; }
 .bp3-button-group.bp3-minimal .bp3-button:active, .bp3-button-group.bp3-minimal .bp3-button.bp3-active{
 background:rgba(115, 134, 148, 0.3);
 -webkit-box-shadow:none;
 box-shadow:none;
 color:#182026; }
 .bp3-button-group.bp3-minimal .bp3-button:disabled, .bp3-button-group.bp3-minimal .bp3-button:disabled:hover, .bp3-button-group.bp3-minimal .bp3-button.bp3-disabled, .bp3-button-group.bp3-minimal .bp3-button.bp3-disabled:hover{
 background:none;
 color:rgba(92, 112, 128, 0.6);
 cursor:not-allowed; }
 .bp3-button-group.bp3-minimal .bp3-button:disabled.bp3-active, .bp3-button-group.bp3-minimal .bp3-button:disabled:hover.bp3-active, .bp3-button-group.bp3-minimal .bp3-button.bp3-disabled.bp3-active, .bp3-button-group.bp3-minimal .bp3-button.bp3-disabled:hover.bp3-active{
 background:rgba(115, 134, 148, 0.3); }
 .bp3-dark .bp3-button-group.bp3-minimal .bp3-button{
 background:none;
 -webkit-box-shadow:none;
 box-shadow:none;
 color:inherit; }
 .bp3-dark .bp3-button-group.bp3-minimal .bp3-button:hover, .bp3-dark .bp3-button-group.bp3-minimal .bp3-button:active, .bp3-dark .bp3-button-group.bp3-minimal .bp3-button.bp3-active{
 background:none;
 -webkit-box-shadow:none;
 box-shadow:none; }
 .bp3-dark .bp3-button-group.bp3-minimal .bp3-button:hover{
 background:rgba(138, 155, 168, 0.15); }
 .bp3-dark .bp3-button-group.bp3-minimal .bp3-button:active, .bp3-dark .bp3-button-group.bp3-minimal .bp3-button.bp3-active{
 background:rgba(138, 155, 168, 0.3);
 color:#f5f8fa; }
 .bp3-dark .bp3-button-group.bp3-minimal .bp3-button:disabled, .bp3-dark .bp3-button-group.bp3-minimal .bp3-button:disabled:hover, .bp3-dark .bp3-button-group.bp3-minimal .bp3-button.bp3-disabled, .bp3-dark .bp3-button-group.bp3-minimal .bp3-button.bp3-disabled:hover{
 background:none;
 color:rgba(167, 182, 194, 0.6);
 cursor:not-allowed; }
 .bp3-dark .bp3-button-group.bp3-minimal .bp3-button:disabled.bp3-active, .bp3-dark .bp3-button-group.bp3-minimal .bp3-button:disabled:hover.bp3-active, .bp3-dark .bp3-button-group.bp3-minimal .bp3-button.bp3-disabled.bp3-active, .bp3-dark .bp3-button-group.bp3-minimal .bp3-button.bp3-disabled:hover.bp3-active{
 background:rgba(138, 155, 168, 0.3); }
 .bp3-button-group.bp3-minimal .bp3-button.bp3-intent-primary{
 color:#106ba3; }
 .bp3-button-group.bp3-minimal .bp3-button.bp3-intent-primary:hover, .bp3-button-group.bp3-minimal .bp3-button.bp3-intent-primary:active, .bp3-button-group.bp3-minimal .bp3-button.bp3-intent-primary.bp3-active{
 background:none;
 -webkit-box-shadow:none;
 box-shadow:none;
 color:#106ba3; }
 .bp3-button-group.bp3-minimal .bp3-button.bp3-intent-primary:hover{
 background:rgba(19, 124, 189, 0.15);
 color:#106ba3; }
 .bp3-button-group.bp3-minimal .bp3-button.bp3-intent-primary:active, .bp3-button-group.bp3-minimal .bp3-button.bp3-intent-primary.bp3-active{
 background:rgba(19, 124, 189, 0.3);
 color:#106ba3; }
 .bp3-button-group.bp3-minimal .bp3-button.bp3-intent-primary:disabled, .bp3-button-group.bp3-minimal .bp3-button.bp3-intent-primary.bp3-disabled{
 background:none;
 color:rgba(16, 107, 163, 0.5); }
 .bp3-button-group.bp3-minimal .bp3-button.bp3-intent-primary:disabled.bp3-active, .bp3-button-group.bp3-minimal .bp3-button.bp3-intent-primary.bp3-disabled.bp3-active{
 background:rgba(19, 124, 189, 0.3); }
 .bp3-button-group.bp3-minimal .bp3-button.bp3-intent-primary .bp3-button-spinner .bp3-spinner-head{
 stroke:#106ba3; }
 .bp3-dark .bp3-button-group.bp3-minimal .bp3-button.bp3-intent-primary{
 color:#48aff0; }
 .bp3-dark .bp3-button-group.bp3-minimal .bp3-button.bp3-intent-primary:hover{
 background:rgba(19, 124, 189, 0.2);
 color:#48aff0; }
 .bp3-dark .bp3-button-group.bp3-minimal .bp3-button.bp3-intent-primary:active, .bp3-dark .bp3-button-group.bp3-minimal .bp3-button.bp3-intent-primary.bp3-active{
 background:rgba(19, 124, 189, 0.3);
 color:#48aff0; }
 .bp3-dark .bp3-button-group.bp3-minimal .bp3-button.bp3-intent-primary:disabled, .bp3-dark .bp3-button-group.bp3-minimal .bp3-button.bp3-intent-primary.bp3-disabled{
 background:none;
 color:rgba(72, 175, 240, 0.5); }
 .bp3-dark .bp3-button-group.bp3-minimal .bp3-button.bp3-intent-primary:disabled.bp3-active, .bp3-dark .bp3-button-group.bp3-minimal .bp3-button.bp3-intent-primary.bp3-disabled.bp3-active{
 background:rgba(19, 124, 189, 0.3); }
 .bp3-button-group.bp3-minimal .bp3-button.bp3-intent-success{
 color:#0d8050; }
 .bp3-button-group.bp3-minimal .bp3-button.bp3-intent-success:hover, .bp3-button-group.bp3-minimal .bp3-button.bp3-intent-success:active, .bp3-button-group.bp3-minimal .bp3-button.bp3-intent-success.bp3-active{
 background:none;
 -webkit-box-shadow:none;
 box-shadow:none;
 color:#0d8050; }
 .bp3-button-group.bp3-minimal .bp3-button.bp3-intent-success:hover{
 background:rgba(15, 153, 96, 0.15);
 color:#0d8050; }
 .bp3-button-group.bp3-minimal .bp3-button.bp3-intent-success:active, .bp3-button-group.bp3-minimal .bp3-button.bp3-intent-success.bp3-active{
 background:rgba(15, 153, 96, 0.3);
 color:#0d8050; }
 .bp3-button-group.bp3-minimal .bp3-button.bp3-intent-success:disabled, .bp3-button-group.bp3-minimal .bp3-button.bp3-intent-success.bp3-disabled{
 background:none;
 color:rgba(13, 128, 80, 0.5); }
 .bp3-button-group.bp3-minimal .bp3-button.bp3-intent-success:disabled.bp3-active, .bp3-button-group.bp3-minimal .bp3-button.bp3-intent-success.bp3-disabled.bp3-active{
 background:rgba(15, 153, 96, 0.3); }
 .bp3-button-group.bp3-minimal .bp3-button.bp3-intent-success .bp3-button-spinner .bp3-spinner-head{
 stroke:#0d8050; }
 .bp3-dark .bp3-button-group.bp3-minimal .bp3-button.bp3-intent-success{
 color:#3dcc91; }
 .bp3-dark .bp3-button-group.bp3-minimal .bp3-button.bp3-intent-success:hover{
 background:rgba(15, 153, 96, 0.2);
 color:#3dcc91; }
 .bp3-dark .bp3-button-group.bp3-minimal .bp3-button.bp3-intent-success:active, .bp3-dark .bp3-button-group.bp3-minimal .bp3-button.bp3-intent-success.bp3-active{
 background:rgba(15, 153, 96, 0.3);
 color:#3dcc91; }
 .bp3-dark .bp3-button-group.bp3-minimal .bp3-button.bp3-intent-success:disabled, .bp3-dark .bp3-button-group.bp3-minimal .bp3-button.bp3-intent-success.bp3-disabled{
 background:none;
 color:rgba(61, 204, 145, 0.5); }
 .bp3-dark .bp3-button-group.bp3-minimal .bp3-button.bp3-intent-success:disabled.bp3-active, .bp3-dark .bp3-button-group.bp3-minimal .bp3-button.bp3-intent-success.bp3-disabled.bp3-active{
 background:rgba(15, 153, 96, 0.3); }
 .bp3-button-group.bp3-minimal .bp3-button.bp3-intent-warning{
 color:#bf7326; }
 .bp3-button-group.bp3-minimal .bp3-button.bp3-intent-warning:hover, .bp3-button-group.bp3-minimal .bp3-button.bp3-intent-warning:active, .bp3-button-group.bp3-minimal .bp3-button.bp3-intent-warning.bp3-active{
 background:none;
 -webkit-box-shadow:none;
 box-shadow:none;
 color:#bf7326; }
 .bp3-button-group.bp3-minimal .bp3-button.bp3-intent-warning:hover{
 background:rgba(217, 130, 43, 0.15);
 color:#bf7326; }
 .bp3-button-group.bp3-minimal .bp3-button.bp3-intent-warning:active, .bp3-button-group.bp3-minimal .bp3-button.bp3-intent-warning.bp3-active{
 background:rgba(217, 130, 43, 0.3);
 color:#bf7326; }
 .bp3-button-group.bp3-minimal .bp3-button.bp3-intent-warning:disabled, .bp3-button-group.bp3-minimal .bp3-button.bp3-intent-warning.bp3-disabled{
 background:none;
 color:rgba(191, 115, 38, 0.5); }
 .bp3-button-group.bp3-minimal .bp3-button.bp3-intent-warning:disabled.bp3-active, .bp3-button-group.bp3-minimal .bp3-button.bp3-intent-warning.bp3-disabled.bp3-active{
 background:rgba(217, 130, 43, 0.3); }
 .bp3-button-group.bp3-minimal .bp3-button.bp3-intent-warning .bp3-button-spinner .bp3-spinner-head{
 stroke:#bf7326; }
 .bp3-dark .bp3-button-group.bp3-minimal .bp3-button.bp3-intent-warning{
 color:#ffb366; }
 .bp3-dark .bp3-button-group.bp3-minimal .bp3-button.bp3-intent-warning:hover{
 background:rgba(217, 130, 43, 0.2);
 color:#ffb366; }
 .bp3-dark .bp3-button-group.bp3-minimal .bp3-button.bp3-intent-warning:active, .bp3-dark .bp3-button-group.bp3-minimal .bp3-button.bp3-intent-warning.bp3-active{
 background:rgba(217, 130, 43, 0.3);
 color:#ffb366; }
 .bp3-dark .bp3-button-group.bp3-minimal .bp3-button.bp3-intent-warning:disabled, .bp3-dark .bp3-button-group.bp3-minimal .bp3-button.bp3-intent-warning.bp3-disabled{
 background:none;
 color:rgba(255, 179, 102, 0.5); }
 .bp3-dark .bp3-button-group.bp3-minimal .bp3-button.bp3-intent-warning:disabled.bp3-active, .bp3-dark .bp3-button-group.bp3-minimal .bp3-button.bp3-intent-warning.bp3-disabled.bp3-active{
 background:rgba(217, 130, 43, 0.3); }
 .bp3-button-group.bp3-minimal .bp3-button.bp3-intent-danger{
 color:#c23030; }
 .bp3-button-group.bp3-minimal .bp3-button.bp3-intent-danger:hover, .bp3-button-group.bp3-minimal .bp3-button.bp3-intent-danger:active, .bp3-button-group.bp3-minimal .bp3-button.bp3-intent-danger.bp3-active{
 background:none;
 -webkit-box-shadow:none;
 box-shadow:none;
 color:#c23030; }
 .bp3-button-group.bp3-minimal .bp3-button.bp3-intent-danger:hover{
 background:rgba(219, 55, 55, 0.15);
 color:#c23030; }
 .bp3-button-group.bp3-minimal .bp3-button.bp3-intent-danger:active, .bp3-button-group.bp3-minimal .bp3-button.bp3-intent-danger.bp3-active{
 background:rgba(219, 55, 55, 0.3);
 color:#c23030; }
 .bp3-button-group.bp3-minimal .bp3-button.bp3-intent-danger:disabled, .bp3-button-group.bp3-minimal .bp3-button.bp3-intent-danger.bp3-disabled{
 background:none;
 color:rgba(194, 48, 48, 0.5); }
 .bp3-button-group.bp3-minimal .bp3-button.bp3-intent-danger:disabled.bp3-active, .bp3-button-group.bp3-minimal .bp3-button.bp3-intent-danger.bp3-disabled.bp3-active{
 background:rgba(219, 55, 55, 0.3); }
 .bp3-button-group.bp3-minimal .bp3-button.bp3-intent-danger .bp3-button-spinner .bp3-spinner-head{
 stroke:#c23030; }
 .bp3-dark .bp3-button-group.bp3-minimal .bp3-button.bp3-intent-danger{
 color:#ff7373; }
 .bp3-dark .bp3-button-group.bp3-minimal .bp3-button.bp3-intent-danger:hover{
 background:rgba(219, 55, 55, 0.2);
 color:#ff7373; }
 .bp3-dark .bp3-button-group.bp3-minimal .bp3-button.bp3-intent-danger:active, .bp3-dark .bp3-button-group.bp3-minimal .bp3-button.bp3-intent-danger.bp3-active{
 background:rgba(219, 55, 55, 0.3);
 color:#ff7373; }
 .bp3-dark .bp3-button-group.bp3-minimal .bp3-button.bp3-intent-danger:disabled, .bp3-dark .bp3-button-group.bp3-minimal .bp3-button.bp3-intent-danger.bp3-disabled{
 background:none;
 color:rgba(255, 115, 115, 0.5); }
 .bp3-dark .bp3-button-group.bp3-minimal .bp3-button.bp3-intent-danger:disabled.bp3-active, .bp3-dark .bp3-button-group.bp3-minimal .bp3-button.bp3-intent-danger.bp3-disabled.bp3-active{
 background:rgba(219, 55, 55, 0.3); }
 .bp3-button-group .bp3-popover-wrapper,
 .bp3-button-group .bp3-popover-target{
 display:-webkit-box;
 display:-ms-flexbox;
 display:flex;
 -webkit-box-flex:1;
 -ms-flex:1 1 auto;
 flex:1 1 auto; }
 .bp3-button-group.bp3-fill{
 display:-webkit-box;
 display:-ms-flexbox;
 display:flex;
 width:100%; }
 .bp3-button-group .bp3-button.bp3-fill,
 .bp3-button-group.bp3-fill .bp3-button:not(.bp3-fixed){
 -webkit-box-flex:1;
 -ms-flex:1 1 auto;
 flex:1 1 auto; }
 .bp3-button-group.bp3-vertical{
 -webkit-box-align:stretch;
 -ms-flex-align:stretch;
 align-items:stretch;
 -webkit-box-orient:vertical;
 -webkit-box-direction:normal;
 -ms-flex-direction:column;
 flex-direction:column;
 vertical-align:top; }
 .bp3-button-group.bp3-vertical.bp3-fill{
 height:100%;
 width:unset; }
 .bp3-button-group.bp3-vertical .bp3-button{
 margin-right:0 !important;
 width:100%; }
 .bp3-button-group.bp3-vertical:not(.bp3-minimal) > .bp3-popover-wrapper:first-child .bp3-button,
 .bp3-button-group.bp3-vertical:not(.bp3-minimal) > .bp3-button:first-child{
 border-radius:3px 3px 0 0; }
 .bp3-button-group.bp3-vertical:not(.bp3-minimal) > .bp3-popover-wrapper:last-child .bp3-button,
 .bp3-button-group.bp3-vertical:not(.bp3-minimal) > .bp3-button:last-child{
 border-radius:0 0 3px 3px; }
 .bp3-button-group.bp3-vertical:not(.bp3-minimal) > .bp3-popover-wrapper:not(:last-child) .bp3-button,
 .bp3-button-group.bp3-vertical:not(.bp3-minimal) > .bp3-button:not(:last-child){
 margin-bottom:-1px; }
 .bp3-button-group.bp3-align-left .bp3-button{
 text-align:left; }
 .bp3-dark .bp3-button-group:not(.bp3-minimal) > .bp3-popover-wrapper:not(:last-child) .bp3-button,
 .bp3-dark .bp3-button-group:not(.bp3-minimal) > .bp3-button:not(:last-child){
 margin-right:1px; }
 .bp3-dark .bp3-button-group.bp3-vertical > .bp3-popover-wrapper:not(:last-child) .bp3-button,
 .bp3-dark .bp3-button-group.bp3-vertical > .bp3-button:not(:last-child){
 margin-bottom:1px; }
.bp3-callout{
 font-size:14px;
 line-height:1.5;
 background-color:rgba(138, 155, 168, 0.15);
 border-radius:3px;
 padding:10px 12px 9px;
 position:relative;
 width:100%; }
 .bp3-callout[class\*="bp3-icon-"]{
 padding-left:40px; }
 .bp3-callout[class\*="bp3-icon-"]::before{
 font-family:"Icons20", sans-serif;
 font-size:20px;
 font-style:normal;
 font-weight:400;
 line-height:1;
 -moz-osx-font-smoothing:grayscale;
 -webkit-font-smoothing:antialiased;
 color:#5c7080;
 left:10px;
 position:absolute;
 top:10px; }
 .bp3-callout.bp3-callout-icon{
 padding-left:40px; }
 .bp3-callout.bp3-callout-icon > .bp3-icon:first-child{
 color:#5c7080;
 left:10px;
 position:absolute;
 top:10px; }
 .bp3-callout .bp3-heading{
 line-height:20px;
 margin-bottom:5px;
 margin-top:0; }
 .bp3-callout .bp3-heading:last-child{
 margin-bottom:0; }
 .bp3-dark .bp3-callout{
 background-color:rgba(138, 155, 168, 0.2); }
 .bp3-dark .bp3-callout[class\*="bp3-icon-"]::before{
 color:#a7b6c2; }
 .bp3-callout.bp3-intent-primary{
 background-color:rgba(19, 124, 189, 0.15); }
 .bp3-callout.bp3-intent-primary[class\*="bp3-icon-"]::before,
 .bp3-callout.bp3-intent-primary > .bp3-icon:first-child,
 .bp3-callout.bp3-intent-primary .bp3-heading{
 color:#106ba3; }
 .bp3-dark .bp3-callout.bp3-intent-primary{
 background-color:rgba(19, 124, 189, 0.25); }
 .bp3-dark .bp3-callout.bp3-intent-primary[class\*="bp3-icon-"]::before,
 .bp3-dark .bp3-callout.bp3-intent-primary > .bp3-icon:first-child,
 .bp3-dark .bp3-callout.bp3-intent-primary .bp3-heading{
 color:#48aff0; }
 .bp3-callout.bp3-intent-success{
 background-color:rgba(15, 153, 96, 0.15); }
 .bp3-callout.bp3-intent-success[class\*="bp3-icon-"]::before,
 .bp3-callout.bp3-intent-success > .bp3-icon:first-child,
 .bp3-callout.bp3-intent-success .bp3-heading{
 color:#0d8050; }
 .bp3-dark .bp3-callout.bp3-intent-success{
 background-color:rgba(15, 153, 96, 0.25); }
 .bp3-dark .bp3-callout.bp3-intent-success[class\*="bp3-icon-"]::before,
 .bp3-dark .bp3-callout.bp3-intent-success > .bp3-icon:first-child,
 .bp3-dark .bp3-callout.bp3-intent-success .bp3-heading{
 color:#3dcc91; }
 .bp3-callout.bp3-intent-warning{
 background-color:rgba(217, 130, 43, 0.15); }
 .bp3-callout.bp3-intent-warning[class\*="bp3-icon-"]::before,
 .bp3-callout.bp3-intent-warning > .bp3-icon:first-child,
 .bp3-callout.bp3-intent-warning .bp3-heading{
 color:#bf7326; }
 .bp3-dark .bp3-callout.bp3-intent-warning{
 background-color:rgba(217, 130, 43, 0.25); }
 .bp3-dark .bp3-callout.bp3-intent-warning[class\*="bp3-icon-"]::before,
 .bp3-dark .bp3-callout.bp3-intent-warning > .bp3-icon:first-child,
 .bp3-dark .bp3-callout.bp3-intent-warning .bp3-heading{
 color:#ffb366; }
 .bp3-callout.bp3-intent-danger{
 background-color:rgba(219, 55, 55, 0.15); }
 .bp3-callout.bp3-intent-danger[class\*="bp3-icon-"]::before,
 .bp3-callout.bp3-intent-danger > .bp3-icon:first-child,
 .bp3-callout.bp3-intent-danger .bp3-heading{
 color:#c23030; }
 .bp3-dark .bp3-callout.bp3-intent-danger{
 background-color:rgba(219, 55, 55, 0.25); }
 .bp3-dark .bp3-callout.bp3-intent-danger[class\*="bp3-icon-"]::before,
 .bp3-dark .bp3-callout.bp3-intent-danger > .bp3-icon:first-child,
 .bp3-dark .bp3-callout.bp3-intent-danger .bp3-heading{
 color:#ff7373; }
 .bp3-running-text .bp3-callout{
 margin:20px 0; }
.bp3-card{
 background-color:#ffffff;
 border-radius:3px;
 -webkit-box-shadow:0 0 0 1px rgba(16, 22, 26, 0.15), 0 0 0 rgba(16, 22, 26, 0), 0 0 0 rgba(16, 22, 26, 0);
 box-shadow:0 0 0 1px rgba(16, 22, 26, 0.15), 0 0 0 rgba(16, 22, 26, 0), 0 0 0 rgba(16, 22, 26, 0);
 padding:20px;
 -webkit-transition:-webkit-transform 200ms cubic-bezier(0.4, 1, 0.75, 0.9), -webkit-box-shadow 200ms cubic-bezier(0.4, 1, 0.75, 0.9);
 transition:-webkit-transform 200ms cubic-bezier(0.4, 1, 0.75, 0.9), -webkit-box-shadow 200ms cubic-bezier(0.4, 1, 0.75, 0.9);
 transition:transform 200ms cubic-bezier(0.4, 1, 0.75, 0.9), box-shadow 200ms cubic-bezier(0.4, 1, 0.75, 0.9);
 transition:transform 200ms cubic-bezier(0.4, 1, 0.75, 0.9), box-shadow 200ms cubic-bezier(0.4, 1, 0.75, 0.9), -webkit-transform 200ms cubic-bezier(0.4, 1, 0.75, 0.9), -webkit-box-shadow 200ms cubic-bezier(0.4, 1, 0.75, 0.9); }
 .bp3-card.bp3-dark,
 .bp3-dark .bp3-card{
 background-color:#30404d;
 -webkit-box-shadow:0 0 0 1px rgba(16, 22, 26, 0.4), 0 0 0 rgba(16, 22, 26, 0), 0 0 0 rgba(16, 22, 26, 0);
 box-shadow:0 0 0 1px rgba(16, 22, 26, 0.4), 0 0 0 rgba(16, 22, 26, 0), 0 0 0 rgba(16, 22, 26, 0); }

.bp3-elevation-0{
 -webkit-box-shadow:0 0 0 1px rgba(16, 22, 26, 0.15), 0 0 0 rgba(16, 22, 26, 0), 0 0 0 rgba(16, 22, 26, 0);
 box-shadow:0 0 0 1px rgba(16, 22, 26, 0.15), 0 0 0 rgba(16, 22, 26, 0), 0 0 0 rgba(16, 22, 26, 0); }
 .bp3-elevation-0.bp3-dark,
 .bp3-dark .bp3-elevation-0{
 -webkit-box-shadow:0 0 0 1px rgba(16, 22, 26, 0.4), 0 0 0 rgba(16, 22, 26, 0), 0 0 0 rgba(16, 22, 26, 0);
 box-shadow:0 0 0 1px rgba(16, 22, 26, 0.4), 0 0 0 rgba(16, 22, 26, 0), 0 0 0 rgba(16, 22, 26, 0); }

.bp3-elevation-1{
 -webkit-box-shadow:0 0 0 1px rgba(16, 22, 26, 0.1), 0 0 0 rgba(16, 22, 26, 0), 0 1px 1px rgba(16, 22, 26, 0.2);
 box-shadow:0 0 0 1px rgba(16, 22, 26, 0.1), 0 0 0 rgba(16, 22, 26, 0), 0 1px 1px rgba(16, 22, 26, 0.2); }
 .bp3-elevation-1.bp3-dark,
 .bp3-dark .bp3-elevation-1{
 -webkit-box-shadow:0 0 0 1px rgba(16, 22, 26, 0.2), 0 0 0 rgba(16, 22, 26, 0), 0 1px 1px rgba(16, 22, 26, 0.4);
 box-shadow:0 0 0 1px rgba(16, 22, 26, 0.2), 0 0 0 rgba(16, 22, 26, 0), 0 1px 1px rgba(16, 22, 26, 0.4); }

.bp3-elevation-2{
 -webkit-box-shadow:0 0 0 1px rgba(16, 22, 26, 0.1), 0 1px 1px rgba(16, 22, 26, 0.2), 0 2px 6px rgba(16, 22, 26, 0.2);
 box-shadow:0 0 0 1px rgba(16, 22, 26, 0.1), 0 1px 1px rgba(16, 22, 26, 0.2), 0 2px 6px rgba(16, 22, 26, 0.2); }
 .bp3-elevation-2.bp3-dark,
 .bp3-dark .bp3-elevation-2{
 -webkit-box-shadow:0 0 0 1px rgba(16, 22, 26, 0.2), 0 1px 1px rgba(16, 22, 26, 0.4), 0 2px 6px rgba(16, 22, 26, 0.4);
 box-shadow:0 0 0 1px rgba(16, 22, 26, 0.2), 0 1px 1px rgba(16, 22, 26, 0.4), 0 2px 6px rgba(16, 22, 26, 0.4); }

.bp3-elevation-3{
 -webkit-box-shadow:0 0 0 1px rgba(16, 22, 26, 0.1), 0 2px 4px rgba(16, 22, 26, 0.2), 0 8px 24px rgba(16, 22, 26, 0.2);
 box-shadow:0 0 0 1px rgba(16, 22, 26, 0.1), 0 2px 4px rgba(16, 22, 26, 0.2), 0 8px 24px rgba(16, 22, 26, 0.2); }
 .bp3-elevation-3.bp3-dark,
 .bp3-dark .bp3-elevation-3{
 -webkit-box-shadow:0 0 0 1px rgba(16, 22, 26, 0.2), 0 2px 4px rgba(16, 22, 26, 0.4), 0 8px 24px rgba(16, 22, 26, 0.4);
 box-shadow:0 0 0 1px rgba(16, 22, 26, 0.2), 0 2px 4px rgba(16, 22, 26, 0.4), 0 8px 24px rgba(16, 22, 26, 0.4); }

.bp3-elevation-4{
 -webkit-box-shadow:0 0 0 1px rgba(16, 22, 26, 0.1), 0 4px 8px rgba(16, 22, 26, 0.2), 0 18px 46px 6px rgba(16, 22, 26, 0.2);
 box-shadow:0 0 0 1px rgba(16, 22, 26, 0.1), 0 4px 8px rgba(16, 22, 26, 0.2), 0 18px 46px 6px rgba(16, 22, 26, 0.2); }
 .bp3-elevation-4.bp3-dark,
 .bp3-dark .bp3-elevation-4{
 -webkit-box-shadow:0 0 0 1px rgba(16, 22, 26, 0.2), 0 4px 8px rgba(16, 22, 26, 0.4), 0 18px 46px 6px rgba(16, 22, 26, 0.4);
 box-shadow:0 0 0 1px rgba(16, 22, 26, 0.2), 0 4px 8px rgba(16, 22, 26, 0.4), 0 18px 46px 6px rgba(16, 22, 26, 0.4); }

.bp3-card.bp3-interactive:hover{
 -webkit-box-shadow:0 0 0 1px rgba(16, 22, 26, 0.1), 0 2px 4px rgba(16, 22, 26, 0.2), 0 8px 24px rgba(16, 22, 26, 0.2);
 box-shadow:0 0 0 1px rgba(16, 22, 26, 0.1), 0 2px 4px rgba(16, 22, 26, 0.2), 0 8px 24px rgba(16, 22, 26, 0.2);
 cursor:pointer; }
 .bp3-card.bp3-interactive:hover.bp3-dark,
 .bp3-dark .bp3-card.bp3-interactive:hover{
 -webkit-box-shadow:0 0 0 1px rgba(16, 22, 26, 0.2), 0 2px 4px rgba(16, 22, 26, 0.4), 0 8px 24px rgba(16, 22, 26, 0.4);
 box-shadow:0 0 0 1px rgba(16, 22, 26, 0.2), 0 2px 4px rgba(16, 22, 26, 0.4), 0 8px 24px rgba(16, 22, 26, 0.4); }

.bp3-card.bp3-interactive:active{
 -webkit-box-shadow:0 0 0 1px rgba(16, 22, 26, 0.1), 0 0 0 rgba(16, 22, 26, 0), 0 1px 1px rgba(16, 22, 26, 0.2);
 box-shadow:0 0 0 1px rgba(16, 22, 26, 0.1), 0 0 0 rgba(16, 22, 26, 0), 0 1px 1px rgba(16, 22, 26, 0.2);
 opacity:0.9;
 -webkit-transition-duration:0;
 transition-duration:0; }
 .bp3-card.bp3-interactive:active.bp3-dark,
 .bp3-dark .bp3-card.bp3-interactive:active{
 -webkit-box-shadow:0 0 0 1px rgba(16, 22, 26, 0.2), 0 0 0 rgba(16, 22, 26, 0), 0 1px 1px rgba(16, 22, 26, 0.4);
 box-shadow:0 0 0 1px rgba(16, 22, 26, 0.2), 0 0 0 rgba(16, 22, 26, 0), 0 1px 1px rgba(16, 22, 26, 0.4); }

.bp3-collapse{
 height:0;
 overflow-y:hidden;
 -webkit-transition:height 200ms cubic-bezier(0.4, 1, 0.75, 0.9);
 transition:height 200ms cubic-bezier(0.4, 1, 0.75, 0.9); }
 .bp3-collapse .bp3-collapse-body{
 -webkit-transition:-webkit-transform 200ms cubic-bezier(0.4, 1, 0.75, 0.9);
 transition:-webkit-transform 200ms cubic-bezier(0.4, 1, 0.75, 0.9);
 transition:transform 200ms cubic-bezier(0.4, 1, 0.75, 0.9);
 transition:transform 200ms cubic-bezier(0.4, 1, 0.75, 0.9), -webkit-transform 200ms cubic-bezier(0.4, 1, 0.75, 0.9); }
 .bp3-collapse .bp3-collapse-body[aria-hidden="true"]{
 display:none; }

.bp3-context-menu .bp3-popover-target{
 display:block; }

.bp3-context-menu-popover-target{
 position:fixed; }

.bp3-divider{
 border-bottom:1px solid rgba(16, 22, 26, 0.15);
 border-right:1px solid rgba(16, 22, 26, 0.15);
 margin:5px; }
 .bp3-dark .bp3-divider{
 border-color:rgba(16, 22, 26, 0.4); }
.bp3-dialog-container{
 opacity:1;
 -webkit-transform:scale(1);
 transform:scale(1);
 -webkit-box-align:center;
 -ms-flex-align:center;
 align-items:center;
 display:-webkit-box;
 display:-ms-flexbox;
 display:flex;
 -webkit-box-pack:center;
 -ms-flex-pack:center;
 justify-content:center;
 min-height:100%;
 pointer-events:none;
 -webkit-user-select:none;
 -moz-user-select:none;
 -ms-user-select:none;
 user-select:none;
 width:100%; }
 .bp3-dialog-container.bp3-overlay-enter > .bp3-dialog, .bp3-dialog-container.bp3-overlay-appear > .bp3-dialog{
 opacity:0;
 -webkit-transform:scale(0.5);
 transform:scale(0.5); }
 .bp3-dialog-container.bp3-overlay-enter-active > .bp3-dialog, .bp3-dialog-container.bp3-overlay-appear-active > .bp3-dialog{
 opacity:1;
 -webkit-transform:scale(1);
 transform:scale(1);
 -webkit-transition-delay:0;
 transition-delay:0;
 -webkit-transition-duration:300ms;
 transition-duration:300ms;
 -webkit-transition-property:opacity, -webkit-transform;
 transition-property:opacity, -webkit-transform;
 transition-property:opacity, transform;
 transition-property:opacity, transform, -webkit-transform;
 -webkit-transition-timing-function:cubic-bezier(0.54, 1.12, 0.38, 1.11);
 transition-timing-function:cubic-bezier(0.54, 1.12, 0.38, 1.11); }
 .bp3-dialog-container.bp3-overlay-exit > .bp3-dialog{
 opacity:1;
 -webkit-transform:scale(1);
 transform:scale(1); }
 .bp3-dialog-container.bp3-overlay-exit-active > .bp3-dialog{
 opacity:0;
 -webkit-transform:scale(0.5);
 transform:scale(0.5);
 -webkit-transition-delay:0;
 transition-delay:0;
 -webkit-transition-duration:300ms;
 transition-duration:300ms;
 -webkit-transition-property:opacity, -webkit-transform;
 transition-property:opacity, -webkit-transform;
 transition-property:opacity, transform;
 transition-property:opacity, transform, -webkit-transform;
 -webkit-transition-timing-function:cubic-bezier(0.54, 1.12, 0.38, 1.11);
 transition-timing-function:cubic-bezier(0.54, 1.12, 0.38, 1.11); }

.bp3-dialog{
 background:#ebf1f5;
 border-radius:6px;
 -webkit-box-shadow:0 0 0 1px rgba(16, 22, 26, 0.1), 0 4px 8px rgba(16, 22, 26, 0.2), 0 18px 46px 6px rgba(16, 22, 26, 0.2);
 box-shadow:0 0 0 1px rgba(16, 22, 26, 0.1), 0 4px 8px rgba(16, 22, 26, 0.2), 0 18px 46px 6px rgba(16, 22, 26, 0.2);
 display:-webkit-box;
 display:-ms-flexbox;
 display:flex;
 -webkit-box-orient:vertical;
 -webkit-box-direction:normal;
 -ms-flex-direction:column;
 flex-direction:column;
 margin:30px 0;
 padding-bottom:20px;
 pointer-events:all;
 -webkit-user-select:text;
 -moz-user-select:text;
 -ms-user-select:text;
 user-select:text;
 width:500px; }
 .bp3-dialog:focus{
 outline:0; }
 .bp3-dialog.bp3-dark,
 .bp3-dark .bp3-dialog{
 background:#293742;
 -webkit-box-shadow:0 0 0 1px rgba(16, 22, 26, 0.2), 0 4px 8px rgba(16, 22, 26, 0.4), 0 18px 46px 6px rgba(16, 22, 26, 0.4);
 box-shadow:0 0 0 1px rgba(16, 22, 26, 0.2), 0 4px 8px rgba(16, 22, 26, 0.4), 0 18px 46px 6px rgba(16, 22, 26, 0.4);
 color:#f5f8fa; }

.bp3-dialog-header{
 -webkit-box-align:center;
 -ms-flex-align:center;
 align-items:center;
 background:#ffffff;
 border-radius:6px 6px 0 0;
 -webkit-box-shadow:0 1px 0 rgba(16, 22, 26, 0.15);
 box-shadow:0 1px 0 rgba(16, 22, 26, 0.15);
 display:-webkit-box;
 display:-ms-flexbox;
 display:flex;
 -webkit-box-flex:0;
 -ms-flex:0 0 auto;
 flex:0 0 auto;
 min-height:40px;
 padding-left:20px;
 padding-right:5px;
 z-index:30; }
 .bp3-dialog-header .bp3-icon-large,
 .bp3-dialog-header .bp3-icon{
 color:#5c7080;
 -webkit-box-flex:0;
 -ms-flex:0 0 auto;
 flex:0 0 auto;
 margin-right:10px; }
 .bp3-dialog-header .bp3-heading{
 overflow:hidden;
 text-overflow:ellipsis;
 white-space:nowrap;
 word-wrap:normal;
 -webkit-box-flex:1;
 -ms-flex:1 1 auto;
 flex:1 1 auto;
 line-height:inherit;
 margin:0; }
 .bp3-dialog-header .bp3-heading:last-child{
 margin-right:20px; }
 .bp3-dark .bp3-dialog-header{
 background:#30404d;
 -webkit-box-shadow:0 1px 0 rgba(16, 22, 26, 0.4);
 box-shadow:0 1px 0 rgba(16, 22, 26, 0.4); }
 .bp3-dark .bp3-dialog-header .bp3-icon-large,
 .bp3-dark .bp3-dialog-header .bp3-icon{
 color:#a7b6c2; }

.bp3-dialog-body{
 -webkit-box-flex:1;
 -ms-flex:1 1 auto;
 flex:1 1 auto;
 line-height:18px;
 margin:20px; }

.bp3-dialog-footer{
 -webkit-box-flex:0;
 -ms-flex:0 0 auto;
 flex:0 0 auto;
 margin:0 20px; }

.bp3-dialog-footer-actions{
 display:-webkit-box;
 display:-ms-flexbox;
 display:flex;
 -webkit-box-pack:end;
 -ms-flex-pack:end;
 justify-content:flex-end; }
 .bp3-dialog-footer-actions .bp3-button{
 margin-left:10px; }
.bp3-multistep-dialog-panels{
 display:-webkit-box;
 display:-ms-flexbox;
 display:flex; }

.bp3-multistep-dialog-left-panel{
 display:-webkit-box;
 display:-ms-flexbox;
 display:flex;
 -webkit-box-flex:1;
 -ms-flex:1;
 flex:1;
 -webkit-box-orient:vertical;
 -webkit-box-direction:normal;
 -ms-flex-direction:column;
 flex-direction:column; }
 .bp3-dark .bp3-multistep-dialog-left-panel{
 background:#202b33; }

.bp3-multistep-dialog-right-panel{
 background-color:#f5f8fa;
 border-left:1px solid rgba(16, 22, 26, 0.15);
 border-radius:0 0 6px 0;
 -webkit-box-flex:3;
 -ms-flex:3;
 flex:3;
 min-width:0; }
 .bp3-dark .bp3-multistep-dialog-right-panel{
 background-color:#293742;
 border-left:1px solid rgba(16, 22, 26, 0.4); }

.bp3-multistep-dialog-footer{
 background-color:#ffffff;
 border-radius:0 0 6px 0;
 border-top:1px solid rgba(16, 22, 26, 0.15);
 padding:10px; }
 .bp3-dark .bp3-multistep-dialog-footer{
 background:#30404d;
 border-top:1px solid rgba(16, 22, 26, 0.4); }

.bp3-dialog-step-container{
 background-color:#f5f8fa;
 border-bottom:1px solid rgba(16, 22, 26, 0.15); }
 .bp3-dark .bp3-dialog-step-container{
 background:#293742;
 border-bottom:1px solid rgba(16, 22, 26, 0.4); }
 .bp3-dialog-step-container.bp3-dialog-step-viewed{
 background-color:#ffffff; }
 .bp3-dark .bp3-dialog-step-container.bp3-dialog-step-viewed{
 background:#30404d; }

.bp3-dialog-step{
 -webkit-box-align:center;
 -ms-flex-align:center;
 align-items:center;
 background-color:#f5f8fa;
 border-radius:6px;
 cursor:not-allowed;
 display:-webkit-box;
 display:-ms-flexbox;
 display:flex;
 margin:4px;
 padding:6px 14px; }
 .bp3-dark .bp3-dialog-step{
 background:#293742; }
 .bp3-dialog-step-viewed .bp3-dialog-step{
 background-color:#ffffff;
 cursor:pointer; }
 .bp3-dark .bp3-dialog-step-viewed .bp3-dialog-step{
 background:#30404d; }
 .bp3-dialog-step:hover{
 background-color:#f5f8fa; }
 .bp3-dark .bp3-dialog-step:hover{
 background:#293742; }

.bp3-dialog-step-icon{
 -webkit-box-align:center;
 -ms-flex-align:center;
 align-items:center;
 background-color:rgba(92, 112, 128, 0.6);
 border-radius:50%;
 color:#ffffff;
 display:-webkit-box;
 display:-ms-flexbox;
 display:flex;
 height:25px;
 -webkit-box-pack:center;
 -ms-flex-pack:center;
 justify-content:center;
 width:25px; }
 .bp3-dark .bp3-dialog-step-icon{
 background-color:rgba(167, 182, 194, 0.6); }
 .bp3-active.bp3-dialog-step-viewed .bp3-dialog-step-icon{
 background-color:#2b95d6; }
 .bp3-dialog-step-viewed .bp3-dialog-step-icon{
 background-color:#8a9ba8; }

.bp3-dialog-step-title{
 color:rgba(92, 112, 128, 0.6);
 -webkit-box-flex:1;
 -ms-flex:1;
 flex:1;
 padding-left:10px; }
 .bp3-dark .bp3-dialog-step-title{
 color:rgba(167, 182, 194, 0.6); }
 .bp3-active.bp3-dialog-step-viewed .bp3-dialog-step-title{
 color:#2b95d6; }
 .bp3-dialog-step-viewed:not(.bp3-active) .bp3-dialog-step-title{
 color:#182026; }
 .bp3-dark .bp3-dialog-step-viewed:not(.bp3-active) .bp3-dialog-step-title{
 color:#f5f8fa; }
.bp3-drawer{
 background:#ffffff;
 -webkit-box-shadow:0 0 0 1px rgba(16, 22, 26, 0.1), 0 4px 8px rgba(16, 22, 26, 0.2), 0 18px 46px 6px rgba(16, 22, 26, 0.2);
 box-shadow:0 0 0 1px rgba(16, 22, 26, 0.1), 0 4px 8px rgba(16, 22, 26, 0.2), 0 18px 46px 6px rgba(16, 22, 26, 0.2);
 display:-webkit-box;
 display:-ms-flexbox;
 display:flex;
 -webkit-box-orient:vertical;
 -webkit-box-direction:normal;
 -ms-flex-direction:column;
 flex-direction:column;
 margin:0;
 padding:0; }
 .bp3-drawer:focus{
 outline:0; }
 .bp3-drawer.bp3-position-top{
 height:50%;
 left:0;
 right:0;
 top:0; }
 .bp3-drawer.bp3-position-top.bp3-overlay-enter, .bp3-drawer.bp3-position-top.bp3-overlay-appear{
 -webkit-transform:translateY(-100%);
 transform:translateY(-100%); }
 .bp3-drawer.bp3-position-top.bp3-overlay-enter-active, .bp3-drawer.bp3-position-top.bp3-overlay-appear-active{
 -webkit-transform:translateY(0);
 transform:translateY(0);
 -webkit-transition-delay:0;
 transition-delay:0;
 -webkit-transition-duration:200ms;
 transition-duration:200ms;
 -webkit-transition-property:-webkit-transform;
 transition-property:-webkit-transform;
 transition-property:transform;
 transition-property:transform, -webkit-transform;
 -webkit-transition-timing-function:cubic-bezier(0.4, 1, 0.75, 0.9);
 transition-timing-function:cubic-bezier(0.4, 1, 0.75, 0.9); }
 .bp3-drawer.bp3-position-top.bp3-overlay-exit{
 -webkit-transform:translateY(0);
 transform:translateY(0); }
 .bp3-drawer.bp3-position-top.bp3-overlay-exit-active{
 -webkit-transform:translateY(-100%);
 transform:translateY(-100%);
 -webkit-transition-delay:0;
 transition-delay:0;
 -webkit-transition-duration:100ms;
 transition-duration:100ms;
 -webkit-transition-property:-webkit-transform;
 transition-property:-webkit-transform;
 transition-property:transform;
 transition-property:transform, -webkit-transform;
 -webkit-transition-timing-function:cubic-bezier(0.4, 1, 0.75, 0.9);
 transition-timing-function:cubic-bezier(0.4, 1, 0.75, 0.9); }
 .bp3-drawer.bp3-position-bottom{
 bottom:0;
 height:50%;
 left:0;
 right:0; }
 .bp3-drawer.bp3-position-bottom.bp3-overlay-enter, .bp3-drawer.bp3-position-bottom.bp3-overlay-appear{
 -webkit-transform:translateY(100%);
 transform:translateY(100%); }
 .bp3-drawer.bp3-position-bottom.bp3-overlay-enter-active, .bp3-drawer.bp3-position-bottom.bp3-overlay-appear-active{
 -webkit-transform:translateY(0);
 transform:translateY(0);
 -webkit-transition-delay:0;
 transition-delay:0;
 -webkit-transition-duration:200ms;
 transition-duration:200ms;
 -webkit-transition-property:-webkit-transform;
 transition-property:-webkit-transform;
 transition-property:transform;
 transition-property:transform, -webkit-transform;
 -webkit-transition-timing-function:cubic-bezier(0.4, 1, 0.75, 0.9);
 transition-timing-function:cubic-bezier(0.4, 1, 0.75, 0.9); }
 .bp3-drawer.bp3-position-bottom.bp3-overlay-exit{
 -webkit-transform:translateY(0);
 transform:translateY(0); }
 .bp3-drawer.bp3-position-bottom.bp3-overlay-exit-active{
 -webkit-transform:translateY(100%);
 transform:translateY(100%);
 -webkit-transition-delay:0;
 transition-delay:0;
 -webkit-transition-duration:100ms;
 transition-duration:100ms;
 -webkit-transition-property:-webkit-transform;
 transition-property:-webkit-transform;
 transition-property:transform;
 transition-property:transform, -webkit-transform;
 -webkit-transition-timing-function:cubic-bezier(0.4, 1, 0.75, 0.9);
 transition-timing-function:cubic-bezier(0.4, 1, 0.75, 0.9); }
 .bp3-drawer.bp3-position-left{
 bottom:0;
 left:0;
 top:0;
 width:50%; }
 .bp3-drawer.bp3-position-left.bp3-overlay-enter, .bp3-drawer.bp3-position-left.bp3-overlay-appear{
 -webkit-transform:translateX(-100%);
 transform:translateX(-100%); }
 .bp3-drawer.bp3-position-left.bp3-overlay-enter-active, .bp3-drawer.bp3-position-left.bp3-overlay-appear-active{
 -webkit-transform:translateX(0);
 transform:translateX(0);
 -webkit-transition-delay:0;
 transition-delay:0;
 -webkit-transition-duration:200ms;
 transition-duration:200ms;
 -webkit-transition-property:-webkit-transform;
 transition-property:-webkit-transform;
 transition-property:transform;
 transition-property:transform, -webkit-transform;
 -webkit-transition-timing-function:cubic-bezier(0.4, 1, 0.75, 0.9);
 transition-timing-function:cubic-bezier(0.4, 1, 0.75, 0.9); }
 .bp3-drawer.bp3-position-left.bp3-overlay-exit{
 -webkit-transform:translateX(0);
 transform:translateX(0); }
 .bp3-drawer.bp3-position-left.bp3-overlay-exit-active{
 -webkit-transform:translateX(-100%);
 transform:translateX(-100%);
 -webkit-transition-delay:0;
 transition-delay:0;
 -webkit-transition-duration:100ms;
 transition-duration:100ms;
 -webkit-transition-property:-webkit-transform;
 transition-property:-webkit-transform;
 transition-property:transform;
 transition-property:transform, -webkit-transform;
 -webkit-transition-timing-function:cubic-bezier(0.4, 1, 0.75, 0.9);
 transition-timing-function:cubic-bezier(0.4, 1, 0.75, 0.9); }
 .bp3-drawer.bp3-position-right{
 bottom:0;
 right:0;
 top:0;
 width:50%; }
 .bp3-drawer.bp3-position-right.bp3-overlay-enter, .bp3-drawer.bp3-position-right.bp3-overlay-appear{
 -webkit-transform:translateX(100%);
 transform:translateX(100%); }
 .bp3-drawer.bp3-position-right.bp3-overlay-enter-active, .bp3-drawer.bp3-position-right.bp3-overlay-appear-active{
 -webkit-transform:translateX(0);
 transform:translateX(0);
 -webkit-transition-delay:0;
 transition-delay:0;
 -webkit-transition-duration:200ms;
 transition-duration:200ms;
 -webkit-transition-property:-webkit-transform;
 transition-property:-webkit-transform;
 transition-property:transform;
 transition-property:transform, -webkit-transform;
 -webkit-transition-timing-function:cubic-bezier(0.4, 1, 0.75, 0.9);
 transition-timing-function:cubic-bezier(0.4, 1, 0.75, 0.9); }
 .bp3-drawer.bp3-position-right.bp3-overlay-exit{
 -webkit-transform:translateX(0);
 transform:translateX(0); }
 .bp3-drawer.bp3-position-right.bp3-overlay-exit-active{
 -webkit-transform:translateX(100%);
 transform:translateX(100%);
 -webkit-transition-delay:0;
 transition-delay:0;
 -webkit-transition-duration:100ms;
 transition-duration:100ms;
 -webkit-transition-property:-webkit-transform;
 transition-property:-webkit-transform;
 transition-property:transform;
 transition-property:transform, -webkit-transform;
 -webkit-transition-timing-function:cubic-bezier(0.4, 1, 0.75, 0.9);
 transition-timing-function:cubic-bezier(0.4, 1, 0.75, 0.9); }
 .bp3-drawer:not(.bp3-position-top):not(.bp3-position-bottom):not(.bp3-position-left):not(
 .bp3-position-right):not(.bp3-vertical){
 bottom:0;
 right:0;
 top:0;
 width:50%; }
 .bp3-drawer:not(.bp3-position-top):not(.bp3-position-bottom):not(.bp3-position-left):not(
 .bp3-position-right):not(.bp3-vertical).bp3-overlay-enter, .bp3-drawer:not(.bp3-position-top):not(.bp3-position-bottom):not(.bp3-position-left):not(
 .bp3-position-right):not(.bp3-vertical).bp3-overlay-appear{
 -webkit-transform:translateX(100%);
 transform:translateX(100%); }
 .bp3-drawer:not(.bp3-position-top):not(.bp3-position-bottom):not(.bp3-position-left):not(
 .bp3-position-right):not(.bp3-vertical).bp3-overlay-enter-active, .bp3-drawer:not(.bp3-position-top):not(.bp3-position-bottom):not(.bp3-position-left):not(
 .bp3-position-right):not(.bp3-vertical).bp3-overlay-appear-active{
 -webkit-transform:translateX(0);
 transform:translateX(0);
 -webkit-transition-delay:0;
 transition-delay:0;
 -webkit-transition-duration:200ms;
 transition-duration:200ms;
 -webkit-transition-property:-webkit-transform;
 transition-property:-webkit-transform;
 transition-property:transform;
 transition-property:transform, -webkit-transform;
 -webkit-transition-timing-function:cubic-bezier(0.4, 1, 0.75, 0.9);
 transition-timing-function:cubic-bezier(0.4, 1, 0.75, 0.9); }
 .bp3-drawer:not(.bp3-position-top):not(.bp3-position-bottom):not(.bp3-position-left):not(
 .bp3-position-right):not(.bp3-vertical).bp3-overlay-exit{
 -webkit-transform:translateX(0);
 transform:translateX(0); }
 .bp3-drawer:not(.bp3-position-top):not(.bp3-position-bottom):not(.bp3-position-left):not(
 .bp3-position-right):not(.bp3-vertical).bp3-overlay-exit-active{
 -webkit-transform:translateX(100%);
 transform:translateX(100%);
 -webkit-transition-delay:0;
 transition-delay:0;
 -webkit-transition-duration:100ms;
 transition-duration:100ms;
 -webkit-transition-property:-webkit-transform;
 transition-property:-webkit-transform;
 transition-property:transform;
 transition-property:transform, -webkit-transform;
 -webkit-transition-timing-function:cubic-bezier(0.4, 1, 0.75, 0.9);
 transition-timing-function:cubic-bezier(0.4, 1, 0.75, 0.9); }
 .bp3-drawer:not(.bp3-position-top):not(.bp3-position-bottom):not(.bp3-position-left):not(
 .bp3-position-right).bp3-vertical{
 bottom:0;
 height:50%;
 left:0;
 right:0; }
 .bp3-drawer:not(.bp3-position-top):not(.bp3-position-bottom):not(.bp3-position-left):not(
 .bp3-position-right).bp3-vertical.bp3-overlay-enter, .bp3-drawer:not(.bp3-position-top):not(.bp3-position-bottom):not(.bp3-position-left):not(
 .bp3-position-right).bp3-vertical.bp3-overlay-appear{
 -webkit-transform:translateY(100%);
 transform:translateY(100%); }
 .bp3-drawer:not(.bp3-position-top):not(.bp3-position-bottom):not(.bp3-position-left):not(
 .bp3-position-right).bp3-vertical.bp3-overlay-enter-active, .bp3-drawer:not(.bp3-position-top):not(.bp3-position-bottom):not(.bp3-position-left):not(
 .bp3-position-right).bp3-vertical.bp3-overlay-appear-active{
 -webkit-transform:translateY(0);
 transform:translateY(0);
 -webkit-transition-delay:0;
 transition-delay:0;
 -webkit-transition-duration:200ms;
 transition-duration:200ms;
 -webkit-transition-property:-webkit-transform;
 transition-property:-webkit-transform;
 transition-property:transform;
 transition-property:transform, -webkit-transform;
 -webkit-transition-timing-function:cubic-bezier(0.4, 1, 0.75, 0.9);
 transition-timing-function:cubic-bezier(0.4, 1, 0.75, 0.9); }
 .bp3-drawer:not(.bp3-position-top):not(.bp3-position-bottom):not(.bp3-position-left):not(
 .bp3-position-right).bp3-vertical.bp3-overlay-exit{
 -webkit-transform:translateY(0);
 transform:translateY(0); }
 .bp3-drawer:not(.bp3-position-top):not(.bp3-position-bottom):not(.bp3-position-left):not(
 .bp3-position-right).bp3-vertical.bp3-overlay-exit-active{
 -webkit-transform:translateY(100%);
 transform:translateY(100%);
 -webkit-transition-delay:0;
 transition-delay:0;
 -webkit-transition-duration:100ms;
 transition-duration:100ms;
 -webkit-transition-property:-webkit-transform;
 transition-property:-webkit-transform;
 transition-property:transform;
 transition-property:transform, -webkit-transform;
 -webkit-transition-timing-function:cubic-bezier(0.4, 1, 0.75, 0.9);
 transition-timing-function:cubic-bezier(0.4, 1, 0.75, 0.9); }
 .bp3-drawer.bp3-dark,
 .bp3-dark .bp3-drawer{
 background:#30404d;
 -webkit-box-shadow:0 0 0 1px rgba(16, 22, 26, 0.2), 0 4px 8px rgba(16, 22, 26, 0.4), 0 18px 46px 6px rgba(16, 22, 26, 0.4);
 box-shadow:0 0 0 1px rgba(16, 22, 26, 0.2), 0 4px 8px rgba(16, 22, 26, 0.4), 0 18px 46px 6px rgba(16, 22, 26, 0.4);
 color:#f5f8fa; }

.bp3-drawer-header{
 -webkit-box-align:center;
 -ms-flex-align:center;
 align-items:center;
 border-radius:0;
 -webkit-box-shadow:0 1px 0 rgba(16, 22, 26, 0.15);
 box-shadow:0 1px 0 rgba(16, 22, 26, 0.15);
 display:-webkit-box;
 display:-ms-flexbox;
 display:flex;
 -webkit-box-flex:0;
 -ms-flex:0 0 auto;
 flex:0 0 auto;
 min-height:40px;
 padding:5px;
 padding-left:20px;
 position:relative; }
 .bp3-drawer-header .bp3-icon-large,
 .bp3-drawer-header .bp3-icon{
 color:#5c7080;
 -webkit-box-flex:0;
 -ms-flex:0 0 auto;
 flex:0 0 auto;
 margin-right:10px; }
 .bp3-drawer-header .bp3-heading{
 overflow:hidden;
 text-overflow:ellipsis;
 white-space:nowrap;
 word-wrap:normal;
 -webkit-box-flex:1;
 -ms-flex:1 1 auto;
 flex:1 1 auto;
 line-height:inherit;
 margin:0; }
 .bp3-drawer-header .bp3-heading:last-child{
 margin-right:20px; }
 .bp3-dark .bp3-drawer-header{
 -webkit-box-shadow:0 1px 0 rgba(16, 22, 26, 0.4);
 box-shadow:0 1px 0 rgba(16, 22, 26, 0.4); }
 .bp3-dark .bp3-drawer-header .bp3-icon-large,
 .bp3-dark .bp3-drawer-header .bp3-icon{
 color:#a7b6c2; }

.bp3-drawer-body{
 -webkit-box-flex:1;
 -ms-flex:1 1 auto;
 flex:1 1 auto;
 line-height:18px;
 overflow:auto; }

.bp3-drawer-footer{
 -webkit-box-shadow:inset 0 1px 0 rgba(16, 22, 26, 0.15);
 box-shadow:inset 0 1px 0 rgba(16, 22, 26, 0.15);
 -webkit-box-flex:0;
 -ms-flex:0 0 auto;
 flex:0 0 auto;
 padding:10px 20px;
 position:relative; }
 .bp3-dark .bp3-drawer-footer{
 -webkit-box-shadow:inset 0 1px 0 rgba(16, 22, 26, 0.4);
 box-shadow:inset 0 1px 0 rgba(16, 22, 26, 0.4); }
.bp3-editable-text{
 cursor:text;
 display:inline-block;
 max-width:100%;
 position:relative;
 vertical-align:top;
 white-space:nowrap; }
 .bp3-editable-text::before{
 bottom:-3px;
 left:-3px;
 position:absolute;
 right:-3px;
 top:-3px;
 border-radius:3px;
 content:"";
 -webkit-transition:background-color 100ms cubic-bezier(0.4, 1, 0.75, 0.9), -webkit-box-shadow 100ms cubic-bezier(0.4, 1, 0.75, 0.9);
 transition:background-color 100ms cubic-bezier(0.4, 1, 0.75, 0.9), -webkit-box-shadow 100ms cubic-bezier(0.4, 1, 0.75, 0.9);
 transition:background-color 100ms cubic-bezier(0.4, 1, 0.75, 0.9), box-shadow 100ms cubic-bezier(0.4, 1, 0.75, 0.9);
 transition:background-color 100ms cubic-bezier(0.4, 1, 0.75, 0.9), box-shadow 100ms cubic-bezier(0.4, 1, 0.75, 0.9), -webkit-box-shadow 100ms cubic-bezier(0.4, 1, 0.75, 0.9); }
 .bp3-editable-text:hover::before{
 -webkit-box-shadow:0 0 0 0 rgba(19, 124, 189, 0), 0 0 0 0 rgba(19, 124, 189, 0), inset 0 0 0 1px rgba(16, 22, 26, 0.15);
 box-shadow:0 0 0 0 rgba(19, 124, 189, 0), 0 0 0 0 rgba(19, 124, 189, 0), inset 0 0 0 1px rgba(16, 22, 26, 0.15); }
 .bp3-editable-text.bp3-editable-text-editing::before{
 background-color:#ffffff;
 -webkit-box-shadow:0 0 0 1px #137cbd, 0 0 0 3px rgba(19, 124, 189, 0.3), inset 0 1px 1px rgba(16, 22, 26, 0.2);
 box-shadow:0 0 0 1px #137cbd, 0 0 0 3px rgba(19, 124, 189, 0.3), inset 0 1px 1px rgba(16, 22, 26, 0.2); }
 .bp3-editable-text.bp3-disabled::before{
 -webkit-box-shadow:none;
 box-shadow:none; }
 .bp3-editable-text.bp3-intent-primary .bp3-editable-text-input,
 .bp3-editable-text.bp3-intent-primary .bp3-editable-text-content{
 color:#137cbd; }
 .bp3-editable-text.bp3-intent-primary:hover::before{
 -webkit-box-shadow:0 0 0 0 rgba(19, 124, 189, 0), 0 0 0 0 rgba(19, 124, 189, 0), inset 0 0 0 1px rgba(19, 124, 189, 0.4);
 box-shadow:0 0 0 0 rgba(19, 124, 189, 0), 0 0 0 0 rgba(19, 124, 189, 0), inset 0 0 0 1px rgba(19, 124, 189, 0.4); }
 .bp3-editable-text.bp3-intent-primary.bp3-editable-text-editing::before{
 -webkit-box-shadow:0 0 0 1px #137cbd, 0 0 0 3px rgba(19, 124, 189, 0.3), inset 0 1px 1px rgba(16, 22, 26, 0.2);
 box-shadow:0 0 0 1px #137cbd, 0 0 0 3px rgba(19, 124, 189, 0.3), inset 0 1px 1px rgba(16, 22, 26, 0.2); }
 .bp3-editable-text.bp3-intent-success .bp3-editable-text-input,
 .bp3-editable-text.bp3-intent-success .bp3-editable-text-content{
 color:#0f9960; }
 .bp3-editable-text.bp3-intent-success:hover::before{
 -webkit-box-shadow:0 0 0 0 rgba(15, 153, 96, 0), 0 0 0 0 rgba(15, 153, 96, 0), inset 0 0 0 1px rgba(15, 153, 96, 0.4);
 box-shadow:0 0 0 0 rgba(15, 153, 96, 0), 0 0 0 0 rgba(15, 153, 96, 0), inset 0 0 0 1px rgba(15, 153, 96, 0.4); }
 .bp3-editable-text.bp3-intent-success.bp3-editable-text-editing::before{
 -webkit-box-shadow:0 0 0 1px #0f9960, 0 0 0 3px rgba(15, 153, 96, 0.3), inset 0 1px 1px rgba(16, 22, 26, 0.2);
 box-shadow:0 0 0 1px #0f9960, 0 0 0 3px rgba(15, 153, 96, 0.3), inset 0 1px 1px rgba(16, 22, 26, 0.2); }
 .bp3-editable-text.bp3-intent-warning .bp3-editable-text-input,
 .bp3-editable-text.bp3-intent-warning .bp3-editable-text-content{
 color:#d9822b; }
 .bp3-editable-text.bp3-intent-warning:hover::before{
 -webkit-box-shadow:0 0 0 0 rgba(217, 130, 43, 0), 0 0 0 0 rgba(217, 130, 43, 0), inset 0 0 0 1px rgba(217, 130, 43, 0.4);
 box-shadow:0 0 0 0 rgba(217, 130, 43, 0), 0 0 0 0 rgba(217, 130, 43, 0), inset 0 0 0 1px rgba(217, 130, 43, 0.4); }
 .bp3-editable-text.bp3-intent-warning.bp3-editable-text-editing::before{
 -webkit-box-shadow:0 0 0 1px #d9822b, 0 0 0 3px rgba(217, 130, 43, 0.3), inset 0 1px 1px rgba(16, 22, 26, 0.2);
 box-shadow:0 0 0 1px #d9822b, 0 0 0 3px rgba(217, 130, 43, 0.3), inset 0 1px 1px rgba(16, 22, 26, 0.2); }
 .bp3-editable-text.bp3-intent-danger .bp3-editable-text-input,
 .bp3-editable-text.bp3-intent-danger .bp3-editable-text-content{
 color:#db3737; }
 .bp3-editable-text.bp3-intent-danger:hover::before{
 -webkit-box-shadow:0 0 0 0 rgba(219, 55, 55, 0), 0 0 0 0 rgba(219, 55, 55, 0), inset 0 0 0 1px rgba(219, 55, 55, 0.4);
 box-shadow:0 0 0 0 rgba(219, 55, 55, 0), 0 0 0 0 rgba(219, 55, 55, 0), inset 0 0 0 1px rgba(219, 55, 55, 0.4); }
 .bp3-editable-text.bp3-intent-danger.bp3-editable-text-editing::before{
 -webkit-box-shadow:0 0 0 1px #db3737, 0 0 0 3px rgba(219, 55, 55, 0.3), inset 0 1px 1px rgba(16, 22, 26, 0.2);
 box-shadow:0 0 0 1px #db3737, 0 0 0 3px rgba(219, 55, 55, 0.3), inset 0 1px 1px rgba(16, 22, 26, 0.2); }
 .bp3-dark .bp3-editable-text:hover::before{
 -webkit-box-shadow:0 0 0 0 rgba(19, 124, 189, 0), 0 0 0 0 rgba(19, 124, 189, 0), inset 0 0 0 1px rgba(255, 255, 255, 0.15);
 box-shadow:0 0 0 0 rgba(19, 124, 189, 0), 0 0 0 0 rgba(19, 124, 189, 0), inset 0 0 0 1px rgba(255, 255, 255, 0.15); }
 .bp3-dark .bp3-editable-text.bp3-editable-text-editing::before{
 background-color:rgba(16, 22, 26, 0.3);
 -webkit-box-shadow:0 0 0 1px #137cbd, 0 0 0 3px rgba(19, 124, 189, 0.3), inset 0 0 0 1px rgba(16, 22, 26, 0.3), inset 0 1px 1px rgba(16, 22, 26, 0.4);
 box-shadow:0 0 0 1px #137cbd, 0 0 0 3px rgba(19, 124, 189, 0.3), inset 0 0 0 1px rgba(16, 22, 26, 0.3), inset 0 1px 1px rgba(16, 22, 26, 0.4); }
 .bp3-dark .bp3-editable-text.bp3-disabled::before{
 -webkit-box-shadow:none;
 box-shadow:none; }
 .bp3-dark .bp3-editable-text.bp3-intent-primary .bp3-editable-text-content{
 color:#48aff0; }
 .bp3-dark .bp3-editable-text.bp3-intent-primary:hover::before{
 -webkit-box-shadow:0 0 0 0 rgba(72, 175, 240, 0), 0 0 0 0 rgba(72, 175, 240, 0), inset 0 0 0 1px rgba(72, 175, 240, 0.4);
 box-shadow:0 0 0 0 rgba(72, 175, 240, 0), 0 0 0 0 rgba(72, 175, 240, 0), inset 0 0 0 1px rgba(72, 175, 240, 0.4); }
 .bp3-dark .bp3-editable-text.bp3-intent-primary.bp3-editable-text-editing::before{
 -webkit-box-shadow:0 0 0 1px #48aff0, 0 0 0 3px rgba(72, 175, 240, 0.3), inset 0 0 0 1px rgba(16, 22, 26, 0.3), inset 0 1px 1px rgba(16, 22, 26, 0.4);
 box-shadow:0 0 0 1px #48aff0, 0 0 0 3px rgba(72, 175, 240, 0.3), inset 0 0 0 1px rgba(16, 22, 26, 0.3), inset 0 1px 1px rgba(16, 22, 26, 0.4); }
 .bp3-dark .bp3-editable-text.bp3-intent-success .bp3-editable-text-content{
 color:#3dcc91; }
 .bp3-dark .bp3-editable-text.bp3-intent-success:hover::before{
 -webkit-box-shadow:0 0 0 0 rgba(61, 204, 145, 0), 0 0 0 0 rgba(61, 204, 145, 0), inset 0 0 0 1px rgba(61, 204, 145, 0.4);
 box-shadow:0 0 0 0 rgba(61, 204, 145, 0), 0 0 0 0 rgba(61, 204, 145, 0), inset 0 0 0 1px rgba(61, 204, 145, 0.4); }
 .bp3-dark .bp3-editable-text.bp3-intent-success.bp3-editable-text-editing::before{
 -webkit-box-shadow:0 0 0 1px #3dcc91, 0 0 0 3px rgba(61, 204, 145, 0.3), inset 0 0 0 1px rgba(16, 22, 26, 0.3), inset 0 1px 1px rgba(16, 22, 26, 0.4);
 box-shadow:0 0 0 1px #3dcc91, 0 0 0 3px rgba(61, 204, 145, 0.3), inset 0 0 0 1px rgba(16, 22, 26, 0.3), inset 0 1px 1px rgba(16, 22, 26, 0.4); }
 .bp3-dark .bp3-editable-text.bp3-intent-warning .bp3-editable-text-content{
 color:#ffb366; }
 .bp3-dark .bp3-editable-text.bp3-intent-warning:hover::before{
 -webkit-box-shadow:0 0 0 0 rgba(255, 179, 102, 0), 0 0 0 0 rgba(255, 179, 102, 0), inset 0 0 0 1px rgba(255, 179, 102, 0.4);
 box-shadow:0 0 0 0 rgba(255, 179, 102, 0), 0 0 0 0 rgba(255, 179, 102, 0), inset 0 0 0 1px rgba(255, 179, 102, 0.4); }
 .bp3-dark .bp3-editable-text.bp3-intent-warning.bp3-editable-text-editing::before{
 -webkit-box-shadow:0 0 0 1px #ffb366, 0 0 0 3px rgba(255, 179, 102, 0.3), inset 0 0 0 1px rgba(16, 22, 26, 0.3), inset 0 1px 1px rgba(16, 22, 26, 0.4);
 box-shadow:0 0 0 1px #ffb366, 0 0 0 3px rgba(255, 179, 102, 0.3), inset 0 0 0 1px rgba(16, 22, 26, 0.3), inset 0 1px 1px rgba(16, 22, 26, 0.4); }
 .bp3-dark .bp3-editable-text.bp3-intent-danger .bp3-editable-text-content{
 color:#ff7373; }
 .bp3-dark .bp3-editable-text.bp3-intent-danger:hover::before{
 -webkit-box-shadow:0 0 0 0 rgba(255, 115, 115, 0), 0 0 0 0 rgba(255, 115, 115, 0), inset 0 0 0 1px rgba(255, 115, 115, 0.4);
 box-shadow:0 0 0 0 rgba(255, 115, 115, 0), 0 0 0 0 rgba(255, 115, 115, 0), inset 0 0 0 1px rgba(255, 115, 115, 0.4); }
 .bp3-dark .bp3-editable-text.bp3-intent-danger.bp3-editable-text-editing::before{
 -webkit-box-shadow:0 0 0 1px #ff7373, 0 0 0 3px rgba(255, 115, 115, 0.3), inset 0 0 0 1px rgba(16, 22, 26, 0.3), inset 0 1px 1px rgba(16, 22, 26, 0.4);
 box-shadow:0 0 0 1px #ff7373, 0 0 0 3px rgba(255, 115, 115, 0.3), inset 0 0 0 1px rgba(16, 22, 26, 0.3), inset 0 1px 1px rgba(16, 22, 26, 0.4); }

.bp3-editable-text-input,
.bp3-editable-text-content{
 color:inherit;
 display:inherit;
 font:inherit;
 letter-spacing:inherit;
 max-width:inherit;
 min-width:inherit;
 position:relative;
 resize:none;
 text-transform:inherit;
 vertical-align:top; }

.bp3-editable-text-input{
 background:none;
 border:none;
 -webkit-box-shadow:none;
 box-shadow:none;
 padding:0;
 white-space:pre-wrap;
 width:100%; }
 .bp3-editable-text-input::-webkit-input-placeholder{
 color:rgba(92, 112, 128, 0.6);
 opacity:1; }
 .bp3-editable-text-input::-moz-placeholder{
 color:rgba(92, 112, 128, 0.6);
 opacity:1; }
 .bp3-editable-text-input:-ms-input-placeholder{
 color:rgba(92, 112, 128, 0.6);
 opacity:1; }
 .bp3-editable-text-input::-ms-input-placeholder{
 color:rgba(92, 112, 128, 0.6);
 opacity:1; }
 .bp3-editable-text-input::placeholder{
 color:rgba(92, 112, 128, 0.6);
 opacity:1; }
 .bp3-editable-text-input:focus{
 outline:none; }
 .bp3-editable-text-input::-ms-clear{
 display:none; }

.bp3-editable-text-content{
 overflow:hidden;
 padding-right:2px;
 text-overflow:ellipsis;
 white-space:pre; }
 .bp3-editable-text-editing > .bp3-editable-text-content{
 left:0;
 position:absolute;
 visibility:hidden; }
 .bp3-editable-text-placeholder > .bp3-editable-text-content{
 color:rgba(92, 112, 128, 0.6); }
 .bp3-dark .bp3-editable-text-placeholder > .bp3-editable-text-content{
 color:rgba(167, 182, 194, 0.6); }

.bp3-editable-text.bp3-multiline{
 display:block; }
 .bp3-editable-text.bp3-multiline .bp3-editable-text-content{
 overflow:auto;
 white-space:pre-wrap;
 word-wrap:break-word; }
.bp3-divider{
 border-bottom:1px solid rgba(16, 22, 26, 0.15);
 border-right:1px solid rgba(16, 22, 26, 0.15);
 margin:5px; }
 .bp3-dark .bp3-divider{
 border-color:rgba(16, 22, 26, 0.4); }
.bp3-control-group{
 -webkit-transform:translateZ(0);
 transform:translateZ(0);
 display:-webkit-box;
 display:-ms-flexbox;
 display:flex;
 -webkit-box-orient:horizontal;
 -webkit-box-direction:normal;
 -ms-flex-direction:row;
 flex-direction:row;
 -webkit-box-align:stretch;
 -ms-flex-align:stretch;
 align-items:stretch; }
 .bp3-control-group > \*{
 -webkit-box-flex:0;
 -ms-flex-positive:0;
 flex-grow:0;
 -ms-flex-negative:0;
 flex-shrink:0; }
 .bp3-control-group > .bp3-fill{
 -webkit-box-flex:1;
 -ms-flex-positive:1;
 flex-grow:1;
 -ms-flex-negative:1;
 flex-shrink:1; }
 .bp3-control-group .bp3-button,
 .bp3-control-group .bp3-html-select,
 .bp3-control-group .bp3-input,
 .bp3-control-group .bp3-select{
 position:relative; }
 .bp3-control-group .bp3-input{
 border-radius:inherit;
 z-index:2; }
 .bp3-control-group .bp3-input:focus{
 border-radius:3px;
 z-index:14; }
 .bp3-control-group .bp3-input[class\*="bp3-intent"]{
 z-index:13; }
 .bp3-control-group .bp3-input[class\*="bp3-intent"]:focus{
 z-index:15; }
 .bp3-control-group .bp3-input[readonly], .bp3-control-group .bp3-input:disabled, .bp3-control-group .bp3-input.bp3-disabled{
 z-index:1; }
 .bp3-control-group .bp3-input-group[class\*="bp3-intent"] .bp3-input{
 z-index:13; }
 .bp3-control-group .bp3-input-group[class\*="bp3-intent"] .bp3-input:focus{
 z-index:15; }
 .bp3-control-group .bp3-button,
 .bp3-control-group .bp3-html-select select,
 .bp3-control-group .bp3-select select{
 -webkit-transform:translateZ(0);
 transform:translateZ(0);
 border-radius:inherit;
 z-index:4; }
 .bp3-control-group .bp3-button:focus,
 .bp3-control-group .bp3-html-select select:focus,
 .bp3-control-group .bp3-select select:focus{
 z-index:5; }
 .bp3-control-group .bp3-button:hover,
 .bp3-control-group .bp3-html-select select:hover,
 .bp3-control-group .bp3-select select:hover{
 z-index:6; }
 .bp3-control-group .bp3-button:active,
 .bp3-control-group .bp3-html-select select:active,
 .bp3-control-group .bp3-select select:active{
 z-index:7; }
 .bp3-control-group .bp3-button[readonly], .bp3-control-group .bp3-button:disabled, .bp3-control-group .bp3-button.bp3-disabled,
 .bp3-control-group .bp3-html-select select[readonly],
 .bp3-control-group .bp3-html-select select:disabled,
 .bp3-control-group .bp3-html-select select.bp3-disabled,
 .bp3-control-group .bp3-select select[readonly],
 .bp3-control-group .bp3-select select:disabled,
 .bp3-control-group .bp3-select select.bp3-disabled{
 z-index:3; }
 .bp3-control-group .bp3-button[class\*="bp3-intent"],
 .bp3-control-group .bp3-html-select select[class\*="bp3-intent"],
 .bp3-control-group .bp3-select select[class\*="bp3-intent"]{
 z-index:9; }
 .bp3-control-group .bp3-button[class\*="bp3-intent"]:focus,
 .bp3-control-group .bp3-html-select select[class\*="bp3-intent"]:focus,
 .bp3-control-group .bp3-select select[class\*="bp3-intent"]:focus{
 z-index:10; }
 .bp3-control-group .bp3-button[class\*="bp3-intent"]:hover,
 .bp3-control-group .bp3-html-select select[class\*="bp3-intent"]:hover,
 .bp3-control-group .bp3-select select[class\*="bp3-intent"]:hover{
 z-index:11; }
 .bp3-control-group .bp3-button[class\*="bp3-intent"]:active,
 .bp3-control-group .bp3-html-select select[class\*="bp3-intent"]:active,
 .bp3-control-group .bp3-select select[class\*="bp3-intent"]:active{
 z-index:12; }
 .bp3-control-group .bp3-button[class\*="bp3-intent"][readonly], .bp3-control-group .bp3-button[class\*="bp3-intent"]:disabled, .bp3-control-group .bp3-button[class\*="bp3-intent"].bp3-disabled,
 .bp3-control-group .bp3-html-select select[class\*="bp3-intent"][readonly],
 .bp3-control-group .bp3-html-select select[class\*="bp3-intent"]:disabled,
 .bp3-control-group .bp3-html-select select[class\*="bp3-intent"].bp3-disabled,
 .bp3-control-group .bp3-select select[class\*="bp3-intent"][readonly],
 .bp3-control-group .bp3-select select[class\*="bp3-intent"]:disabled,
 .bp3-control-group .bp3-select select[class\*="bp3-intent"].bp3-disabled{
 z-index:8; }
 .bp3-control-group .bp3-input-group > .bp3-icon,
 .bp3-control-group .bp3-input-group > .bp3-button,
 .bp3-control-group .bp3-input-group > .bp3-input-left-container,
 .bp3-control-group .bp3-input-group > .bp3-input-action{
 z-index:16; }
 .bp3-control-group .bp3-select::after,
 .bp3-control-group .bp3-html-select::after,
 .bp3-control-group .bp3-select > .bp3-icon,
 .bp3-control-group .bp3-html-select > .bp3-icon{
 z-index:17; }
 .bp3-control-group .bp3-select:focus-within{
 z-index:5; }
 .bp3-control-group:not(.bp3-vertical) > \*:not(.bp3-divider){
 margin-right:-1px; }
 .bp3-control-group:not(.bp3-vertical) > .bp3-divider:not(:first-child){
 margin-left:6px; }
 .bp3-dark .bp3-control-group:not(.bp3-vertical) > \*:not(.bp3-divider){
 margin-right:0; }
 .bp3-dark .bp3-control-group:not(.bp3-vertical) > .bp3-button + .bp3-button{
 margin-left:1px; }
 .bp3-control-group .bp3-popover-wrapper,
 .bp3-control-group .bp3-popover-target{
 border-radius:inherit; }
 .bp3-control-group > :first-child{
 border-radius:3px 0 0 3px; }
 .bp3-control-group > :last-child{
 border-radius:0 3px 3px 0;
 margin-right:0; }
 .bp3-control-group > :only-child{
 border-radius:3px;
 margin-right:0; }
 .bp3-control-group .bp3-input-group .bp3-button{
 border-radius:3px; }
 .bp3-control-group .bp3-numeric-input:not(:first-child) .bp3-input-group{
 border-bottom-left-radius:0;
 border-top-left-radius:0; }
 .bp3-control-group.bp3-fill{
 width:100%; }
 .bp3-control-group > .bp3-fill{
 -webkit-box-flex:1;
 -ms-flex:1 1 auto;
 flex:1 1 auto; }
 .bp3-control-group.bp3-fill > \*:not(.bp3-fixed){
 -webkit-box-flex:1;
 -ms-flex:1 1 auto;
 flex:1 1 auto; }
 .bp3-control-group.bp3-vertical{
 -webkit-box-orient:vertical;
 -webkit-box-direction:normal;
 -ms-flex-direction:column;
 flex-direction:column; }
 .bp3-control-group.bp3-vertical > \*{
 margin-top:-1px; }
 .bp3-control-group.bp3-vertical > :first-child{
 border-radius:3px 3px 0 0;
 margin-top:0; }
 .bp3-control-group.bp3-vertical > :last-child{
 border-radius:0 0 3px 3px; }
.bp3-control{
 cursor:pointer;
 display:block;
 margin-bottom:10px;
 position:relative;
 text-transform:none; }
 .bp3-control input:checked ~ .bp3-control-indicator{
 background-color:#137cbd;
 background-image:-webkit-gradient(linear, left top, left bottom, from(rgba(255, 255, 255, 0.1)), to(rgba(255, 255, 255, 0)));
 background-image:linear-gradient(to bottom, rgba(255, 255, 255, 0.1), rgba(255, 255, 255, 0));
 -webkit-box-shadow:inset 0 0 0 1px rgba(16, 22, 26, 0.4), inset 0 -1px 0 rgba(16, 22, 26, 0.2);
 box-shadow:inset 0 0 0 1px rgba(16, 22, 26, 0.4), inset 0 -1px 0 rgba(16, 22, 26, 0.2);
 color:#ffffff; }
 .bp3-control:hover input:checked ~ .bp3-control-indicator{
 background-color:#106ba3;
 -webkit-box-shadow:inset 0 0 0 1px rgba(16, 22, 26, 0.4), inset 0 -1px 0 rgba(16, 22, 26, 0.2);
 box-shadow:inset 0 0 0 1px rgba(16, 22, 26, 0.4), inset 0 -1px 0 rgba(16, 22, 26, 0.2); }
 .bp3-control input:not(:disabled):active:checked ~ .bp3-control-indicator{
 background:#0e5a8a;
 -webkit-box-shadow:inset 0 0 0 1px rgba(16, 22, 26, 0.4), inset 0 1px 2px rgba(16, 22, 26, 0.2);
 box-shadow:inset 0 0 0 1px rgba(16, 22, 26, 0.4), inset 0 1px 2px rgba(16, 22, 26, 0.2); }
 .bp3-control input:disabled:checked ~ .bp3-control-indicator{
 background:rgba(19, 124, 189, 0.5);
 -webkit-box-shadow:none;
 box-shadow:none; }
 .bp3-dark .bp3-control input:checked ~ .bp3-control-indicator{
 -webkit-box-shadow:0 0 0 1px rgba(16, 22, 26, 0.4);
 box-shadow:0 0 0 1px rgba(16, 22, 26, 0.4); }
 .bp3-dark .bp3-control:hover input:checked ~ .bp3-control-indicator{
 background-color:#106ba3;
 -webkit-box-shadow:0 0 0 1px rgba(16, 22, 26, 0.4);
 box-shadow:0 0 0 1px rgba(16, 22, 26, 0.4); }
 .bp3-dark .bp3-control input:not(:disabled):active:checked ~ .bp3-control-indicator{
 background-color:#0e5a8a;
 -webkit-box-shadow:0 0 0 1px rgba(16, 22, 26, 0.4), inset 0 1px 2px rgba(16, 22, 26, 0.2);
 box-shadow:0 0 0 1px rgba(16, 22, 26, 0.4), inset 0 1px 2px rgba(16, 22, 26, 0.2); }
 .bp3-dark .bp3-control input:disabled:checked ~ .bp3-control-indicator{
 background:rgba(14, 90, 138, 0.5);
 -webkit-box-shadow:none;
 box-shadow:none; }
 .bp3-control:not(.bp3-align-right){
 padding-left:26px; }
 .bp3-control:not(.bp3-align-right) .bp3-control-indicator{
 margin-left:-26px; }
 .bp3-control.bp3-align-right{
 padding-right:26px; }
 .bp3-control.bp3-align-right .bp3-control-indicator{
 margin-right:-26px; }
 .bp3-control.bp3-disabled{
 color:rgba(92, 112, 128, 0.6);
 cursor:not-allowed; }
 .bp3-control.bp3-inline{
 display:inline-block;
 margin-right:20px; }
 .bp3-control input{
 left:0;
 opacity:0;
 position:absolute;
 top:0;
 z-index:-1; }
 .bp3-control .bp3-control-indicator{
 background-clip:padding-box;
 background-color:#f5f8fa;
 background-image:-webkit-gradient(linear, left top, left bottom, from(rgba(255, 255, 255, 0.8)), to(rgba(255, 255, 255, 0)));
 background-image:linear-gradient(to bottom, rgba(255, 255, 255, 0.8), rgba(255, 255, 255, 0));
 border:none;
 -webkit-box-shadow:inset 0 0 0 1px rgba(16, 22, 26, 0.2), inset 0 -1px 0 rgba(16, 22, 26, 0.1);
 box-shadow:inset 0 0 0 1px rgba(16, 22, 26, 0.2), inset 0 -1px 0 rgba(16, 22, 26, 0.1);
 cursor:pointer;
 display:inline-block;
 font-size:16px;
 height:1em;
 margin-right:10px;
 margin-top:-3px;
 position:relative;
 -webkit-user-select:none;
 -moz-user-select:none;
 -ms-user-select:none;
 user-select:none;
 vertical-align:middle;
 width:1em; }
 .bp3-control .bp3-control-indicator::before{
 content:"";
 display:block;
 height:1em;
 width:1em; }
 .bp3-control:hover .bp3-control-indicator{
 background-color:#ebf1f5; }
 .bp3-control input:not(:disabled):active ~ .bp3-control-indicator{
 background:#d8e1e8;
 -webkit-box-shadow:inset 0 0 0 1px rgba(16, 22, 26, 0.2), inset 0 1px 2px rgba(16, 22, 26, 0.2);
 box-shadow:inset 0 0 0 1px rgba(16, 22, 26, 0.2), inset 0 1px 2px rgba(16, 22, 26, 0.2); }
 .bp3-control input:disabled ~ .bp3-control-indicator{
 background:rgba(206, 217, 224, 0.5);
 -webkit-box-shadow:none;
 box-shadow:none;
 cursor:not-allowed; }
 .bp3-control input:focus ~ .bp3-control-indicator{
 outline:rgba(19, 124, 189, 0.6) auto 2px;
 outline-offset:2px;
 -moz-outline-radius:6px; }
 .bp3-control.bp3-align-right .bp3-control-indicator{
 float:right;
 margin-left:10px;
 margin-top:1px; }
 .bp3-control.bp3-large{
 font-size:16px; }
 .bp3-control.bp3-large:not(.bp3-align-right){
 padding-left:30px; }
 .bp3-control.bp3-large:not(.bp3-align-right) .bp3-control-indicator{
 margin-left:-30px; }
 .bp3-control.bp3-large.bp3-align-right{
 padding-right:30px; }
 .bp3-control.bp3-large.bp3-align-right .bp3-control-indicator{
 margin-right:-30px; }
 .bp3-control.bp3-large .bp3-control-indicator{
 font-size:20px; }
 .bp3-control.bp3-large.bp3-align-right .bp3-control-indicator{
 margin-top:0; }
 .bp3-control.bp3-checkbox input:indeterminate ~ .bp3-control-indicator{
 background-color:#137cbd;
 background-image:-webkit-gradient(linear, left top, left bottom, from(rgba(255, 255, 255, 0.1)), to(rgba(255, 255, 255, 0)));
 background-image:linear-gradient(to bottom, rgba(255, 255, 255, 0.1), rgba(255, 255, 255, 0));
 -webkit-box-shadow:inset 0 0 0 1px rgba(16, 22, 26, 0.4), inset 0 -1px 0 rgba(16, 22, 26, 0.2);
 box-shadow:inset 0 0 0 1px rgba(16, 22, 26, 0.4), inset 0 -1px 0 rgba(16, 22, 26, 0.2);
 color:#ffffff; }
 .bp3-control.bp3-checkbox:hover input:indeterminate ~ .bp3-control-indicator{
 background-color:#106ba3;
 -webkit-box-shadow:inset 0 0 0 1px rgba(16, 22, 26, 0.4), inset 0 -1px 0 rgba(16, 22, 26, 0.2);
 box-shadow:inset 0 0 0 1px rgba(16, 22, 26, 0.4), inset 0 -1px 0 rgba(16, 22, 26, 0.2); }
 .bp3-control.bp3-checkbox input:not(:disabled):active:indeterminate ~ .bp3-control-indicator{
 background:#0e5a8a;
 -webkit-box-shadow:inset 0 0 0 1px rgba(16, 22, 26, 0.4), inset 0 1px 2px rgba(16, 22, 26, 0.2);
 box-shadow:inset 0 0 0 1px rgba(16, 22, 26, 0.4), inset 0 1px 2px rgba(16, 22, 26, 0.2); }
 .bp3-control.bp3-checkbox input:disabled:indeterminate ~ .bp3-control-indicator{
 background:rgba(19, 124, 189, 0.5);
 -webkit-box-shadow:none;
 box-shadow:none; }
 .bp3-dark .bp3-control.bp3-checkbox input:indeterminate ~ .bp3-control-indicator{
 -webkit-box-shadow:0 0 0 1px rgba(16, 22, 26, 0.4);
 box-shadow:0 0 0 1px rgba(16, 22, 26, 0.4); }
 .bp3-dark .bp3-control.bp3-checkbox:hover input:indeterminate ~ .bp3-control-indicator{
 background-color:#106ba3;
 -webkit-box-shadow:0 0 0 1px rgba(16, 22, 26, 0.4);
 box-shadow:0 0 0 1px rgba(16, 22, 26, 0.4); }
 .bp3-dark .bp3-control.bp3-checkbox input:not(:disabled):active:indeterminate ~ .bp3-control-indicator{
 background-color:#0e5a8a;
 -webkit-box-shadow:0 0 0 1px rgba(16, 22, 26, 0.4), inset 0 1px 2px rgba(16, 22, 26, 0.2);
 box-shadow:0 0 0 1px rgba(16, 22, 26, 0.4), inset 0 1px 2px rgba(16, 22, 26, 0.2); }
 .bp3-dark .bp3-control.bp3-checkbox input:disabled:indeterminate ~ .bp3-control-indicator{
 background:rgba(14, 90, 138, 0.5);
 -webkit-box-shadow:none;
 box-shadow:none; }
 .bp3-control.bp3-checkbox .bp3-control-indicator{
 border-radius:3px; }
 .bp3-control.bp3-checkbox input:checked ~ .bp3-control-indicator::before{
 background-image:url("data:image/svg+xml,%3csvg xmlns='http://www.w3.org/2000/svg' viewBox='0 0 16 16'%3e%3cpath fill-rule='evenodd' clip-rule='evenodd' d='M12 5c-.28 0-.53.11-.71.29L7 9.59l-2.29-2.3a1.003 1.003 0 00-1.42 1.42l3 3c.18.18.43.29.71.29s.53-.11.71-.29l5-5A1.003 1.003 0 0012 5z' fill='white'/%3e%3c/svg%3e"); }
 .bp3-control.bp3-checkbox input:indeterminate ~ .bp3-control-indicator::before{
 background-image:url("data:image/svg+xml,%3csvg xmlns='http://www.w3.org/2000/svg' viewBox='0 0 16 16'%3e%3cpath fill-rule='evenodd' clip-rule='evenodd' d='M11 7H5c-.55 0-1 .45-1 1s.45 1 1 1h6c.55 0 1-.45 1-1s-.45-1-1-1z' fill='white'/%3e%3c/svg%3e"); }
 .bp3-control.bp3-radio .bp3-control-indicator{
 border-radius:50%; }
 .bp3-control.bp3-radio input:checked ~ .bp3-control-indicator::before{
 background-image:radial-gradient(#ffffff, #ffffff 28%, transparent 32%); }
 .bp3-control.bp3-radio input:checked:disabled ~ .bp3-control-indicator::before{
 opacity:0.5; }
 .bp3-control.bp3-radio input:focus ~ .bp3-control-indicator{
 -moz-outline-radius:16px; }
 .bp3-control.bp3-switch input ~ .bp3-control-indicator{
 background:rgba(167, 182, 194, 0.5); }
 .bp3-control.bp3-switch:hover input ~ .bp3-control-indicator{
 background:rgba(115, 134, 148, 0.5); }
 .bp3-control.bp3-switch input:not(:disabled):active ~ .bp3-control-indicator{
 background:rgba(92, 112, 128, 0.5); }
 .bp3-control.bp3-switch input:disabled ~ .bp3-control-indicator{
 background:rgba(206, 217, 224, 0.5); }
 .bp3-control.bp3-switch input:disabled ~ .bp3-control-indicator::before{
 background:rgba(255, 255, 255, 0.8); }
 .bp3-control.bp3-switch input:checked ~ .bp3-control-indicator{
 background:#137cbd; }
 .bp3-control.bp3-switch:hover input:checked ~ .bp3-control-indicator{
 background:#106ba3; }
 .bp3-control.bp3-switch input:checked:not(:disabled):active ~ .bp3-control-indicator{
 background:#0e5a8a; }
 .bp3-control.bp3-switch input:checked:disabled ~ .bp3-control-indicator{
 background:rgba(19, 124, 189, 0.5); }
 .bp3-control.bp3-switch input:checked:disabled ~ .bp3-control-indicator::before{
 background:rgba(255, 255, 255, 0.8); }
 .bp3-control.bp3-switch:not(.bp3-align-right){
 padding-left:38px; }
 .bp3-control.bp3-switch:not(.bp3-align-right) .bp3-control-indicator{
 margin-left:-38px; }
 .bp3-control.bp3-switch.bp3-align-right{
 padding-right:38px; }
 .bp3-control.bp3-switch.bp3-align-right .bp3-control-indicator{
 margin-right:-38px; }
 .bp3-control.bp3-switch .bp3-control-indicator{
 border:none;
 border-radius:1.75em;
 -webkit-box-shadow:none !important;
 box-shadow:none !important;
 min-width:1.75em;
 -webkit-transition:background-color 100ms cubic-bezier(0.4, 1, 0.75, 0.9);
 transition:background-color 100ms cubic-bezier(0.4, 1, 0.75, 0.9);
 width:auto; }
 .bp3-control.bp3-switch .bp3-control-indicator::before{
 background:#ffffff;
 border-radius:50%;
 -webkit-box-shadow:0 0 0 1px rgba(16, 22, 26, 0.2), 0 1px 1px rgba(16, 22, 26, 0.2);
 box-shadow:0 0 0 1px rgba(16, 22, 26, 0.2), 0 1px 1px rgba(16, 22, 26, 0.2);
 height:calc(1em - 4px);
 left:0;
 margin:2px;
 position:absolute;
 -webkit-transition:left 100ms cubic-bezier(0.4, 1, 0.75, 0.9);
 transition:left 100ms cubic-bezier(0.4, 1, 0.75, 0.9);
 width:calc(1em - 4px); }
 .bp3-control.bp3-switch input:checked ~ .bp3-control-indicator::before{
 left:calc(100% - 1em); }
 .bp3-control.bp3-switch.bp3-large:not(.bp3-align-right){
 padding-left:45px; }
 .bp3-control.bp3-switch.bp3-large:not(.bp3-align-right) .bp3-control-indicator{
 margin-left:-45px; }
 .bp3-control.bp3-switch.bp3-large.bp3-align-right{
 padding-right:45px; }
 .bp3-control.bp3-switch.bp3-large.bp3-align-right .bp3-control-indicator{
 margin-right:-45px; }
 .bp3-dark .bp3-control.bp3-switch input ~ .bp3-control-indicator{
 background:rgba(16, 22, 26, 0.5); }
 .bp3-dark .bp3-control.bp3-switch:hover input ~ .bp3-control-indicator{
 background:rgba(16, 22, 26, 0.7); }
 .bp3-dark .bp3-control.bp3-switch input:not(:disabled):active ~ .bp3-control-indicator{
 background:rgba(16, 22, 26, 0.9); }
 .bp3-dark .bp3-control.bp3-switch input:disabled ~ .bp3-control-indicator{
 background:rgba(57, 75, 89, 0.5); }
 .bp3-dark .bp3-control.bp3-switch input:disabled ~ .bp3-control-indicator::before{
 background:rgba(16, 22, 26, 0.4); }
 .bp3-dark .bp3-control.bp3-switch input:checked ~ .bp3-control-indicator{
 background:#137cbd; }
 .bp3-dark .bp3-control.bp3-switch:hover input:checked ~ .bp3-control-indicator{
 background:#106ba3; }
 .bp3-dark .bp3-control.bp3-switch input:checked:not(:disabled):active ~ .bp3-control-indicator{
 background:#0e5a8a; }
 .bp3-dark .bp3-control.bp3-switch input:checked:disabled ~ .bp3-control-indicator{
 background:rgba(14, 90, 138, 0.5); }
 .bp3-dark .bp3-control.bp3-switch input:checked:disabled ~ .bp3-control-indicator::before{
 background:rgba(16, 22, 26, 0.4); }
 .bp3-dark .bp3-control.bp3-switch .bp3-control-indicator::before{
 background:#394b59;
 -webkit-box-shadow:0 0 0 1px rgba(16, 22, 26, 0.4);
 box-shadow:0 0 0 1px rgba(16, 22, 26, 0.4); }
 .bp3-dark .bp3-control.bp3-switch input:checked ~ .bp3-control-indicator::before{
 -webkit-box-shadow:inset 0 0 0 1px rgba(16, 22, 26, 0.4);
 box-shadow:inset 0 0 0 1px rgba(16, 22, 26, 0.4); }
 .bp3-control.bp3-switch .bp3-switch-inner-text{
 font-size:0.7em;
 text-align:center; }
 .bp3-control.bp3-switch .bp3-control-indicator-child:first-child{
 line-height:0;
 margin-left:0.5em;
 margin-right:1.2em;
 visibility:hidden; }
 .bp3-control.bp3-switch .bp3-control-indicator-child:last-child{
 line-height:1em;
 margin-left:1.2em;
 margin-right:0.5em;
 visibility:visible; }
 .bp3-control.bp3-switch input:checked ~ .bp3-control-indicator .bp3-control-indicator-child:first-child{
 line-height:1em;
 visibility:visible; }
 .bp3-control.bp3-switch input:checked ~ .bp3-control-indicator .bp3-control-indicator-child:last-child{
 line-height:0;
 visibility:hidden; }
 .bp3-dark .bp3-control{
 color:#f5f8fa; }
 .bp3-dark .bp3-control.bp3-disabled{
 color:rgba(167, 182, 194, 0.6); }
 .bp3-dark .bp3-control .bp3-control-indicator{
 background-color:#394b59;
 background-image:-webkit-gradient(linear, left top, left bottom, from(rgba(255, 255, 255, 0.05)), to(rgba(255, 255, 255, 0)));
 background-image:linear-gradient(to bottom, rgba(255, 255, 255, 0.05), rgba(255, 255, 255, 0));
 -webkit-box-shadow:0 0 0 1px rgba(16, 22, 26, 0.4);
 box-shadow:0 0 0 1px rgba(16, 22, 26, 0.4); }
 .bp3-dark .bp3-control:hover .bp3-control-indicator{
 background-color:#30404d; }
 .bp3-dark .bp3-control input:not(:disabled):active ~ .bp3-control-indicator{
 background:#202b33;
 -webkit-box-shadow:0 0 0 1px rgba(16, 22, 26, 0.6), inset 0 1px 2px rgba(16, 22, 26, 0.2);
 box-shadow:0 0 0 1px rgba(16, 22, 26, 0.6), inset 0 1px 2px rgba(16, 22, 26, 0.2); }
 .bp3-dark .bp3-control input:disabled ~ .bp3-control-indicator{
 background:rgba(57, 75, 89, 0.5);
 -webkit-box-shadow:none;
 box-shadow:none;
 cursor:not-allowed; }
 .bp3-dark .bp3-control.bp3-checkbox input:disabled:checked ~ .bp3-control-indicator, .bp3-dark .bp3-control.bp3-checkbox input:disabled:indeterminate ~ .bp3-control-indicator{
 color:rgba(167, 182, 194, 0.6); }
.bp3-file-input{
 cursor:pointer;
 display:inline-block;
 height:30px;
 position:relative; }
 .bp3-file-input input{
 margin:0;
 min-width:200px;
 opacity:0; }
 .bp3-file-input input:disabled + .bp3-file-upload-input,
 .bp3-file-input input.bp3-disabled + .bp3-file-upload-input{
 background:rgba(206, 217, 224, 0.5);
 -webkit-box-shadow:none;
 box-shadow:none;
 color:rgba(92, 112, 128, 0.6);
 cursor:not-allowed;
 resize:none; }
 .bp3-file-input input:disabled + .bp3-file-upload-input::after,
 .bp3-file-input input.bp3-disabled + .bp3-file-upload-input::after{
 background-color:rgba(206, 217, 224, 0.5);
 background-image:none;
 -webkit-box-shadow:none;
 box-shadow:none;
 color:rgba(92, 112, 128, 0.6);
 cursor:not-allowed;
 outline:none; }
 .bp3-file-input input:disabled + .bp3-file-upload-input::after.bp3-active, .bp3-file-input input:disabled + .bp3-file-upload-input::after.bp3-active:hover,
 .bp3-file-input input.bp3-disabled + .bp3-file-upload-input::after.bp3-active,
 .bp3-file-input input.bp3-disabled + .bp3-file-upload-input::after.bp3-active:hover{
 background:rgba(206, 217, 224, 0.7); }
 .bp3-dark .bp3-file-input input:disabled + .bp3-file-upload-input, .bp3-dark
 .bp3-file-input input.bp3-disabled + .bp3-file-upload-input{
 background:rgba(57, 75, 89, 0.5);
 -webkit-box-shadow:none;
 box-shadow:none;
 color:rgba(167, 182, 194, 0.6); }
 .bp3-dark .bp3-file-input input:disabled + .bp3-file-upload-input::after, .bp3-dark
 .bp3-file-input input.bp3-disabled + .bp3-file-upload-input::after{
 background-color:rgba(57, 75, 89, 0.5);
 background-image:none;
 -webkit-box-shadow:none;
 box-shadow:none;
 color:rgba(167, 182, 194, 0.6); }
 .bp3-dark .bp3-file-input input:disabled + .bp3-file-upload-input::after.bp3-active, .bp3-dark
 .bp3-file-input input.bp3-disabled + .bp3-file-upload-input::after.bp3-active{
 background:rgba(57, 75, 89, 0.7); }
 .bp3-file-input.bp3-file-input-has-selection .bp3-file-upload-input{
 color:#182026; }
 .bp3-dark .bp3-file-input.bp3-file-input-has-selection .bp3-file-upload-input{
 color:#f5f8fa; }
 .bp3-file-input.bp3-fill{
 width:100%; }
 .bp3-file-input.bp3-large,
 .bp3-large .bp3-file-input{
 height:40px; }
 .bp3-file-input .bp3-file-upload-input-custom-text::after{
 content:attr(bp3-button-text); }

.bp3-file-upload-input{
 -webkit-appearance:none;
 -moz-appearance:none;
 appearance:none;
 background:#ffffff;
 border:none;
 border-radius:3px;
 -webkit-box-shadow:0 0 0 0 rgba(19, 124, 189, 0), 0 0 0 0 rgba(19, 124, 189, 0), inset 0 0 0 1px rgba(16, 22, 26, 0.15), inset 0 1px 1px rgba(16, 22, 26, 0.2);
 box-shadow:0 0 0 0 rgba(19, 124, 189, 0), 0 0 0 0 rgba(19, 124, 189, 0), inset 0 0 0 1px rgba(16, 22, 26, 0.15), inset 0 1px 1px rgba(16, 22, 26, 0.2);
 color:#182026;
 font-size:14px;
 font-weight:400;
 height:30px;
 line-height:30px;
 outline:none;
 padding:0 10px;
 -webkit-transition:-webkit-box-shadow 100ms cubic-bezier(0.4, 1, 0.75, 0.9);
 transition:-webkit-box-shadow 100ms cubic-bezier(0.4, 1, 0.75, 0.9);
 transition:box-shadow 100ms cubic-bezier(0.4, 1, 0.75, 0.9);
 transition:box-shadow 100ms cubic-bezier(0.4, 1, 0.75, 0.9), -webkit-box-shadow 100ms cubic-bezier(0.4, 1, 0.75, 0.9);
 vertical-align:middle;
 overflow:hidden;
 text-overflow:ellipsis;
 white-space:nowrap;
 word-wrap:normal;
 color:rgba(92, 112, 128, 0.6);
 left:0;
 padding-right:80px;
 position:absolute;
 right:0;
 top:0;
 -webkit-user-select:none;
 -moz-user-select:none;
 -ms-user-select:none;
 user-select:none; }
 .bp3-file-upload-input::-webkit-input-placeholder{
 color:rgba(92, 112, 128, 0.6);
 opacity:1; }
 .bp3-file-upload-input::-moz-placeholder{
 color:rgba(92, 112, 128, 0.6);
 opacity:1; }
 .bp3-file-upload-input:-ms-input-placeholder{
 color:rgba(92, 112, 128, 0.6);
 opacity:1; }
 .bp3-file-upload-input::-ms-input-placeholder{
 color:rgba(92, 112, 128, 0.6);
 opacity:1; }
 .bp3-file-upload-input::placeholder{
 color:rgba(92, 112, 128, 0.6);
 opacity:1; }
 .bp3-file-upload-input:focus, .bp3-file-upload-input.bp3-active{
 -webkit-box-shadow:0 0 0 1px #137cbd, 0 0 0 3px rgba(19, 124, 189, 0.3), inset 0 1px 1px rgba(16, 22, 26, 0.2);
 box-shadow:0 0 0 1px #137cbd, 0 0 0 3px rgba(19, 124, 189, 0.3), inset 0 1px 1px rgba(16, 22, 26, 0.2); }
 .bp3-file-upload-input[type="search"], .bp3-file-upload-input.bp3-round{
 border-radius:30px;
 -webkit-box-sizing:border-box;
 box-sizing:border-box;
 padding-left:10px; }
 .bp3-file-upload-input[readonly]{
 -webkit-box-shadow:inset 0 0 0 1px rgba(16, 22, 26, 0.15);
 box-shadow:inset 0 0 0 1px rgba(16, 22, 26, 0.15); }
 .bp3-file-upload-input:disabled, .bp3-file-upload-input.bp3-disabled{
 background:rgba(206, 217, 224, 0.5);
 -webkit-box-shadow:none;
 box-shadow:none;
 color:rgba(92, 112, 128, 0.6);
 cursor:not-allowed;
 resize:none; }
 .bp3-file-upload-input::after{
 background-color:#f5f8fa;
 background-image:-webkit-gradient(linear, left top, left bottom, from(rgba(255, 255, 255, 0.8)), to(rgba(255, 255, 255, 0)));
 background-image:linear-gradient(to bottom, rgba(255, 255, 255, 0.8), rgba(255, 255, 255, 0));
 -webkit-box-shadow:inset 0 0 0 1px rgba(16, 22, 26, 0.2), inset 0 -1px 0 rgba(16, 22, 26, 0.1);
 box-shadow:inset 0 0 0 1px rgba(16, 22, 26, 0.2), inset 0 -1px 0 rgba(16, 22, 26, 0.1);
 color:#182026;
 min-height:24px;
 min-width:24px;
 overflow:hidden;
 text-overflow:ellipsis;
 white-space:nowrap;
 word-wrap:normal;
 border-radius:3px;
 content:"Browse";
 line-height:24px;
 margin:3px;
 position:absolute;
 right:0;
 text-align:center;
 top:0;
 width:70px; }
 .bp3-file-upload-input::after:hover{
 background-clip:padding-box;
 background-color:#ebf1f5;
 -webkit-box-shadow:inset 0 0 0 1px rgba(16, 22, 26, 0.2), inset 0 -1px 0 rgba(16, 22, 26, 0.1);
 box-shadow:inset 0 0 0 1px rgba(16, 22, 26, 0.2), inset 0 -1px 0 rgba(16, 22, 26, 0.1); }
 .bp3-file-upload-input::after:active, .bp3-file-upload-input::after.bp3-active{
 background-color:#d8e1e8;
 background-image:none;
 -webkit-box-shadow:inset 0 0 0 1px rgba(16, 22, 26, 0.2), inset 0 1px 2px rgba(16, 22, 26, 0.2);
 box-shadow:inset 0 0 0 1px rgba(16, 22, 26, 0.2), inset 0 1px 2px rgba(16, 22, 26, 0.2); }
 .bp3-file-upload-input::after:disabled, .bp3-file-upload-input::after.bp3-disabled{
 background-color:rgba(206, 217, 224, 0.5);
 background-image:none;
 -webkit-box-shadow:none;
 box-shadow:none;
 color:rgba(92, 112, 128, 0.6);
 cursor:not-allowed;
 outline:none; }
 .bp3-file-upload-input::after:disabled.bp3-active, .bp3-file-upload-input::after:disabled.bp3-active:hover, .bp3-file-upload-input::after.bp3-disabled.bp3-active, .bp3-file-upload-input::after.bp3-disabled.bp3-active:hover{
 background:rgba(206, 217, 224, 0.7); }
 .bp3-file-upload-input:hover::after{
 background-clip:padding-box;
 background-color:#ebf1f5;
 -webkit-box-shadow:inset 0 0 0 1px rgba(16, 22, 26, 0.2), inset 0 -1px 0 rgba(16, 22, 26, 0.1);
 box-shadow:inset 0 0 0 1px rgba(16, 22, 26, 0.2), inset 0 -1px 0 rgba(16, 22, 26, 0.1); }
 .bp3-file-upload-input:active::after{
 background-color:#d8e1e8;
 background-image:none;
 -webkit-box-shadow:inset 0 0 0 1px rgba(16, 22, 26, 0.2), inset 0 1px 2px rgba(16, 22, 26, 0.2);
 box-shadow:inset 0 0 0 1px rgba(16, 22, 26, 0.2), inset 0 1px 2px rgba(16, 22, 26, 0.2); }
 .bp3-large .bp3-file-upload-input{
 font-size:16px;
 height:40px;
 line-height:40px;
 padding-right:95px; }
 .bp3-large .bp3-file-upload-input[type="search"], .bp3-large .bp3-file-upload-input.bp3-round{
 padding:0 15px; }
 .bp3-large .bp3-file-upload-input::after{
 min-height:30px;
 min-width:30px;
 line-height:30px;
 margin:5px;
 width:85px; }
 .bp3-dark .bp3-file-upload-input{
 background:rgba(16, 22, 26, 0.3);
 -webkit-box-shadow:0 0 0 0 rgba(19, 124, 189, 0), 0 0 0 0 rgba(19, 124, 189, 0), 0 0 0 0 rgba(19, 124, 189, 0), inset 0 0 0 1px rgba(16, 22, 26, 0.3), inset 0 1px 1px rgba(16, 22, 26, 0.4);
 box-shadow:0 0 0 0 rgba(19, 124, 189, 0), 0 0 0 0 rgba(19, 124, 189, 0), 0 0 0 0 rgba(19, 124, 189, 0), inset 0 0 0 1px rgba(16, 22, 26, 0.3), inset 0 1px 1px rgba(16, 22, 26, 0.4);
 color:#f5f8fa;
 color:rgba(167, 182, 194, 0.6); }
 .bp3-dark .bp3-file-upload-input::-webkit-input-placeholder{
 color:rgba(167, 182, 194, 0.6); }
 .bp3-dark .bp3-file-upload-input::-moz-placeholder{
 color:rgba(167, 182, 194, 0.6); }
 .bp3-dark .bp3-file-upload-input:-ms-input-placeholder{
 color:rgba(167, 182, 194, 0.6); }
 .bp3-dark .bp3-file-upload-input::-ms-input-placeholder{
 color:rgba(167, 182, 194, 0.6); }
 .bp3-dark .bp3-file-upload-input::placeholder{
 color:rgba(167, 182, 194, 0.6); }
 .bp3-dark .bp3-file-upload-input:focus{
 -webkit-box-shadow:0 0 0 1px #137cbd, 0 0 0 1px #137cbd, 0 0 0 3px rgba(19, 124, 189, 0.3), inset 0 0 0 1px rgba(16, 22, 26, 0.3), inset 0 1px 1px rgba(16, 22, 26, 0.4);
 box-shadow:0 0 0 1px #137cbd, 0 0 0 1px #137cbd, 0 0 0 3px rgba(19, 124, 189, 0.3), inset 0 0 0 1px rgba(16, 22, 26, 0.3), inset 0 1px 1px rgba(16, 22, 26, 0.4); }
 .bp3-dark .bp3-file-upload-input[readonly]{
 -webkit-box-shadow:inset 0 0 0 1px rgba(16, 22, 26, 0.4);
 box-shadow:inset 0 0 0 1px rgba(16, 22, 26, 0.4); }
 .bp3-dark .bp3-file-upload-input:disabled, .bp3-dark .bp3-file-upload-input.bp3-disabled{
 background:rgba(57, 75, 89, 0.5);
 -webkit-box-shadow:none;
 box-shadow:none;
 color:rgba(167, 182, 194, 0.6); }
 .bp3-dark .bp3-file-upload-input::after{
 background-color:#394b59;
 background-image:-webkit-gradient(linear, left top, left bottom, from(rgba(255, 255, 255, 0.05)), to(rgba(255, 255, 255, 0)));
 background-image:linear-gradient(to bottom, rgba(255, 255, 255, 0.05), rgba(255, 255, 255, 0));
 -webkit-box-shadow:0 0 0 1px rgba(16, 22, 26, 0.4);
 box-shadow:0 0 0 1px rgba(16, 22, 26, 0.4);
 color:#f5f8fa; }
 .bp3-dark .bp3-file-upload-input::after:hover, .bp3-dark .bp3-file-upload-input::after:active, .bp3-dark .bp3-file-upload-input::after.bp3-active{
 color:#f5f8fa; }
 .bp3-dark .bp3-file-upload-input::after:hover{
 background-color:#30404d;
 -webkit-box-shadow:0 0 0 1px rgba(16, 22, 26, 0.4);
 box-shadow:0 0 0 1px rgba(16, 22, 26, 0.4); }
 .bp3-dark .bp3-file-upload-input::after:active, .bp3-dark .bp3-file-upload-input::after.bp3-active{
 background-color:#202b33;
 background-image:none;
 -webkit-box-shadow:0 0 0 1px rgba(16, 22, 26, 0.6), inset 0 1px 2px rgba(16, 22, 26, 0.2);
 box-shadow:0 0 0 1px rgba(16, 22, 26, 0.6), inset 0 1px 2px rgba(16, 22, 26, 0.2); }
 .bp3-dark .bp3-file-upload-input::after:disabled, .bp3-dark .bp3-file-upload-input::after.bp3-disabled{
 background-color:rgba(57, 75, 89, 0.5);
 background-image:none;
 -webkit-box-shadow:none;
 box-shadow:none;
 color:rgba(167, 182, 194, 0.6); }
 .bp3-dark .bp3-file-upload-input::after:disabled.bp3-active, .bp3-dark .bp3-file-upload-input::after.bp3-disabled.bp3-active{
 background:rgba(57, 75, 89, 0.7); }
 .bp3-dark .bp3-file-upload-input::after .bp3-button-spinner .bp3-spinner-head{
 background:rgba(16, 22, 26, 0.5);
 stroke:#8a9ba8; }
 .bp3-dark .bp3-file-upload-input:hover::after{
 background-color:#30404d;
 -webkit-box-shadow:0 0 0 1px rgba(16, 22, 26, 0.4);
 box-shadow:0 0 0 1px rgba(16, 22, 26, 0.4); }
 .bp3-dark .bp3-file-upload-input:active::after{
 background-color:#202b33;
 background-image:none;
 -webkit-box-shadow:0 0 0 1px rgba(16, 22, 26, 0.6), inset 0 1px 2px rgba(16, 22, 26, 0.2);
 box-shadow:0 0 0 1px rgba(16, 22, 26, 0.6), inset 0 1px 2px rgba(16, 22, 26, 0.2); }
.bp3-file-upload-input::after{
 -webkit-box-shadow:inset 0 0 0 1px rgba(16, 22, 26, 0.2), inset 0 -1px 0 rgba(16, 22, 26, 0.1);
 box-shadow:inset 0 0 0 1px rgba(16, 22, 26, 0.2), inset 0 -1px 0 rgba(16, 22, 26, 0.1); }
.bp3-form-group{
 display:-webkit-box;
 display:-ms-flexbox;
 display:flex;
 -webkit-box-orient:vertical;
 -webkit-box-direction:normal;
 -ms-flex-direction:column;
 flex-direction:column;
 margin:0 0 15px; }
 .bp3-form-group label.bp3-label{
 margin-bottom:5px; }
 .bp3-form-group .bp3-control{
 margin-top:7px; }
 .bp3-form-group .bp3-form-helper-text{
 color:#5c7080;
 font-size:12px;
 margin-top:5px; }
 .bp3-form-group.bp3-intent-primary .bp3-form-helper-text{
 color:#106ba3; }
 .bp3-form-group.bp3-intent-success .bp3-form-helper-text{
 color:#0d8050; }
 .bp3-form-group.bp3-intent-warning .bp3-form-helper-text{
 color:#bf7326; }
 .bp3-form-group.bp3-intent-danger .bp3-form-helper-text{
 color:#c23030; }
 .bp3-form-group.bp3-inline{
 -webkit-box-align:start;
 -ms-flex-align:start;
 align-items:flex-start;
 -webkit-box-orient:horizontal;
 -webkit-box-direction:normal;
 -ms-flex-direction:row;
 flex-direction:row; }
 .bp3-form-group.bp3-inline.bp3-large label.bp3-label{
 line-height:40px;
 margin:0 10px 0 0; }
 .bp3-form-group.bp3-inline label.bp3-label{
 line-height:30px;
 margin:0 10px 0 0; }
 .bp3-form-group.bp3-disabled .bp3-label,
 .bp3-form-group.bp3-disabled .bp3-text-muted,
 .bp3-form-group.bp3-disabled .bp3-form-helper-text{
 color:rgba(92, 112, 128, 0.6) !important; }
 .bp3-dark .bp3-form-group.bp3-intent-primary .bp3-form-helper-text{
 color:#48aff0; }
 .bp3-dark .bp3-form-group.bp3-intent-success .bp3-form-helper-text{
 color:#3dcc91; }
 .bp3-dark .bp3-form-group.bp3-intent-warning .bp3-form-helper-text{
 color:#ffb366; }
 .bp3-dark .bp3-form-group.bp3-intent-danger .bp3-form-helper-text{
 color:#ff7373; }
 .bp3-dark .bp3-form-group .bp3-form-helper-text{
 color:#a7b6c2; }
 .bp3-dark .bp3-form-group.bp3-disabled .bp3-label,
 .bp3-dark .bp3-form-group.bp3-disabled .bp3-text-muted,
 .bp3-dark .bp3-form-group.bp3-disabled .bp3-form-helper-text{
 color:rgba(167, 182, 194, 0.6) !important; }
.bp3-input-group{
 display:block;
 position:relative; }
 .bp3-input-group .bp3-input{
 position:relative;
 width:100%; }
 .bp3-input-group .bp3-input:not(:first-child){
 padding-left:30px; }
 .bp3-input-group .bp3-input:not(:last-child){
 padding-right:30px; }
 .bp3-input-group .bp3-input-action,
 .bp3-input-group > .bp3-input-left-container,
 .bp3-input-group > .bp3-button,
 .bp3-input-group > .bp3-icon{
 position:absolute;
 top:0; }
 .bp3-input-group .bp3-input-action:first-child,
 .bp3-input-group > .bp3-input-left-container:first-child,
 .bp3-input-group > .bp3-button:first-child,
 .bp3-input-group > .bp3-icon:first-child{
 left:0; }
 .bp3-input-group .bp3-input-action:last-child,
 .bp3-input-group > .bp3-input-left-container:last-child,
 .bp3-input-group > .bp3-button:last-child,
 .bp3-input-group > .bp3-icon:last-child{
 right:0; }
 .bp3-input-group .bp3-button{
 min-height:24px;
 min-width:24px;
 margin:3px;
 padding:0 7px; }
 .bp3-input-group .bp3-button:empty{
 padding:0; }
 .bp3-input-group > .bp3-input-left-container,
 .bp3-input-group > .bp3-icon{
 z-index:1; }
 .bp3-input-group > .bp3-input-left-container > .bp3-icon,
 .bp3-input-group > .bp3-icon{
 color:#5c7080; }
 .bp3-input-group > .bp3-input-left-container > .bp3-icon:empty,
 .bp3-input-group > .bp3-icon:empty{
 font-family:"Icons16", sans-serif;
 font-size:16px;
 font-style:normal;
 font-weight:400;
 line-height:1;
 -moz-osx-font-smoothing:grayscale;
 -webkit-font-smoothing:antialiased; }
 .bp3-input-group > .bp3-input-left-container > .bp3-icon,
 .bp3-input-group > .bp3-icon,
 .bp3-input-group .bp3-input-action > .bp3-spinner{
 margin:7px; }
 .bp3-input-group .bp3-tag{
 margin:5px; }
 .bp3-input-group .bp3-input:not(:focus) + .bp3-button.bp3-minimal:not(:hover):not(:focus),
 .bp3-input-group .bp3-input:not(:focus) + .bp3-input-action .bp3-button.bp3-minimal:not(:hover):not(:focus){
 color:#5c7080; }
 .bp3-dark .bp3-input-group .bp3-input:not(:focus) + .bp3-button.bp3-minimal:not(:hover):not(:focus), .bp3-dark
 .bp3-input-group .bp3-input:not(:focus) + .bp3-input-action .bp3-button.bp3-minimal:not(:hover):not(:focus){
 color:#a7b6c2; }
 .bp3-input-group .bp3-input:not(:focus) + .bp3-button.bp3-minimal:not(:hover):not(:focus) .bp3-icon, .bp3-input-group .bp3-input:not(:focus) + .bp3-button.bp3-minimal:not(:hover):not(:focus) .bp3-icon-standard, .bp3-input-group .bp3-input:not(:focus) + .bp3-button.bp3-minimal:not(:hover):not(:focus) .bp3-icon-large,
 .bp3-input-group .bp3-input:not(:focus) + .bp3-input-action .bp3-button.bp3-minimal:not(:hover):not(:focus) .bp3-icon,
 .bp3-input-group .bp3-input:not(:focus) + .bp3-input-action .bp3-button.bp3-minimal:not(:hover):not(:focus) .bp3-icon-standard,
 .bp3-input-group .bp3-input:not(:focus) + .bp3-input-action .bp3-button.bp3-minimal:not(:hover):not(:focus) .bp3-icon-large{
 color:#5c7080; }
 .bp3-input-group .bp3-input:not(:focus) + .bp3-button.bp3-minimal:disabled,
 .bp3-input-group .bp3-input:not(:focus) + .bp3-input-action .bp3-button.bp3-minimal:disabled{
 color:rgba(92, 112, 128, 0.6) !important; }
 .bp3-input-group .bp3-input:not(:focus) + .bp3-button.bp3-minimal:disabled .bp3-icon, .bp3-input-group .bp3-input:not(:focus) + .bp3-button.bp3-minimal:disabled .bp3-icon-standard, .bp3-input-group .bp3-input:not(:focus) + .bp3-button.bp3-minimal:disabled .bp3-icon-large,
 .bp3-input-group .bp3-input:not(:focus) + .bp3-input-action .bp3-button.bp3-minimal:disabled .bp3-icon,
 .bp3-input-group .bp3-input:not(:focus) + .bp3-input-action .bp3-button.bp3-minimal:disabled .bp3-icon-standard,
 .bp3-input-group .bp3-input:not(:focus) + .bp3-input-action .bp3-button.bp3-minimal:disabled .bp3-icon-large{
 color:rgba(92, 112, 128, 0.6) !important; }
 .bp3-input-group.bp3-disabled{
 cursor:not-allowed; }
 .bp3-input-group.bp3-disabled .bp3-icon{
 color:rgba(92, 112, 128, 0.6); }
 .bp3-input-group.bp3-large .bp3-button{
 min-height:30px;
 min-width:30px;
 margin:5px; }
 .bp3-input-group.bp3-large > .bp3-input-left-container > .bp3-icon,
 .bp3-input-group.bp3-large > .bp3-icon,
 .bp3-input-group.bp3-large .bp3-input-action > .bp3-spinner{
 margin:12px; }
 .bp3-input-group.bp3-large .bp3-input{
 font-size:16px;
 height:40px;
 line-height:40px; }
 .bp3-input-group.bp3-large .bp3-input[type="search"], .bp3-input-group.bp3-large .bp3-input.bp3-round{
 padding:0 15px; }
 .bp3-input-group.bp3-large .bp3-input:not(:first-child){
 padding-left:40px; }
 .bp3-input-group.bp3-large .bp3-input:not(:last-child){
 padding-right:40px; }
 .bp3-input-group.bp3-small .bp3-button{
 min-height:20px;
 min-width:20px;
 margin:2px; }
 .bp3-input-group.bp3-small .bp3-tag{
 min-height:20px;
 min-width:20px;
 margin:2px; }
 .bp3-input-group.bp3-small > .bp3-input-left-container > .bp3-icon,
 .bp3-input-group.bp3-small > .bp3-icon,
 .bp3-input-group.bp3-small .bp3-input-action > .bp3-spinner{
 margin:4px; }
 .bp3-input-group.bp3-small .bp3-input{
 font-size:12px;
 height:24px;
 line-height:24px;
 padding-left:8px;
 padding-right:8px; }
 .bp3-input-group.bp3-small .bp3-input[type="search"], .bp3-input-group.bp3-small .bp3-input.bp3-round{
 padding:0 12px; }
 .bp3-input-group.bp3-small .bp3-input:not(:first-child){
 padding-left:24px; }
 .bp3-input-group.bp3-small .bp3-input:not(:last-child){
 padding-right:24px; }
 .bp3-input-group.bp3-fill{
 -webkit-box-flex:1;
 -ms-flex:1 1 auto;
 flex:1 1 auto;
 width:100%; }
 .bp3-input-group.bp3-round .bp3-button,
 .bp3-input-group.bp3-round .bp3-input,
 .bp3-input-group.bp3-round .bp3-tag{
 border-radius:30px; }
 .bp3-dark .bp3-input-group .bp3-icon{
 color:#a7b6c2; }
 .bp3-dark .bp3-input-group.bp3-disabled .bp3-icon{
 color:rgba(167, 182, 194, 0.6); }
 .bp3-input-group.bp3-intent-primary .bp3-input{
 -webkit-box-shadow:0 0 0 0 rgba(19, 124, 189, 0), 0 0 0 0 rgba(19, 124, 189, 0), inset 0 0 0 1px #137cbd, inset 0 0 0 1px rgba(16, 22, 26, 0.15), inset 0 1px 1px rgba(16, 22, 26, 0.2);
 box-shadow:0 0 0 0 rgba(19, 124, 189, 0), 0 0 0 0 rgba(19, 124, 189, 0), inset 0 0 0 1px #137cbd, inset 0 0 0 1px rgba(16, 22, 26, 0.15), inset 0 1px 1px rgba(16, 22, 26, 0.2); }
 .bp3-input-group.bp3-intent-primary .bp3-input:focus{
 -webkit-box-shadow:0 0 0 1px #137cbd, 0 0 0 3px rgba(19, 124, 189, 0.3), inset 0 1px 1px rgba(16, 22, 26, 0.2);
 box-shadow:0 0 0 1px #137cbd, 0 0 0 3px rgba(19, 124, 189, 0.3), inset 0 1px 1px rgba(16, 22, 26, 0.2); }
 .bp3-input-group.bp3-intent-primary .bp3-input[readonly]{
 -webkit-box-shadow:inset 0 0 0 1px #137cbd;
 box-shadow:inset 0 0 0 1px #137cbd; }
 .bp3-input-group.bp3-intent-primary .bp3-input:disabled, .bp3-input-group.bp3-intent-primary .bp3-input.bp3-disabled{
 -webkit-box-shadow:none;
 box-shadow:none; }
 .bp3-input-group.bp3-intent-primary > .bp3-icon{
 color:#106ba3; }
 .bp3-dark .bp3-input-group.bp3-intent-primary > .bp3-icon{
 color:#48aff0; }
 .bp3-input-group.bp3-intent-success .bp3-input{
 -webkit-box-shadow:0 0 0 0 rgba(15, 153, 96, 0), 0 0 0 0 rgba(15, 153, 96, 0), inset 0 0 0 1px #0f9960, inset 0 0 0 1px rgba(16, 22, 26, 0.15), inset 0 1px 1px rgba(16, 22, 26, 0.2);
 box-shadow:0 0 0 0 rgba(15, 153, 96, 0), 0 0 0 0 rgba(15, 153, 96, 0), inset 0 0 0 1px #0f9960, inset 0 0 0 1px rgba(16, 22, 26, 0.15), inset 0 1px 1px rgba(16, 22, 26, 0.2); }
 .bp3-input-group.bp3-intent-success .bp3-input:focus{
 -webkit-box-shadow:0 0 0 1px #0f9960, 0 0 0 3px rgba(15, 153, 96, 0.3), inset 0 1px 1px rgba(16, 22, 26, 0.2);
 box-shadow:0 0 0 1px #0f9960, 0 0 0 3px rgba(15, 153, 96, 0.3), inset 0 1px 1px rgba(16, 22, 26, 0.2); }
 .bp3-input-group.bp3-intent-success .bp3-input[readonly]{
 -webkit-box-shadow:inset 0 0 0 1px #0f9960;
 box-shadow:inset 0 0 0 1px #0f9960; }
 .bp3-input-group.bp3-intent-success .bp3-input:disabled, .bp3-input-group.bp3-intent-success .bp3-input.bp3-disabled{
 -webkit-box-shadow:none;
 box-shadow:none; }
 .bp3-input-group.bp3-intent-success > .bp3-icon{
 color:#0d8050; }
 .bp3-dark .bp3-input-group.bp3-intent-success > .bp3-icon{
 color:#3dcc91; }
 .bp3-input-group.bp3-intent-warning .bp3-input{
 -webkit-box-shadow:0 0 0 0 rgba(217, 130, 43, 0), 0 0 0 0 rgba(217, 130, 43, 0), inset 0 0 0 1px #d9822b, inset 0 0 0 1px rgba(16, 22, 26, 0.15), inset 0 1px 1px rgba(16, 22, 26, 0.2);
 box-shadow:0 0 0 0 rgba(217, 130, 43, 0), 0 0 0 0 rgba(217, 130, 43, 0), inset 0 0 0 1px #d9822b, inset 0 0 0 1px rgba(16, 22, 26, 0.15), inset 0 1px 1px rgba(16, 22, 26, 0.2); }
 .bp3-input-group.bp3-intent-warning .bp3-input:focus{
 -webkit-box-shadow:0 0 0 1px #d9822b, 0 0 0 3px rgba(217, 130, 43, 0.3), inset 0 1px 1px rgba(16, 22, 26, 0.2);
 box-shadow:0 0 0 1px #d9822b, 0 0 0 3px rgba(217, 130, 43, 0.3), inset 0 1px 1px rgba(16, 22, 26, 0.2); }
 .bp3-input-group.bp3-intent-warning .bp3-input[readonly]{
 -webkit-box-shadow:inset 0 0 0 1px #d9822b;
 box-shadow:inset 0 0 0 1px #d9822b; }
 .bp3-input-group.bp3-intent-warning .bp3-input:disabled, .bp3-input-group.bp3-intent-warning .bp3-input.bp3-disabled{
 -webkit-box-shadow:none;
 box-shadow:none; }
 .bp3-input-group.bp3-intent-warning > .bp3-icon{
 color:#bf7326; }
 .bp3-dark .bp3-input-group.bp3-intent-warning > .bp3-icon{
 color:#ffb366; }
 .bp3-input-group.bp3-intent-danger .bp3-input{
 -webkit-box-shadow:0 0 0 0 rgba(219, 55, 55, 0), 0 0 0 0 rgba(219, 55, 55, 0), inset 0 0 0 1px #db3737, inset 0 0 0 1px rgba(16, 22, 26, 0.15), inset 0 1px 1px rgba(16, 22, 26, 0.2);
 box-shadow:0 0 0 0 rgba(219, 55, 55, 0), 0 0 0 0 rgba(219, 55, 55, 0), inset 0 0 0 1px #db3737, inset 0 0 0 1px rgba(16, 22, 26, 0.15), inset 0 1px 1px rgba(16, 22, 26, 0.2); }
 .bp3-input-group.bp3-intent-danger .bp3-input:focus{
 -webkit-box-shadow:0 0 0 1px #db3737, 0 0 0 3px rgba(219, 55, 55, 0.3), inset 0 1px 1px rgba(16, 22, 26, 0.2);
 box-shadow:0 0 0 1px #db3737, 0 0 0 3px rgba(219, 55, 55, 0.3), inset 0 1px 1px rgba(16, 22, 26, 0.2); }
 .bp3-input-group.bp3-intent-danger .bp3-input[readonly]{
 -webkit-box-shadow:inset 0 0 0 1px #db3737;
 box-shadow:inset 0 0 0 1px #db3737; }
 .bp3-input-group.bp3-intent-danger .bp3-input:disabled, .bp3-input-group.bp3-intent-danger .bp3-input.bp3-disabled{
 -webkit-box-shadow:none;
 box-shadow:none; }
 .bp3-input-group.bp3-intent-danger > .bp3-icon{
 color:#c23030; }
 .bp3-dark .bp3-input-group.bp3-intent-danger > .bp3-icon{
 color:#ff7373; }
.bp3-input{
 -webkit-appearance:none;
 -moz-appearance:none;
 appearance:none;
 background:#ffffff;
 border:none;
 border-radius:3px;
 -webkit-box-shadow:0 0 0 0 rgba(19, 124, 189, 0), 0 0 0 0 rgba(19, 124, 189, 0), inset 0 0 0 1px rgba(16, 22, 26, 0.15), inset 0 1px 1px rgba(16, 22, 26, 0.2);
 box-shadow:0 0 0 0 rgba(19, 124, 189, 0), 0 0 0 0 rgba(19, 124, 189, 0), inset 0 0 0 1px rgba(16, 22, 26, 0.15), inset 0 1px 1px rgba(16, 22, 26, 0.2);
 color:#182026;
 font-size:14px;
 font-weight:400;
 height:30px;
 line-height:30px;
 outline:none;
 padding:0 10px;
 -webkit-transition:-webkit-box-shadow 100ms cubic-bezier(0.4, 1, 0.75, 0.9);
 transition:-webkit-box-shadow 100ms cubic-bezier(0.4, 1, 0.75, 0.9);
 transition:box-shadow 100ms cubic-bezier(0.4, 1, 0.75, 0.9);
 transition:box-shadow 100ms cubic-bezier(0.4, 1, 0.75, 0.9), -webkit-box-shadow 100ms cubic-bezier(0.4, 1, 0.75, 0.9);
 vertical-align:middle; }
 .bp3-input::-webkit-input-placeholder{
 color:rgba(92, 112, 128, 0.6);
 opacity:1; }
 .bp3-input::-moz-placeholder{
 color:rgba(92, 112, 128, 0.6);
 opacity:1; }
 .bp3-input:-ms-input-placeholder{
 color:rgba(92, 112, 128, 0.6);
 opacity:1; }
 .bp3-input::-ms-input-placeholder{
 color:rgba(92, 112, 128, 0.6);
 opacity:1; }
 .bp3-input::placeholder{
 color:rgba(92, 112, 128, 0.6);
 opacity:1; }
 .bp3-input:focus, .bp3-input.bp3-active{
 -webkit-box-shadow:0 0 0 1px #137cbd, 0 0 0 3px rgba(19, 124, 189, 0.3), inset 0 1px 1px rgba(16, 22, 26, 0.2);
 box-shadow:0 0 0 1px #137cbd, 0 0 0 3px rgba(19, 124, 189, 0.3), inset 0 1px 1px rgba(16, 22, 26, 0.2); }
 .bp3-input[type="search"], .bp3-input.bp3-round{
 border-radius:30px;
 -webkit-box-sizing:border-box;
 box-sizing:border-box;
 padding-left:10px; }
 .bp3-input[readonly]{
 -webkit-box-shadow:inset 0 0 0 1px rgba(16, 22, 26, 0.15);
 box-shadow:inset 0 0 0 1px rgba(16, 22, 26, 0.15); }
 .bp3-input:disabled, .bp3-input.bp3-disabled{
 background:rgba(206, 217, 224, 0.5);
 -webkit-box-shadow:none;
 box-shadow:none;
 color:rgba(92, 112, 128, 0.6);
 cursor:not-allowed;
 resize:none; }
 .bp3-input.bp3-large{
 font-size:16px;
 height:40px;
 line-height:40px; }
 .bp3-input.bp3-large[type="search"], .bp3-input.bp3-large.bp3-round{
 padding:0 15px; }
 .bp3-input.bp3-small{
 font-size:12px;
 height:24px;
 line-height:24px;
 padding-left:8px;
 padding-right:8px; }
 .bp3-input.bp3-small[type="search"], .bp3-input.bp3-small.bp3-round{
 padding:0 12px; }
 .bp3-input.bp3-fill{
 -webkit-box-flex:1;
 -ms-flex:1 1 auto;
 flex:1 1 auto;
 width:100%; }
 .bp3-dark .bp3-input{
 background:rgba(16, 22, 26, 0.3);
 -webkit-box-shadow:0 0 0 0 rgba(19, 124, 189, 0), 0 0 0 0 rgba(19, 124, 189, 0), 0 0 0 0 rgba(19, 124, 189, 0), inset 0 0 0 1px rgba(16, 22, 26, 0.3), inset 0 1px 1px rgba(16, 22, 26, 0.4);
 box-shadow:0 0 0 0 rgba(19, 124, 189, 0), 0 0 0 0 rgba(19, 124, 189, 0), 0 0 0 0 rgba(19, 124, 189, 0), inset 0 0 0 1px rgba(16, 22, 26, 0.3), inset 0 1px 1px rgba(16, 22, 26, 0.4);
 color:#f5f8fa; }
 .bp3-dark .bp3-input::-webkit-input-placeholder{
 color:rgba(167, 182, 194, 0.6); }
 .bp3-dark .bp3-input::-moz-placeholder{
 color:rgba(167, 182, 194, 0.6); }
 .bp3-dark .bp3-input:-ms-input-placeholder{
 color:rgba(167, 182, 194, 0.6); }
 .bp3-dark .bp3-input::-ms-input-placeholder{
 color:rgba(167, 182, 194, 0.6); }
 .bp3-dark .bp3-input::placeholder{
 color:rgba(167, 182, 194, 0.6); }
 .bp3-dark .bp3-input:focus{
 -webkit-box-shadow:0 0 0 1px #137cbd, 0 0 0 1px #137cbd, 0 0 0 3px rgba(19, 124, 189, 0.3), inset 0 0 0 1px rgba(16, 22, 26, 0.3), inset 0 1px 1px rgba(16, 22, 26, 0.4);
 box-shadow:0 0 0 1px #137cbd, 0 0 0 1px #137cbd, 0 0 0 3px rgba(19, 124, 189, 0.3), inset 0 0 0 1px rgba(16, 22, 26, 0.3), inset 0 1px 1px rgba(16, 22, 26, 0.4); }
 .bp3-dark .bp3-input[readonly]{
 -webkit-box-shadow:inset 0 0 0 1px rgba(16, 22, 26, 0.4);
 box-shadow:inset 0 0 0 1px rgba(16, 22, 26, 0.4); }
 .bp3-dark .bp3-input:disabled, .bp3-dark .bp3-input.bp3-disabled{
 background:rgba(57, 75, 89, 0.5);
 -webkit-box-shadow:none;
 box-shadow:none;
 color:rgba(167, 182, 194, 0.6); }
 .bp3-input.bp3-intent-primary{
 -webkit-box-shadow:0 0 0 0 rgba(19, 124, 189, 0), 0 0 0 0 rgba(19, 124, 189, 0), inset 0 0 0 1px #137cbd, inset 0 0 0 1px rgba(16, 22, 26, 0.15), inset 0 1px 1px rgba(16, 22, 26, 0.2);
 box-shadow:0 0 0 0 rgba(19, 124, 189, 0), 0 0 0 0 rgba(19, 124, 189, 0), inset 0 0 0 1px #137cbd, inset 0 0 0 1px rgba(16, 22, 26, 0.15), inset 0 1px 1px rgba(16, 22, 26, 0.2); }
 .bp3-input.bp3-intent-primary:focus{
 -webkit-box-shadow:0 0 0 1px #137cbd, 0 0 0 3px rgba(19, 124, 189, 0.3), inset 0 1px 1px rgba(16, 22, 26, 0.2);
 box-shadow:0 0 0 1px #137cbd, 0 0 0 3px rgba(19, 124, 189, 0.3), inset 0 1px 1px rgba(16, 22, 26, 0.2); }
 .bp3-input.bp3-intent-primary[readonly]{
 -webkit-box-shadow:inset 0 0 0 1px #137cbd;
 box-shadow:inset 0 0 0 1px #137cbd; }
 .bp3-input.bp3-intent-primary:disabled, .bp3-input.bp3-intent-primary.bp3-disabled{
 -webkit-box-shadow:none;
 box-shadow:none; }
 .bp3-dark .bp3-input.bp3-intent-primary{
 -webkit-box-shadow:0 0 0 0 rgba(19, 124, 189, 0), 0 0 0 0 rgba(19, 124, 189, 0), 0 0 0 0 rgba(19, 124, 189, 0), inset 0 0 0 1px #137cbd, inset 0 0 0 1px rgba(16, 22, 26, 0.3), inset 0 1px 1px rgba(16, 22, 26, 0.4);
 box-shadow:0 0 0 0 rgba(19, 124, 189, 0), 0 0 0 0 rgba(19, 124, 189, 0), 0 0 0 0 rgba(19, 124, 189, 0), inset 0 0 0 1px #137cbd, inset 0 0 0 1px rgba(16, 22, 26, 0.3), inset 0 1px 1px rgba(16, 22, 26, 0.4); }
 .bp3-dark .bp3-input.bp3-intent-primary:focus{
 -webkit-box-shadow:0 0 0 1px #137cbd, 0 0 0 1px #137cbd, 0 0 0 3px rgba(19, 124, 189, 0.3), inset 0 0 0 1px rgba(16, 22, 26, 0.3), inset 0 1px 1px rgba(16, 22, 26, 0.4);
 box-shadow:0 0 0 1px #137cbd, 0 0 0 1px #137cbd, 0 0 0 3px rgba(19, 124, 189, 0.3), inset 0 0 0 1px rgba(16, 22, 26, 0.3), inset 0 1px 1px rgba(16, 22, 26, 0.4); }
 .bp3-dark .bp3-input.bp3-intent-primary[readonly]{
 -webkit-box-shadow:inset 0 0 0 1px #137cbd;
 box-shadow:inset 0 0 0 1px #137cbd; }
 .bp3-dark .bp3-input.bp3-intent-primary:disabled, .bp3-dark .bp3-input.bp3-intent-primary.bp3-disabled{
 -webkit-box-shadow:none;
 box-shadow:none; }
 .bp3-input.bp3-intent-success{
 -webkit-box-shadow:0 0 0 0 rgba(15, 153, 96, 0), 0 0 0 0 rgba(15, 153, 96, 0), inset 0 0 0 1px #0f9960, inset 0 0 0 1px rgba(16, 22, 26, 0.15), inset 0 1px 1px rgba(16, 22, 26, 0.2);
 box-shadow:0 0 0 0 rgba(15, 153, 96, 0), 0 0 0 0 rgba(15, 153, 96, 0), inset 0 0 0 1px #0f9960, inset 0 0 0 1px rgba(16, 22, 26, 0.15), inset 0 1px 1px rgba(16, 22, 26, 0.2); }
 .bp3-input.bp3-intent-success:focus{
 -webkit-box-shadow:0 0 0 1px #0f9960, 0 0 0 3px rgba(15, 153, 96, 0.3), inset 0 1px 1px rgba(16, 22, 26, 0.2);
 box-shadow:0 0 0 1px #0f9960, 0 0 0 3px rgba(15, 153, 96, 0.3), inset 0 1px 1px rgba(16, 22, 26, 0.2); }
 .bp3-input.bp3-intent-success[readonly]{
 -webkit-box-shadow:inset 0 0 0 1px #0f9960;
 box-shadow:inset 0 0 0 1px #0f9960; }
 .bp3-input.bp3-intent-success:disabled, .bp3-input.bp3-intent-success.bp3-disabled{
 -webkit-box-shadow:none;
 box-shadow:none; }
 .bp3-dark .bp3-input.bp3-intent-success{
 -webkit-box-shadow:0 0 0 0 rgba(15, 153, 96, 0), 0 0 0 0 rgba(15, 153, 96, 0), 0 0 0 0 rgba(15, 153, 96, 0), inset 0 0 0 1px #0f9960, inset 0 0 0 1px rgba(16, 22, 26, 0.3), inset 0 1px 1px rgba(16, 22, 26, 0.4);
 box-shadow:0 0 0 0 rgba(15, 153, 96, 0), 0 0 0 0 rgba(15, 153, 96, 0), 0 0 0 0 rgba(15, 153, 96, 0), inset 0 0 0 1px #0f9960, inset 0 0 0 1px rgba(16, 22, 26, 0.3), inset 0 1px 1px rgba(16, 22, 26, 0.4); }
 .bp3-dark .bp3-input.bp3-intent-success:focus{
 -webkit-box-shadow:0 0 0 1px #0f9960, 0 0 0 1px #0f9960, 0 0 0 3px rgba(15, 153, 96, 0.3), inset 0 0 0 1px rgba(16, 22, 26, 0.3), inset 0 1px 1px rgba(16, 22, 26, 0.4);
 box-shadow:0 0 0 1px #0f9960, 0 0 0 1px #0f9960, 0 0 0 3px rgba(15, 153, 96, 0.3), inset 0 0 0 1px rgba(16, 22, 26, 0.3), inset 0 1px 1px rgba(16, 22, 26, 0.4); }
 .bp3-dark .bp3-input.bp3-intent-success[readonly]{
 -webkit-box-shadow:inset 0 0 0 1px #0f9960;
 box-shadow:inset 0 0 0 1px #0f9960; }
 .bp3-dark .bp3-input.bp3-intent-success:disabled, .bp3-dark .bp3-input.bp3-intent-success.bp3-disabled{
 -webkit-box-shadow:none;
 box-shadow:none; }
 .bp3-input.bp3-intent-warning{
 -webkit-box-shadow:0 0 0 0 rgba(217, 130, 43, 0), 0 0 0 0 rgba(217, 130, 43, 0), inset 0 0 0 1px #d9822b, inset 0 0 0 1px rgba(16, 22, 26, 0.15), inset 0 1px 1px rgba(16, 22, 26, 0.2);
 box-shadow:0 0 0 0 rgba(217, 130, 43, 0), 0 0 0 0 rgba(217, 130, 43, 0), inset 0 0 0 1px #d9822b, inset 0 0 0 1px rgba(16, 22, 26, 0.15), inset 0 1px 1px rgba(16, 22, 26, 0.2); }
 .bp3-input.bp3-intent-warning:focus{
 -webkit-box-shadow:0 0 0 1px #d9822b, 0 0 0 3px rgba(217, 130, 43, 0.3), inset 0 1px 1px rgba(16, 22, 26, 0.2);
 box-shadow:0 0 0 1px #d9822b, 0 0 0 3px rgba(217, 130, 43, 0.3), inset 0 1px 1px rgba(16, 22, 26, 0.2); }
 .bp3-input.bp3-intent-warning[readonly]{
 -webkit-box-shadow:inset 0 0 0 1px #d9822b;
 box-shadow:inset 0 0 0 1px #d9822b; }
 .bp3-input.bp3-intent-warning:disabled, .bp3-input.bp3-intent-warning.bp3-disabled{
 -webkit-box-shadow:none;
 box-shadow:none; }
 .bp3-dark .bp3-input.bp3-intent-warning{
 -webkit-box-shadow:0 0 0 0 rgba(217, 130, 43, 0), 0 0 0 0 rgba(217, 130, 43, 0), 0 0 0 0 rgba(217, 130, 43, 0), inset 0 0 0 1px #d9822b, inset 0 0 0 1px rgba(16, 22, 26, 0.3), inset 0 1px 1px rgba(16, 22, 26, 0.4);
 box-shadow:0 0 0 0 rgba(217, 130, 43, 0), 0 0 0 0 rgba(217, 130, 43, 0), 0 0 0 0 rgba(217, 130, 43, 0), inset 0 0 0 1px #d9822b, inset 0 0 0 1px rgba(16, 22, 26, 0.3), inset 0 1px 1px rgba(16, 22, 26, 0.4); }
 .bp3-dark .bp3-input.bp3-intent-warning:focus{
 -webkit-box-shadow:0 0 0 1px #d9822b, 0 0 0 1px #d9822b, 0 0 0 3px rgba(217, 130, 43, 0.3), inset 0 0 0 1px rgba(16, 22, 26, 0.3), inset 0 1px 1px rgba(16, 22, 26, 0.4);
 box-shadow:0 0 0 1px #d9822b, 0 0 0 1px #d9822b, 0 0 0 3px rgba(217, 130, 43, 0.3), inset 0 0 0 1px rgba(16, 22, 26, 0.3), inset 0 1px 1px rgba(16, 22, 26, 0.4); }
 .bp3-dark .bp3-input.bp3-intent-warning[readonly]{
 -webkit-box-shadow:inset 0 0 0 1px #d9822b;
 box-shadow:inset 0 0 0 1px #d9822b; }
 .bp3-dark .bp3-input.bp3-intent-warning:disabled, .bp3-dark .bp3-input.bp3-intent-warning.bp3-disabled{
 -webkit-box-shadow:none;
 box-shadow:none; }
 .bp3-input.bp3-intent-danger{
 -webkit-box-shadow:0 0 0 0 rgba(219, 55, 55, 0), 0 0 0 0 rgba(219, 55, 55, 0), inset 0 0 0 1px #db3737, inset 0 0 0 1px rgba(16, 22, 26, 0.15), inset 0 1px 1px rgba(16, 22, 26, 0.2);
 box-shadow:0 0 0 0 rgba(219, 55, 55, 0), 0 0 0 0 rgba(219, 55, 55, 0), inset 0 0 0 1px #db3737, inset 0 0 0 1px rgba(16, 22, 26, 0.15), inset 0 1px 1px rgba(16, 22, 26, 0.2); }
 .bp3-input.bp3-intent-danger:focus{
 -webkit-box-shadow:0 0 0 1px #db3737, 0 0 0 3px rgba(219, 55, 55, 0.3), inset 0 1px 1px rgba(16, 22, 26, 0.2);
 box-shadow:0 0 0 1px #db3737, 0 0 0 3px rgba(219, 55, 55, 0.3), inset 0 1px 1px rgba(16, 22, 26, 0.2); }
 .bp3-input.bp3-intent-danger[readonly]{
 -webkit-box-shadow:inset 0 0 0 1px #db3737;
 box-shadow:inset 0 0 0 1px #db3737; }
 .bp3-input.bp3-intent-danger:disabled, .bp3-input.bp3-intent-danger.bp3-disabled{
 -webkit-box-shadow:none;
 box-shadow:none; }
 .bp3-dark .bp3-input.bp3-intent-danger{
 -webkit-box-shadow:0 0 0 0 rgba(219, 55, 55, 0), 0 0 0 0 rgba(219, 55, 55, 0), 0 0 0 0 rgba(219, 55, 55, 0), inset 0 0 0 1px #db3737, inset 0 0 0 1px rgba(16, 22, 26, 0.3), inset 0 1px 1px rgba(16, 22, 26, 0.4);
 box-shadow:0 0 0 0 rgba(219, 55, 55, 0), 0 0 0 0 rgba(219, 55, 55, 0), 0 0 0 0 rgba(219, 55, 55, 0), inset 0 0 0 1px #db3737, inset 0 0 0 1px rgba(16, 22, 26, 0.3), inset 0 1px 1px rgba(16, 22, 26, 0.4); }
 .bp3-dark .bp3-input.bp3-intent-danger:focus{
 -webkit-box-shadow:0 0 0 1px #db3737, 0 0 0 1px #db3737, 0 0 0 3px rgba(219, 55, 55, 0.3), inset 0 0 0 1px rgba(16, 22, 26, 0.3), inset 0 1px 1px rgba(16, 22, 26, 0.4);
 box-shadow:0 0 0 1px #db3737, 0 0 0 1px #db3737, 0 0 0 3px rgba(219, 55, 55, 0.3), inset 0 0 0 1px rgba(16, 22, 26, 0.3), inset 0 1px 1px rgba(16, 22, 26, 0.4); }
 .bp3-dark .bp3-input.bp3-intent-danger[readonly]{
 -webkit-box-shadow:inset 0 0 0 1px #db3737;
 box-shadow:inset 0 0 0 1px #db3737; }
 .bp3-dark .bp3-input.bp3-intent-danger:disabled, .bp3-dark .bp3-input.bp3-intent-danger.bp3-disabled{
 -webkit-box-shadow:none;
 box-shadow:none; }
 .bp3-input::-ms-clear{
 display:none; }
textarea.bp3-input{
 max-width:100%;
 padding:10px; }
 textarea.bp3-input, textarea.bp3-input.bp3-large, textarea.bp3-input.bp3-small{
 height:auto;
 line-height:inherit; }
 textarea.bp3-input.bp3-small{
 padding:8px; }
 .bp3-dark textarea.bp3-input{
 background:rgba(16, 22, 26, 0.3);
 -webkit-box-shadow:0 0 0 0 rgba(19, 124, 189, 0), 0 0 0 0 rgba(19, 124, 189, 0), 0 0 0 0 rgba(19, 124, 189, 0), inset 0 0 0 1px rgba(16, 22, 26, 0.3), inset 0 1px 1px rgba(16, 22, 26, 0.4);
 box-shadow:0 0 0 0 rgba(19, 124, 189, 0), 0 0 0 0 rgba(19, 124, 189, 0), 0 0 0 0 rgba(19, 124, 189, 0), inset 0 0 0 1px rgba(16, 22, 26, 0.3), inset 0 1px 1px rgba(16, 22, 26, 0.4);
 color:#f5f8fa; }
 .bp3-dark textarea.bp3-input::-webkit-input-placeholder{
 color:rgba(167, 182, 194, 0.6); }
 .bp3-dark textarea.bp3-input::-moz-placeholder{
 color:rgba(167, 182, 194, 0.6); }
 .bp3-dark textarea.bp3-input:-ms-input-placeholder{
 color:rgba(167, 182, 194, 0.6); }
 .bp3-dark textarea.bp3-input::-ms-input-placeholder{
 color:rgba(167, 182, 194, 0.6); }
 .bp3-dark textarea.bp3-input::placeholder{
 color:rgba(167, 182, 194, 0.6); }
 .bp3-dark textarea.bp3-input:focus{
 -webkit-box-shadow:0 0 0 1px #137cbd, 0 0 0 1px #137cbd, 0 0 0 3px rgba(19, 124, 189, 0.3), inset 0 0 0 1px rgba(16, 22, 26, 0.3), inset 0 1px 1px rgba(16, 22, 26, 0.4);
 box-shadow:0 0 0 1px #137cbd, 0 0 0 1px #137cbd, 0 0 0 3px rgba(19, 124, 189, 0.3), inset 0 0 0 1px rgba(16, 22, 26, 0.3), inset 0 1px 1px rgba(16, 22, 26, 0.4); }
 .bp3-dark textarea.bp3-input[readonly]{
 -webkit-box-shadow:inset 0 0 0 1px rgba(16, 22, 26, 0.4);
 box-shadow:inset 0 0 0 1px rgba(16, 22, 26, 0.4); }
 .bp3-dark textarea.bp3-input:disabled, .bp3-dark textarea.bp3-input.bp3-disabled{
 background:rgba(57, 75, 89, 0.5);
 -webkit-box-shadow:none;
 box-shadow:none;
 color:rgba(167, 182, 194, 0.6); }
label.bp3-label{
 display:block;
 margin-bottom:15px;
 margin-top:0; }
 label.bp3-label .bp3-html-select,
 label.bp3-label .bp3-input,
 label.bp3-label .bp3-select,
 label.bp3-label .bp3-slider,
 label.bp3-label .bp3-popover-wrapper{
 display:block;
 margin-top:5px;
 text-transform:none; }
 label.bp3-label .bp3-button-group{
 margin-top:5px; }
 label.bp3-label .bp3-select select,
 label.bp3-label .bp3-html-select select{
 font-weight:400;
 vertical-align:top;
 width:100%; }
 label.bp3-label.bp3-disabled,
 label.bp3-label.bp3-disabled .bp3-text-muted{
 color:rgba(92, 112, 128, 0.6); }
 label.bp3-label.bp3-inline{
 line-height:30px; }
 label.bp3-label.bp3-inline .bp3-html-select,
 label.bp3-label.bp3-inline .bp3-input,
 label.bp3-label.bp3-inline .bp3-input-group,
 label.bp3-label.bp3-inline .bp3-select,
 label.bp3-label.bp3-inline .bp3-popover-wrapper{
 display:inline-block;
 margin:0 0 0 5px;
 vertical-align:top; }
 label.bp3-label.bp3-inline .bp3-button-group{
 margin:0 0 0 5px; }
 label.bp3-label.bp3-inline .bp3-input-group .bp3-input{
 margin-left:0; }
 label.bp3-label.bp3-inline.bp3-large{
 line-height:40px; }
 label.bp3-label:not(.bp3-inline) .bp3-popover-target{
 display:block; }
 .bp3-dark label.bp3-label{
 color:#f5f8fa; }
 .bp3-dark label.bp3-label.bp3-disabled,
 .bp3-dark label.bp3-label.bp3-disabled .bp3-text-muted{
 color:rgba(167, 182, 194, 0.6); }
.bp3-numeric-input .bp3-button-group.bp3-vertical > .bp3-button{
 -webkit-box-flex:1;
 -ms-flex:1 1 14px;
 flex:1 1 14px;
 min-height:0;
 padding:0;
 width:30px; }
 .bp3-numeric-input .bp3-button-group.bp3-vertical > .bp3-button:first-child{
 border-radius:0 3px 0 0; }
 .bp3-numeric-input .bp3-button-group.bp3-vertical > .bp3-button:last-child{
 border-radius:0 0 3px 0; }

.bp3-numeric-input .bp3-button-group.bp3-vertical:first-child > .bp3-button:first-child{
 border-radius:3px 0 0 0; }

.bp3-numeric-input .bp3-button-group.bp3-vertical:first-child > .bp3-button:last-child{
 border-radius:0 0 0 3px; }

.bp3-numeric-input.bp3-large .bp3-button-group.bp3-vertical > .bp3-button{
 width:40px; }

form{
 display:block; }
.bp3-html-select select,
.bp3-select select{
 display:-webkit-inline-box;
 display:-ms-inline-flexbox;
 display:inline-flex;
 -webkit-box-orient:horizontal;
 -webkit-box-direction:normal;
 -ms-flex-direction:row;
 flex-direction:row;
 -webkit-box-align:center;
 -ms-flex-align:center;
 align-items:center;
 border:none;
 border-radius:3px;
 cursor:pointer;
 font-size:14px;
 -webkit-box-pack:center;
 -ms-flex-pack:center;
 justify-content:center;
 padding:5px 10px;
 text-align:left;
 vertical-align:middle;
 background-color:#f5f8fa;
 background-image:-webkit-gradient(linear, left top, left bottom, from(rgba(255, 255, 255, 0.8)), to(rgba(255, 255, 255, 0)));
 background-image:linear-gradient(to bottom, rgba(255, 255, 255, 0.8), rgba(255, 255, 255, 0));
 -webkit-box-shadow:inset 0 0 0 1px rgba(16, 22, 26, 0.2), inset 0 -1px 0 rgba(16, 22, 26, 0.1);
 box-shadow:inset 0 0 0 1px rgba(16, 22, 26, 0.2), inset 0 -1px 0 rgba(16, 22, 26, 0.1);
 color:#182026;
 -moz-appearance:none;
 -webkit-appearance:none;
 border-radius:3px;
 height:30px;
 padding:0 25px 0 10px;
 width:100%; }
 .bp3-html-select select > \*, .bp3-select select > \*{
 -webkit-box-flex:0;
 -ms-flex-positive:0;
 flex-grow:0;
 -ms-flex-negative:0;
 flex-shrink:0; }
 .bp3-html-select select > .bp3-fill, .bp3-select select > .bp3-fill{
 -webkit-box-flex:1;
 -ms-flex-positive:1;
 flex-grow:1;
 -ms-flex-negative:1;
 flex-shrink:1; }
 .bp3-html-select select::before,
 .bp3-select select::before, .bp3-html-select select > \*, .bp3-select select > \*{
 margin-right:7px; }
 .bp3-html-select select:empty::before,
 .bp3-select select:empty::before,
 .bp3-html-select select > :last-child,
 .bp3-select select > :last-child{
 margin-right:0; }
 .bp3-html-select select:hover,
 .bp3-select select:hover{
 background-clip:padding-box;
 background-color:#ebf1f5;
 -webkit-box-shadow:inset 0 0 0 1px rgba(16, 22, 26, 0.2), inset 0 -1px 0 rgba(16, 22, 26, 0.1);
 box-shadow:inset 0 0 0 1px rgba(16, 22, 26, 0.2), inset 0 -1px 0 rgba(16, 22, 26, 0.1); }
 .bp3-html-select select:active,
 .bp3-select select:active, .bp3-html-select select.bp3-active,
 .bp3-select select.bp3-active{
 background-color:#d8e1e8;
 background-image:none;
 -webkit-box-shadow:inset 0 0 0 1px rgba(16, 22, 26, 0.2), inset 0 1px 2px rgba(16, 22, 26, 0.2);
 box-shadow:inset 0 0 0 1px rgba(16, 22, 26, 0.2), inset 0 1px 2px rgba(16, 22, 26, 0.2); }
 .bp3-html-select select:disabled,
 .bp3-select select:disabled, .bp3-html-select select.bp3-disabled,
 .bp3-select select.bp3-disabled{
 background-color:rgba(206, 217, 224, 0.5);
 background-image:none;
 -webkit-box-shadow:none;
 box-shadow:none;
 color:rgba(92, 112, 128, 0.6);
 cursor:not-allowed;
 outline:none; }
 .bp3-html-select select:disabled.bp3-active,
 .bp3-select select:disabled.bp3-active, .bp3-html-select select:disabled.bp3-active:hover,
 .bp3-select select:disabled.bp3-active:hover, .bp3-html-select select.bp3-disabled.bp3-active,
 .bp3-select select.bp3-disabled.bp3-active, .bp3-html-select select.bp3-disabled.bp3-active:hover,
 .bp3-select select.bp3-disabled.bp3-active:hover{
 background:rgba(206, 217, 224, 0.7); }

.bp3-html-select.bp3-minimal select,
.bp3-select.bp3-minimal select{
 background:none;
 -webkit-box-shadow:none;
 box-shadow:none; }
 .bp3-html-select.bp3-minimal select:hover,
 .bp3-select.bp3-minimal select:hover{
 background:rgba(167, 182, 194, 0.3);
 -webkit-box-shadow:none;
 box-shadow:none;
 color:#182026;
 text-decoration:none; }
 .bp3-html-select.bp3-minimal select:active,
 .bp3-select.bp3-minimal select:active, .bp3-html-select.bp3-minimal select.bp3-active,
 .bp3-select.bp3-minimal select.bp3-active{
 background:rgba(115, 134, 148, 0.3);
 -webkit-box-shadow:none;
 box-shadow:none;
 color:#182026; }
 .bp3-html-select.bp3-minimal select:disabled,
 .bp3-select.bp3-minimal select:disabled, .bp3-html-select.bp3-minimal select:disabled:hover,
 .bp3-select.bp3-minimal select:disabled:hover, .bp3-html-select.bp3-minimal select.bp3-disabled,
 .bp3-select.bp3-minimal select.bp3-disabled, .bp3-html-select.bp3-minimal select.bp3-disabled:hover,
 .bp3-select.bp3-minimal select.bp3-disabled:hover{
 background:none;
 color:rgba(92, 112, 128, 0.6);
 cursor:not-allowed; }
 .bp3-html-select.bp3-minimal select:disabled.bp3-active,
 .bp3-select.bp3-minimal select:disabled.bp3-active, .bp3-html-select.bp3-minimal select:disabled:hover.bp3-active,
 .bp3-select.bp3-minimal select:disabled:hover.bp3-active, .bp3-html-select.bp3-minimal select.bp3-disabled.bp3-active,
 .bp3-select.bp3-minimal select.bp3-disabled.bp3-active, .bp3-html-select.bp3-minimal select.bp3-disabled:hover.bp3-active,
 .bp3-select.bp3-minimal select.bp3-disabled:hover.bp3-active{
 background:rgba(115, 134, 148, 0.3); }
 .bp3-dark .bp3-html-select.bp3-minimal select, .bp3-html-select.bp3-minimal .bp3-dark select,
 .bp3-dark .bp3-select.bp3-minimal select, .bp3-select.bp3-minimal .bp3-dark select{
 background:none;
 -webkit-box-shadow:none;
 box-shadow:none;
 color:inherit; }
 .bp3-dark .bp3-html-select.bp3-minimal select:hover, .bp3-html-select.bp3-minimal .bp3-dark select:hover,
 .bp3-dark .bp3-select.bp3-minimal select:hover, .bp3-select.bp3-minimal .bp3-dark select:hover, .bp3-dark .bp3-html-select.bp3-minimal select:active, .bp3-html-select.bp3-minimal .bp3-dark select:active,
 .bp3-dark .bp3-select.bp3-minimal select:active, .bp3-select.bp3-minimal .bp3-dark select:active, .bp3-dark .bp3-html-select.bp3-minimal select.bp3-active, .bp3-html-select.bp3-minimal .bp3-dark select.bp3-active,
 .bp3-dark .bp3-select.bp3-minimal select.bp3-active, .bp3-select.bp3-minimal .bp3-dark select.bp3-active{
 background:none;
 -webkit-box-shadow:none;
 box-shadow:none; }
 .bp3-dark .bp3-html-select.bp3-minimal select:hover, .bp3-html-select.bp3-minimal .bp3-dark select:hover,
 .bp3-dark .bp3-select.bp3-minimal select:hover, .bp3-select.bp3-minimal .bp3-dark select:hover{
 background:rgba(138, 155, 168, 0.15); }
 .bp3-dark .bp3-html-select.bp3-minimal select:active, .bp3-html-select.bp3-minimal .bp3-dark select:active,
 .bp3-dark .bp3-select.bp3-minimal select:active, .bp3-select.bp3-minimal .bp3-dark select:active, .bp3-dark .bp3-html-select.bp3-minimal select.bp3-active, .bp3-html-select.bp3-minimal .bp3-dark select.bp3-active,
 .bp3-dark .bp3-select.bp3-minimal select.bp3-active, .bp3-select.bp3-minimal .bp3-dark select.bp3-active{
 background:rgba(138, 155, 168, 0.3);
 color:#f5f8fa; }
 .bp3-dark .bp3-html-select.bp3-minimal select:disabled, .bp3-html-select.bp3-minimal .bp3-dark select:disabled,
 .bp3-dark .bp3-select.bp3-minimal select:disabled, .bp3-select.bp3-minimal .bp3-dark select:disabled, .bp3-dark .bp3-html-select.bp3-minimal select:disabled:hover, .bp3-html-select.bp3-minimal .bp3-dark select:disabled:hover,
 .bp3-dark .bp3-select.bp3-minimal select:disabled:hover, .bp3-select.bp3-minimal .bp3-dark select:disabled:hover, .bp3-dark .bp3-html-select.bp3-minimal select.bp3-disabled, .bp3-html-select.bp3-minimal .bp3-dark select.bp3-disabled,
 .bp3-dark .bp3-select.bp3-minimal select.bp3-disabled, .bp3-select.bp3-minimal .bp3-dark select.bp3-disabled, .bp3-dark .bp3-html-select.bp3-minimal select.bp3-disabled:hover, .bp3-html-select.bp3-minimal .bp3-dark select.bp3-disabled:hover,
 .bp3-dark .bp3-select.bp3-minimal select.bp3-disabled:hover, .bp3-select.bp3-minimal .bp3-dark select.bp3-disabled:hover{
 background:none;
 color:rgba(167, 182, 194, 0.6);
 cursor:not-allowed; }
 .bp3-dark .bp3-html-select.bp3-minimal select:disabled.bp3-active, .bp3-html-select.bp3-minimal .bp3-dark select:disabled.bp3-active,
 .bp3-dark .bp3-select.bp3-minimal select:disabled.bp3-active, .bp3-select.bp3-minimal .bp3-dark select:disabled.bp3-active, .bp3-dark .bp3-html-select.bp3-minimal select:disabled:hover.bp3-active, .bp3-html-select.bp3-minimal .bp3-dark select:disabled:hover.bp3-active,
 .bp3-dark .bp3-select.bp3-minimal select:disabled:hover.bp3-active, .bp3-select.bp3-minimal .bp3-dark select:disabled:hover.bp3-active, .bp3-dark .bp3-html-select.bp3-minimal select.bp3-disabled.bp3-active, .bp3-html-select.bp3-minimal .bp3-dark select.bp3-disabled.bp3-active,
 .bp3-dark .bp3-select.bp3-minimal select.bp3-disabled.bp3-active, .bp3-select.bp3-minimal .bp3-dark select.bp3-disabled.bp3-active, .bp3-dark .bp3-html-select.bp3-minimal select.bp3-disabled:hover.bp3-active, .bp3-html-select.bp3-minimal .bp3-dark select.bp3-disabled:hover.bp3-active,
 .bp3-dark .bp3-select.bp3-minimal select.bp3-disabled:hover.bp3-active, .bp3-select.bp3-minimal .bp3-dark select.bp3-disabled:hover.bp3-active{
 background:rgba(138, 155, 168, 0.3); }
 .bp3-html-select.bp3-minimal select.bp3-intent-primary,
 .bp3-select.bp3-minimal select.bp3-intent-primary{
 color:#106ba3; }
 .bp3-html-select.bp3-minimal select.bp3-intent-primary:hover,
 .bp3-select.bp3-minimal select.bp3-intent-primary:hover, .bp3-html-select.bp3-minimal select.bp3-intent-primary:active,
 .bp3-select.bp3-minimal select.bp3-intent-primary:active, .bp3-html-select.bp3-minimal select.bp3-intent-primary.bp3-active,
 .bp3-select.bp3-minimal select.bp3-intent-primary.bp3-active{
 background:none;
 -webkit-box-shadow:none;
 box-shadow:none;
 color:#106ba3; }
 .bp3-html-select.bp3-minimal select.bp3-intent-primary:hover,
 .bp3-select.bp3-minimal select.bp3-intent-primary:hover{
 background:rgba(19, 124, 189, 0.15);
 color:#106ba3; }
 .bp3-html-select.bp3-minimal select.bp3-intent-primary:active,
 .bp3-select.bp3-minimal select.bp3-intent-primary:active, .bp3-html-select.bp3-minimal select.bp3-intent-primary.bp3-active,
 .bp3-select.bp3-minimal select.bp3-intent-primary.bp3-active{
 background:rgba(19, 124, 189, 0.3);
 color:#106ba3; }
 .bp3-html-select.bp3-minimal select.bp3-intent-primary:disabled,
 .bp3-select.bp3-minimal select.bp3-intent-primary:disabled, .bp3-html-select.bp3-minimal select.bp3-intent-primary.bp3-disabled,
 .bp3-select.bp3-minimal select.bp3-intent-primary.bp3-disabled{
 background:none;
 color:rgba(16, 107, 163, 0.5); }
 .bp3-html-select.bp3-minimal select.bp3-intent-primary:disabled.bp3-active,
 .bp3-select.bp3-minimal select.bp3-intent-primary:disabled.bp3-active, .bp3-html-select.bp3-minimal select.bp3-intent-primary.bp3-disabled.bp3-active,
 .bp3-select.bp3-minimal select.bp3-intent-primary.bp3-disabled.bp3-active{
 background:rgba(19, 124, 189, 0.3); }
 .bp3-html-select.bp3-minimal select.bp3-intent-primary .bp3-button-spinner .bp3-spinner-head, .bp3-select.bp3-minimal select.bp3-intent-primary .bp3-button-spinner .bp3-spinner-head{
 stroke:#106ba3; }
 .bp3-dark .bp3-html-select.bp3-minimal select.bp3-intent-primary, .bp3-html-select.bp3-minimal .bp3-dark select.bp3-intent-primary,
 .bp3-dark .bp3-select.bp3-minimal select.bp3-intent-primary, .bp3-select.bp3-minimal .bp3-dark select.bp3-intent-primary{
 color:#48aff0; }
 .bp3-dark .bp3-html-select.bp3-minimal select.bp3-intent-primary:hover, .bp3-html-select.bp3-minimal .bp3-dark select.bp3-intent-primary:hover,
 .bp3-dark .bp3-select.bp3-minimal select.bp3-intent-primary:hover, .bp3-select.bp3-minimal .bp3-dark select.bp3-intent-primary:hover{
 background:rgba(19, 124, 189, 0.2);
 color:#48aff0; }
 .bp3-dark .bp3-html-select.bp3-minimal select.bp3-intent-primary:active, .bp3-html-select.bp3-minimal .bp3-dark select.bp3-intent-primary:active,
 .bp3-dark .bp3-select.bp3-minimal select.bp3-intent-primary:active, .bp3-select.bp3-minimal .bp3-dark select.bp3-intent-primary:active, .bp3-dark .bp3-html-select.bp3-minimal select.bp3-intent-primary.bp3-active, .bp3-html-select.bp3-minimal .bp3-dark select.bp3-intent-primary.bp3-active,
 .bp3-dark .bp3-select.bp3-minimal select.bp3-intent-primary.bp3-active, .bp3-select.bp3-minimal .bp3-dark select.bp3-intent-primary.bp3-active{
 background:rgba(19, 124, 189, 0.3);
 color:#48aff0; }
 .bp3-dark .bp3-html-select.bp3-minimal select.bp3-intent-primary:disabled, .bp3-html-select.bp3-minimal .bp3-dark select.bp3-intent-primary:disabled,
 .bp3-dark .bp3-select.bp3-minimal select.bp3-intent-primary:disabled, .bp3-select.bp3-minimal .bp3-dark select.bp3-intent-primary:disabled, .bp3-dark .bp3-html-select.bp3-minimal select.bp3-intent-primary.bp3-disabled, .bp3-html-select.bp3-minimal .bp3-dark select.bp3-intent-primary.bp3-disabled,
 .bp3-dark .bp3-select.bp3-minimal select.bp3-intent-primary.bp3-disabled, .bp3-select.bp3-minimal .bp3-dark select.bp3-intent-primary.bp3-disabled{
 background:none;
 color:rgba(72, 175, 240, 0.5); }
 .bp3-dark .bp3-html-select.bp3-minimal select.bp3-intent-primary:disabled.bp3-active, .bp3-html-select.bp3-minimal .bp3-dark select.bp3-intent-primary:disabled.bp3-active,
 .bp3-dark .bp3-select.bp3-minimal select.bp3-intent-primary:disabled.bp3-active, .bp3-select.bp3-minimal .bp3-dark select.bp3-intent-primary:disabled.bp3-active, .bp3-dark .bp3-html-select.bp3-minimal select.bp3-intent-primary.bp3-disabled.bp3-active, .bp3-html-select.bp3-minimal .bp3-dark select.bp3-intent-primary.bp3-disabled.bp3-active,
 .bp3-dark .bp3-select.bp3-minimal select.bp3-intent-primary.bp3-disabled.bp3-active, .bp3-select.bp3-minimal .bp3-dark select.bp3-intent-primary.bp3-disabled.bp3-active{
 background:rgba(19, 124, 189, 0.3); }
 .bp3-html-select.bp3-minimal select.bp3-intent-success,
 .bp3-select.bp3-minimal select.bp3-intent-success{
 color:#0d8050; }
 .bp3-html-select.bp3-minimal select.bp3-intent-success:hover,
 .bp3-select.bp3-minimal select.bp3-intent-success:hover, .bp3-html-select.bp3-minimal select.bp3-intent-success:active,
 .bp3-select.bp3-minimal select.bp3-intent-success:active, .bp3-html-select.bp3-minimal select.bp3-intent-success.bp3-active,
 .bp3-select.bp3-minimal select.bp3-intent-success.bp3-active{
 background:none;
 -webkit-box-shadow:none;
 box-shadow:none;
 color:#0d8050; }
 .bp3-html-select.bp3-minimal select.bp3-intent-success:hover,
 .bp3-select.bp3-minimal select.bp3-intent-success:hover{
 background:rgba(15, 153, 96, 0.15);
 color:#0d8050; }
 .bp3-html-select.bp3-minimal select.bp3-intent-success:active,
 .bp3-select.bp3-minimal select.bp3-intent-success:active, .bp3-html-select.bp3-minimal select.bp3-intent-success.bp3-active,
 .bp3-select.bp3-minimal select.bp3-intent-success.bp3-active{
 background:rgba(15, 153, 96, 0.3);
 color:#0d8050; }
 .bp3-html-select.bp3-minimal select.bp3-intent-success:disabled,
 .bp3-select.bp3-minimal select.bp3-intent-success:disabled, .bp3-html-select.bp3-minimal select.bp3-intent-success.bp3-disabled,
 .bp3-select.bp3-minimal select.bp3-intent-success.bp3-disabled{
 background:none;
 color:rgba(13, 128, 80, 0.5); }
 .bp3-html-select.bp3-minimal select.bp3-intent-success:disabled.bp3-active,
 .bp3-select.bp3-minimal select.bp3-intent-success:disabled.bp3-active, .bp3-html-select.bp3-minimal select.bp3-intent-success.bp3-disabled.bp3-active,
 .bp3-select.bp3-minimal select.bp3-intent-success.bp3-disabled.bp3-active{
 background:rgba(15, 153, 96, 0.3); }
 .bp3-html-select.bp3-minimal select.bp3-intent-success .bp3-button-spinner .bp3-spinner-head, .bp3-select.bp3-minimal select.bp3-intent-success .bp3-button-spinner .bp3-spinner-head{
 stroke:#0d8050; }
 .bp3-dark .bp3-html-select.bp3-minimal select.bp3-intent-success, .bp3-html-select.bp3-minimal .bp3-dark select.bp3-intent-success,
 .bp3-dark .bp3-select.bp3-minimal select.bp3-intent-success, .bp3-select.bp3-minimal .bp3-dark select.bp3-intent-success{
 color:#3dcc91; }
 .bp3-dark .bp3-html-select.bp3-minimal select.bp3-intent-success:hover, .bp3-html-select.bp3-minimal .bp3-dark select.bp3-intent-success:hover,
 .bp3-dark .bp3-select.bp3-minimal select.bp3-intent-success:hover, .bp3-select.bp3-minimal .bp3-dark select.bp3-intent-success:hover{
 background:rgba(15, 153, 96, 0.2);
 color:#3dcc91; }
 .bp3-dark .bp3-html-select.bp3-minimal select.bp3-intent-success:active, .bp3-html-select.bp3-minimal .bp3-dark select.bp3-intent-success:active,
 .bp3-dark .bp3-select.bp3-minimal select.bp3-intent-success:active, .bp3-select.bp3-minimal .bp3-dark select.bp3-intent-success:active, .bp3-dark .bp3-html-select.bp3-minimal select.bp3-intent-success.bp3-active, .bp3-html-select.bp3-minimal .bp3-dark select.bp3-intent-success.bp3-active,
 .bp3-dark .bp3-select.bp3-minimal select.bp3-intent-success.bp3-active, .bp3-select.bp3-minimal .bp3-dark select.bp3-intent-success.bp3-active{
 background:rgba(15, 153, 96, 0.3);
 color:#3dcc91; }
 .bp3-dark .bp3-html-select.bp3-minimal select.bp3-intent-success:disabled, .bp3-html-select.bp3-minimal .bp3-dark select.bp3-intent-success:disabled,
 .bp3-dark .bp3-select.bp3-minimal select.bp3-intent-success:disabled, .bp3-select.bp3-minimal .bp3-dark select.bp3-intent-success:disabled, .bp3-dark .bp3-html-select.bp3-minimal select.bp3-intent-success.bp3-disabled, .bp3-html-select.bp3-minimal .bp3-dark select.bp3-intent-success.bp3-disabled,
 .bp3-dark .bp3-select.bp3-minimal select.bp3-intent-success.bp3-disabled, .bp3-select.bp3-minimal .bp3-dark select.bp3-intent-success.bp3-disabled{
 background:none;
 color:rgba(61, 204, 145, 0.5); }
 .bp3-dark .bp3-html-select.bp3-minimal select.bp3-intent-success:disabled.bp3-active, .bp3-html-select.bp3-minimal .bp3-dark select.bp3-intent-success:disabled.bp3-active,
 .bp3-dark .bp3-select.bp3-minimal select.bp3-intent-success:disabled.bp3-active, .bp3-select.bp3-minimal .bp3-dark select.bp3-intent-success:disabled.bp3-active, .bp3-dark .bp3-html-select.bp3-minimal select.bp3-intent-success.bp3-disabled.bp3-active, .bp3-html-select.bp3-minimal .bp3-dark select.bp3-intent-success.bp3-disabled.bp3-active,
 .bp3-dark .bp3-select.bp3-minimal select.bp3-intent-success.bp3-disabled.bp3-active, .bp3-select.bp3-minimal .bp3-dark select.bp3-intent-success.bp3-disabled.bp3-active{
 background:rgba(15, 153, 96, 0.3); }
 .bp3-html-select.bp3-minimal select.bp3-intent-warning,
 .bp3-select.bp3-minimal select.bp3-intent-warning{
 color:#bf7326; }
 .bp3-html-select.bp3-minimal select.bp3-intent-warning:hover,
 .bp3-select.bp3-minimal select.bp3-intent-warning:hover, .bp3-html-select.bp3-minimal select.bp3-intent-warning:active,
 .bp3-select.bp3-minimal select.bp3-intent-warning:active, .bp3-html-select.bp3-minimal select.bp3-intent-warning.bp3-active,
 .bp3-select.bp3-minimal select.bp3-intent-warning.bp3-active{
 background:none;
 -webkit-box-shadow:none;
 box-shadow:none;
 color:#bf7326; }
 .bp3-html-select.bp3-minimal select.bp3-intent-warning:hover,
 .bp3-select.bp3-minimal select.bp3-intent-warning:hover{
 background:rgba(217, 130, 43, 0.15);
 color:#bf7326; }
 .bp3-html-select.bp3-minimal select.bp3-intent-warning:active,
 .bp3-select.bp3-minimal select.bp3-intent-warning:active, .bp3-html-select.bp3-minimal select.bp3-intent-warning.bp3-active,
 .bp3-select.bp3-minimal select.bp3-intent-warning.bp3-active{
 background:rgba(217, 130, 43, 0.3);
 color:#bf7326; }
 .bp3-html-select.bp3-minimal select.bp3-intent-warning:disabled,
 .bp3-select.bp3-minimal select.bp3-intent-warning:disabled, .bp3-html-select.bp3-minimal select.bp3-intent-warning.bp3-disabled,
 .bp3-select.bp3-minimal select.bp3-intent-warning.bp3-disabled{
 background:none;
 color:rgba(191, 115, 38, 0.5); }
 .bp3-html-select.bp3-minimal select.bp3-intent-warning:disabled.bp3-active,
 .bp3-select.bp3-minimal select.bp3-intent-warning:disabled.bp3-active, .bp3-html-select.bp3-minimal select.bp3-intent-warning.bp3-disabled.bp3-active,
 .bp3-select.bp3-minimal select.bp3-intent-warning.bp3-disabled.bp3-active{
 background:rgba(217, 130, 43, 0.3); }
 .bp3-html-select.bp3-minimal select.bp3-intent-warning .bp3-button-spinner .bp3-spinner-head, .bp3-select.bp3-minimal select.bp3-intent-warning .bp3-button-spinner .bp3-spinner-head{
 stroke:#bf7326; }
 .bp3-dark .bp3-html-select.bp3-minimal select.bp3-intent-warning, .bp3-html-select.bp3-minimal .bp3-dark select.bp3-intent-warning,
 .bp3-dark .bp3-select.bp3-minimal select.bp3-intent-warning, .bp3-select.bp3-minimal .bp3-dark select.bp3-intent-warning{
 color:#ffb366; }
 .bp3-dark .bp3-html-select.bp3-minimal select.bp3-intent-warning:hover, .bp3-html-select.bp3-minimal .bp3-dark select.bp3-intent-warning:hover,
 .bp3-dark .bp3-select.bp3-minimal select.bp3-intent-warning:hover, .bp3-select.bp3-minimal .bp3-dark select.bp3-intent-warning:hover{
 background:rgba(217, 130, 43, 0.2);
 color:#ffb366; }
 .bp3-dark .bp3-html-select.bp3-minimal select.bp3-intent-warning:active, .bp3-html-select.bp3-minimal .bp3-dark select.bp3-intent-warning:active,
 .bp3-dark .bp3-select.bp3-minimal select.bp3-intent-warning:active, .bp3-select.bp3-minimal .bp3-dark select.bp3-intent-warning:active, .bp3-dark .bp3-html-select.bp3-minimal select.bp3-intent-warning.bp3-active, .bp3-html-select.bp3-minimal .bp3-dark select.bp3-intent-warning.bp3-active,
 .bp3-dark .bp3-select.bp3-minimal select.bp3-intent-warning.bp3-active, .bp3-select.bp3-minimal .bp3-dark select.bp3-intent-warning.bp3-active{
 background:rgba(217, 130, 43, 0.3);
 color:#ffb366; }
 .bp3-dark .bp3-html-select.bp3-minimal select.bp3-intent-warning:disabled, .bp3-html-select.bp3-minimal .bp3-dark select.bp3-intent-warning:disabled,
 .bp3-dark .bp3-select.bp3-minimal select.bp3-intent-warning:disabled, .bp3-select.bp3-minimal .bp3-dark select.bp3-intent-warning:disabled, .bp3-dark .bp3-html-select.bp3-minimal select.bp3-intent-warning.bp3-disabled, .bp3-html-select.bp3-minimal .bp3-dark select.bp3-intent-warning.bp3-disabled,
 .bp3-dark .bp3-select.bp3-minimal select.bp3-intent-warning.bp3-disabled, .bp3-select.bp3-minimal .bp3-dark select.bp3-intent-warning.bp3-disabled{
 background:none;
 color:rgba(255, 179, 102, 0.5); }
 .bp3-dark .bp3-html-select.bp3-minimal select.bp3-intent-warning:disabled.bp3-active, .bp3-html-select.bp3-minimal .bp3-dark select.bp3-intent-warning:disabled.bp3-active,
 .bp3-dark .bp3-select.bp3-minimal select.bp3-intent-warning:disabled.bp3-active, .bp3-select.bp3-minimal .bp3-dark select.bp3-intent-warning:disabled.bp3-active, .bp3-dark .bp3-html-select.bp3-minimal select.bp3-intent-warning.bp3-disabled.bp3-active, .bp3-html-select.bp3-minimal .bp3-dark select.bp3-intent-warning.bp3-disabled.bp3-active,
 .bp3-dark .bp3-select.bp3-minimal select.bp3-intent-warning.bp3-disabled.bp3-active, .bp3-select.bp3-minimal .bp3-dark select.bp3-intent-warning.bp3-disabled.bp3-active{
 background:rgba(217, 130, 43, 0.3); }
 .bp3-html-select.bp3-minimal select.bp3-intent-danger,
 .bp3-select.bp3-minimal select.bp3-intent-danger{
 color:#c23030; }
 .bp3-html-select.bp3-minimal select.bp3-intent-danger:hover,
 .bp3-select.bp3-minimal select.bp3-intent-danger:hover, .bp3-html-select.bp3-minimal select.bp3-intent-danger:active,
 .bp3-select.bp3-minimal select.bp3-intent-danger:active, .bp3-html-select.bp3-minimal select.bp3-intent-danger.bp3-active,
 .bp3-select.bp3-minimal select.bp3-intent-danger.bp3-active{
 background:none;
 -webkit-box-shadow:none;
 box-shadow:none;
 color:#c23030; }
 .bp3-html-select.bp3-minimal select.bp3-intent-danger:hover,
 .bp3-select.bp3-minimal select.bp3-intent-danger:hover{
 background:rgba(219, 55, 55, 0.15);
 color:#c23030; }
 .bp3-html-select.bp3-minimal select.bp3-intent-danger:active,
 .bp3-select.bp3-minimal select.bp3-intent-danger:active, .bp3-html-select.bp3-minimal select.bp3-intent-danger.bp3-active,
 .bp3-select.bp3-minimal select.bp3-intent-danger.bp3-active{
 background:rgba(219, 55, 55, 0.3);
 color:#c23030; }
 .bp3-html-select.bp3-minimal select.bp3-intent-danger:disabled,
 .bp3-select.bp3-minimal select.bp3-intent-danger:disabled, .bp3-html-select.bp3-minimal select.bp3-intent-danger.bp3-disabled,
 .bp3-select.bp3-minimal select.bp3-intent-danger.bp3-disabled{
 background:none;
 color:rgba(194, 48, 48, 0.5); }
 .bp3-html-select.bp3-minimal select.bp3-intent-danger:disabled.bp3-active,
 .bp3-select.bp3-minimal select.bp3-intent-danger:disabled.bp3-active, .bp3-html-select.bp3-minimal select.bp3-intent-danger.bp3-disabled.bp3-active,
 .bp3-select.bp3-minimal select.bp3-intent-danger.bp3-disabled.bp3-active{
 background:rgba(219, 55, 55, 0.3); }
 .bp3-html-select.bp3-minimal select.bp3-intent-danger .bp3-button-spinner .bp3-spinner-head, .bp3-select.bp3-minimal select.bp3-intent-danger .bp3-button-spinner .bp3-spinner-head{
 stroke:#c23030; }
 .bp3-dark .bp3-html-select.bp3-minimal select.bp3-intent-danger, .bp3-html-select.bp3-minimal .bp3-dark select.bp3-intent-danger,
 .bp3-dark .bp3-select.bp3-minimal select.bp3-intent-danger, .bp3-select.bp3-minimal .bp3-dark select.bp3-intent-danger{
 color:#ff7373; }
 .bp3-dark .bp3-html-select.bp3-minimal select.bp3-intent-danger:hover, .bp3-html-select.bp3-minimal .bp3-dark select.bp3-intent-danger:hover,
 .bp3-dark .bp3-select.bp3-minimal select.bp3-intent-danger:hover, .bp3-select.bp3-minimal .bp3-dark select.bp3-intent-danger:hover{
 background:rgba(219, 55, 55, 0.2);
 color:#ff7373; }
 .bp3-dark .bp3-html-select.bp3-minimal select.bp3-intent-danger:active, .bp3-html-select.bp3-minimal .bp3-dark select.bp3-intent-danger:active,
 .bp3-dark .bp3-select.bp3-minimal select.bp3-intent-danger:active, .bp3-select.bp3-minimal .bp3-dark select.bp3-intent-danger:active, .bp3-dark .bp3-html-select.bp3-minimal select.bp3-intent-danger.bp3-active, .bp3-html-select.bp3-minimal .bp3-dark select.bp3-intent-danger.bp3-active,
 .bp3-dark .bp3-select.bp3-minimal select.bp3-intent-danger.bp3-active, .bp3-select.bp3-minimal .bp3-dark select.bp3-intent-danger.bp3-active{
 background:rgba(219, 55, 55, 0.3);
 color:#ff7373; }
 .bp3-dark .bp3-html-select.bp3-minimal select.bp3-intent-danger:disabled, .bp3-html-select.bp3-minimal .bp3-dark select.bp3-intent-danger:disabled,
 .bp3-dark .bp3-select.bp3-minimal select.bp3-intent-danger:disabled, .bp3-select.bp3-minimal .bp3-dark select.bp3-intent-danger:disabled, .bp3-dark .bp3-html-select.bp3-minimal select.bp3-intent-danger.bp3-disabled, .bp3-html-select.bp3-minimal .bp3-dark select.bp3-intent-danger.bp3-disabled,
 .bp3-dark .bp3-select.bp3-minimal select.bp3-intent-danger.bp3-disabled, .bp3-select.bp3-minimal .bp3-dark select.bp3-intent-danger.bp3-disabled{
 background:none;
 color:rgba(255, 115, 115, 0.5); }
 .bp3-dark .bp3-html-select.bp3-minimal select.bp3-intent-danger:disabled.bp3-active, .bp3-html-select.bp3-minimal .bp3-dark select.bp3-intent-danger:disabled.bp3-active,
 .bp3-dark .bp3-select.bp3-minimal select.bp3-intent-danger:disabled.bp3-active, .bp3-select.bp3-minimal .bp3-dark select.bp3-intent-danger:disabled.bp3-active, .bp3-dark .bp3-html-select.bp3-minimal select.bp3-intent-danger.bp3-disabled.bp3-active, .bp3-html-select.bp3-minimal .bp3-dark select.bp3-intent-danger.bp3-disabled.bp3-active,
 .bp3-dark .bp3-select.bp3-minimal select.bp3-intent-danger.bp3-disabled.bp3-active, .bp3-select.bp3-minimal .bp3-dark select.bp3-intent-danger.bp3-disabled.bp3-active{
 background:rgba(219, 55, 55, 0.3); }

.bp3-html-select.bp3-large select,
.bp3-select.bp3-large select{
 font-size:16px;
 height:40px;
 padding-right:35px; }

.bp3-dark .bp3-html-select select, .bp3-dark .bp3-select select{
 background-color:#394b59;
 background-image:-webkit-gradient(linear, left top, left bottom, from(rgba(255, 255, 255, 0.05)), to(rgba(255, 255, 255, 0)));
 background-image:linear-gradient(to bottom, rgba(255, 255, 255, 0.05), rgba(255, 255, 255, 0));
 -webkit-box-shadow:0 0 0 1px rgba(16, 22, 26, 0.4);
 box-shadow:0 0 0 1px rgba(16, 22, 26, 0.4);
 color:#f5f8fa; }
 .bp3-dark .bp3-html-select select:hover, .bp3-dark .bp3-select select:hover, .bp3-dark .bp3-html-select select:active, .bp3-dark .bp3-select select:active, .bp3-dark .bp3-html-select select.bp3-active, .bp3-dark .bp3-select select.bp3-active{
 color:#f5f8fa; }
 .bp3-dark .bp3-html-select select:hover, .bp3-dark .bp3-select select:hover{
 background-color:#30404d;
 -webkit-box-shadow:0 0 0 1px rgba(16, 22, 26, 0.4);
 box-shadow:0 0 0 1px rgba(16, 22, 26, 0.4); }
 .bp3-dark .bp3-html-select select:active, .bp3-dark .bp3-select select:active, .bp3-dark .bp3-html-select select.bp3-active, .bp3-dark .bp3-select select.bp3-active{
 background-color:#202b33;
 background-image:none;
 -webkit-box-shadow:0 0 0 1px rgba(16, 22, 26, 0.6), inset 0 1px 2px rgba(16, 22, 26, 0.2);
 box-shadow:0 0 0 1px rgba(16, 22, 26, 0.6), inset 0 1px 2px rgba(16, 22, 26, 0.2); }
 .bp3-dark .bp3-html-select select:disabled, .bp3-dark .bp3-select select:disabled, .bp3-dark .bp3-html-select select.bp3-disabled, .bp3-dark .bp3-select select.bp3-disabled{
 background-color:rgba(57, 75, 89, 0.5);
 background-image:none;
 -webkit-box-shadow:none;
 box-shadow:none;
 color:rgba(167, 182, 194, 0.6); }
 .bp3-dark .bp3-html-select select:disabled.bp3-active, .bp3-dark .bp3-select select:disabled.bp3-active, .bp3-dark .bp3-html-select select.bp3-disabled.bp3-active, .bp3-dark .bp3-select select.bp3-disabled.bp3-active{
 background:rgba(57, 75, 89, 0.7); }
 .bp3-dark .bp3-html-select select .bp3-button-spinner .bp3-spinner-head, .bp3-dark .bp3-select select .bp3-button-spinner .bp3-spinner-head{
 background:rgba(16, 22, 26, 0.5);
 stroke:#8a9ba8; }

.bp3-html-select select:disabled,
.bp3-select select:disabled{
 background-color:rgba(206, 217, 224, 0.5);
 -webkit-box-shadow:none;
 box-shadow:none;
 color:rgba(92, 112, 128, 0.6);
 cursor:not-allowed; }

.bp3-html-select .bp3-icon,
.bp3-select .bp3-icon, .bp3-select::after{
 color:#5c7080;
 pointer-events:none;
 position:absolute;
 right:7px;
 top:7px; }
 .bp3-html-select .bp3-disabled.bp3-icon,
 .bp3-select .bp3-disabled.bp3-icon, .bp3-disabled.bp3-select::after{
 color:rgba(92, 112, 128, 0.6); }
.bp3-html-select,
.bp3-select{
 display:inline-block;
 letter-spacing:normal;
 position:relative;
 vertical-align:middle; }
 .bp3-html-select select::-ms-expand,
 .bp3-select select::-ms-expand{
 display:none; }
 .bp3-html-select .bp3-icon,
 .bp3-select .bp3-icon{
 color:#5c7080; }
 .bp3-html-select .bp3-icon:hover,
 .bp3-select .bp3-icon:hover{
 color:#182026; }
 .bp3-dark .bp3-html-select .bp3-icon, .bp3-dark
 .bp3-select .bp3-icon{
 color:#a7b6c2; }
 .bp3-dark .bp3-html-select .bp3-icon:hover, .bp3-dark
 .bp3-select .bp3-icon:hover{
 color:#f5f8fa; }
 .bp3-html-select.bp3-large::after,
 .bp3-html-select.bp3-large .bp3-icon,
 .bp3-select.bp3-large::after,
 .bp3-select.bp3-large .bp3-icon{
 right:12px;
 top:12px; }
 .bp3-html-select.bp3-fill,
 .bp3-html-select.bp3-fill select,
 .bp3-select.bp3-fill,
 .bp3-select.bp3-fill select{
 width:100%; }
 .bp3-dark .bp3-html-select option, .bp3-dark
 .bp3-select option{
 background-color:#30404d;
 color:#f5f8fa; }
 .bp3-dark .bp3-html-select option:disabled, .bp3-dark
 .bp3-select option:disabled{
 color:rgba(167, 182, 194, 0.6); }
 .bp3-dark .bp3-html-select::after, .bp3-dark
 .bp3-select::after{
 color:#a7b6c2; }

.bp3-select::after{
 font-family:"Icons16", sans-serif;
 font-size:16px;
 font-style:normal;
 font-weight:400;
 line-height:1;
 -moz-osx-font-smoothing:grayscale;
 -webkit-font-smoothing:antialiased;
 content:""; }
.bp3-running-text table, table.bp3-html-table{
 border-spacing:0;
 font-size:14px; }
 .bp3-running-text table th, table.bp3-html-table th,
 .bp3-running-text table td,
 table.bp3-html-table td{
 padding:11px;
 text-align:left;
 vertical-align:top; }
 .bp3-running-text table th, table.bp3-html-table th{
 color:#182026;
 font-weight:600; }
 
 .bp3-running-text table td,
 table.bp3-html-table td{
 color:#182026; }
 .bp3-running-text table tbody tr:first-child th, table.bp3-html-table tbody tr:first-child th,
 .bp3-running-text table tbody tr:first-child td,
 table.bp3-html-table tbody tr:first-child td,
 .bp3-running-text table tfoot tr:first-child th,
 table.bp3-html-table tfoot tr:first-child th,
 .bp3-running-text table tfoot tr:first-child td,
 table.bp3-html-table tfoot tr:first-child td{
 -webkit-box-shadow:inset 0 1px 0 0 rgba(16, 22, 26, 0.15);
 box-shadow:inset 0 1px 0 0 rgba(16, 22, 26, 0.15); }
 .bp3-dark .bp3-running-text table th, .bp3-running-text .bp3-dark table th, .bp3-dark table.bp3-html-table th{
 color:#f5f8fa; }
 .bp3-dark .bp3-running-text table td, .bp3-running-text .bp3-dark table td, .bp3-dark table.bp3-html-table td{
 color:#f5f8fa; }
 .bp3-dark .bp3-running-text table tbody tr:first-child th, .bp3-running-text .bp3-dark table tbody tr:first-child th, .bp3-dark table.bp3-html-table tbody tr:first-child th,
 .bp3-dark .bp3-running-text table tbody tr:first-child td,
 .bp3-running-text .bp3-dark table tbody tr:first-child td,
 .bp3-dark table.bp3-html-table tbody tr:first-child td,
 .bp3-dark .bp3-running-text table tfoot tr:first-child th,
 .bp3-running-text .bp3-dark table tfoot tr:first-child th,
 .bp3-dark table.bp3-html-table tfoot tr:first-child th,
 .bp3-dark .bp3-running-text table tfoot tr:first-child td,
 .bp3-running-text .bp3-dark table tfoot tr:first-child td,
 .bp3-dark table.bp3-html-table tfoot tr:first-child td{
 -webkit-box-shadow:inset 0 1px 0 0 rgba(255, 255, 255, 0.15);
 box-shadow:inset 0 1px 0 0 rgba(255, 255, 255, 0.15); }

table.bp3-html-table.bp3-html-table-condensed th,
table.bp3-html-table.bp3-html-table-condensed td, table.bp3-html-table.bp3-small th,
table.bp3-html-table.bp3-small td{
 padding-bottom:6px;
 padding-top:6px; }

table.bp3-html-table.bp3-html-table-striped tbody tr:nth-child(odd) td{
 background:rgba(191, 204, 214, 0.15); }

table.bp3-html-table.bp3-html-table-bordered th:not(:first-child){
 -webkit-box-shadow:inset 1px 0 0 0 rgba(16, 22, 26, 0.15);
 box-shadow:inset 1px 0 0 0 rgba(16, 22, 26, 0.15); }

table.bp3-html-table.bp3-html-table-bordered tbody tr td,
table.bp3-html-table.bp3-html-table-bordered tfoot tr td{
 -webkit-box-shadow:inset 0 1px 0 0 rgba(16, 22, 26, 0.15);
 box-shadow:inset 0 1px 0 0 rgba(16, 22, 26, 0.15); }
 table.bp3-html-table.bp3-html-table-bordered tbody tr td:not(:first-child),
 table.bp3-html-table.bp3-html-table-bordered tfoot tr td:not(:first-child){
 -webkit-box-shadow:inset 1px 1px 0 0 rgba(16, 22, 26, 0.15);
 box-shadow:inset 1px 1px 0 0 rgba(16, 22, 26, 0.15); }

table.bp3-html-table.bp3-html-table-bordered.bp3-html-table-striped tbody tr:not(:first-child) td{
 -webkit-box-shadow:none;
 box-shadow:none; }
 table.bp3-html-table.bp3-html-table-bordered.bp3-html-table-striped tbody tr:not(:first-child) td:not(:first-child){
 -webkit-box-shadow:inset 1px 0 0 0 rgba(16, 22, 26, 0.15);
 box-shadow:inset 1px 0 0 0 rgba(16, 22, 26, 0.15); }

table.bp3-html-table.bp3-interactive tbody tr:hover td{
 background-color:rgba(191, 204, 214, 0.3);
 cursor:pointer; }

table.bp3-html-table.bp3-interactive tbody tr:active td{
 background-color:rgba(191, 204, 214, 0.4); }

.bp3-dark table.bp3-html-table{ }
 .bp3-dark table.bp3-html-table.bp3-html-table-striped tbody tr:nth-child(odd) td{
 background:rgba(92, 112, 128, 0.15); }
 .bp3-dark table.bp3-html-table.bp3-html-table-bordered th:not(:first-child){
 -webkit-box-shadow:inset 1px 0 0 0 rgba(255, 255, 255, 0.15);
 box-shadow:inset 1px 0 0 0 rgba(255, 255, 255, 0.15); }
 .bp3-dark table.bp3-html-table.bp3-html-table-bordered tbody tr td,
 .bp3-dark table.bp3-html-table.bp3-html-table-bordered tfoot tr td{
 -webkit-box-shadow:inset 0 1px 0 0 rgba(255, 255, 255, 0.15);
 box-shadow:inset 0 1px 0 0 rgba(255, 255, 255, 0.15); }
 .bp3-dark table.bp3-html-table.bp3-html-table-bordered tbody tr td:not(:first-child),
 .bp3-dark table.bp3-html-table.bp3-html-table-bordered tfoot tr td:not(:first-child){
 -webkit-box-shadow:inset 1px 1px 0 0 rgba(255, 255, 255, 0.15);
 box-shadow:inset 1px 1px 0 0 rgba(255, 255, 255, 0.15); }
 .bp3-dark table.bp3-html-table.bp3-html-table-bordered.bp3-html-table-striped tbody tr:not(:first-child) td{
 -webkit-box-shadow:inset 1px 0 0 0 rgba(255, 255, 255, 0.15);
 box-shadow:inset 1px 0 0 0 rgba(255, 255, 255, 0.15); }
 .bp3-dark table.bp3-html-table.bp3-html-table-bordered.bp3-html-table-striped tbody tr:not(:first-child) td:first-child{
 -webkit-box-shadow:none;
 box-shadow:none; }
 .bp3-dark table.bp3-html-table.bp3-interactive tbody tr:hover td{
 background-color:rgba(92, 112, 128, 0.3);
 cursor:pointer; }
 .bp3-dark table.bp3-html-table.bp3-interactive tbody tr:active td{
 background-color:rgba(92, 112, 128, 0.4); }

.bp3-key-combo{
 display:-webkit-box;
 display:-ms-flexbox;
 display:flex;
 -webkit-box-orient:horizontal;
 -webkit-box-direction:normal;
 -ms-flex-direction:row;
 flex-direction:row;
 -webkit-box-align:center;
 -ms-flex-align:center;
 align-items:center; }
 .bp3-key-combo > \*{
 -webkit-box-flex:0;
 -ms-flex-positive:0;
 flex-grow:0;
 -ms-flex-negative:0;
 flex-shrink:0; }
 .bp3-key-combo > .bp3-fill{
 -webkit-box-flex:1;
 -ms-flex-positive:1;
 flex-grow:1;
 -ms-flex-negative:1;
 flex-shrink:1; }
 .bp3-key-combo::before,
 .bp3-key-combo > \*{
 margin-right:5px; }
 .bp3-key-combo:empty::before,
 .bp3-key-combo > :last-child{
 margin-right:0; }

.bp3-hotkey-dialog{
 padding-bottom:0;
 top:40px; }
 .bp3-hotkey-dialog .bp3-dialog-body{
 margin:0;
 padding:0; }
 .bp3-hotkey-dialog .bp3-hotkey-label{
 -webkit-box-flex:1;
 -ms-flex-positive:1;
 flex-grow:1; }

.bp3-hotkey-column{
 margin:auto;
 max-height:80vh;
 overflow-y:auto;
 padding:30px; }
 .bp3-hotkey-column .bp3-heading{
 margin-bottom:20px; }
 .bp3-hotkey-column .bp3-heading:not(:first-child){
 margin-top:40px; }

.bp3-hotkey{
 -webkit-box-align:center;
 -ms-flex-align:center;
 align-items:center;
 display:-webkit-box;
 display:-ms-flexbox;
 display:flex;
 -webkit-box-pack:justify;
 -ms-flex-pack:justify;
 justify-content:space-between;
 margin-left:0;
 margin-right:0; }
 .bp3-hotkey:not(:last-child){
 margin-bottom:10px; }
.bp3-icon{
 display:inline-block;
 -webkit-box-flex:0;
 -ms-flex:0 0 auto;
 flex:0 0 auto;
 vertical-align:text-bottom; }
 .bp3-icon:not(:empty)::before{
 content:"" !important;
 content:unset !important; }
 .bp3-icon > svg{
 display:block; }
 .bp3-icon > svg:not([fill]){
 fill:currentColor; }

.bp3-icon.bp3-intent-primary, .bp3-icon-standard.bp3-intent-primary, .bp3-icon-large.bp3-intent-primary{
 color:#106ba3; }
 .bp3-dark .bp3-icon.bp3-intent-primary, .bp3-dark .bp3-icon-standard.bp3-intent-primary, .bp3-dark .bp3-icon-large.bp3-intent-primary{
 color:#48aff0; }

.bp3-icon.bp3-intent-success, .bp3-icon-standard.bp3-intent-success, .bp3-icon-large.bp3-intent-success{
 color:#0d8050; }
 .bp3-dark .bp3-icon.bp3-intent-success, .bp3-dark .bp3-icon-standard.bp3-intent-success, .bp3-dark .bp3-icon-large.bp3-intent-success{
 color:#3dcc91; }

.bp3-icon.bp3-intent-warning, .bp3-icon-standard.bp3-intent-warning, .bp3-icon-large.bp3-intent-warning{
 color:#bf7326; }
 .bp3-dark .bp3-icon.bp3-intent-warning, .bp3-dark .bp3-icon-standard.bp3-intent-warning, .bp3-dark .bp3-icon-large.bp3-intent-warning{
 color:#ffb366; }

.bp3-icon.bp3-intent-danger, .bp3-icon-standard.bp3-intent-danger, .bp3-icon-large.bp3-intent-danger{
 color:#c23030; }
 .bp3-dark .bp3-icon.bp3-intent-danger, .bp3-dark .bp3-icon-standard.bp3-intent-danger, .bp3-dark .bp3-icon-large.bp3-intent-danger{
 color:#ff7373; }

span.bp3-icon-standard{
 font-family:"Icons16", sans-serif;
 font-size:16px;
 font-style:normal;
 font-weight:400;
 line-height:1;
 -moz-osx-font-smoothing:grayscale;
 -webkit-font-smoothing:antialiased;
 display:inline-block; }

span.bp3-icon-large{
 font-family:"Icons20", sans-serif;
 font-size:20px;
 font-style:normal;
 font-weight:400;
 line-height:1;
 -moz-osx-font-smoothing:grayscale;
 -webkit-font-smoothing:antialiased;
 display:inline-block; }

span.bp3-icon:empty{
 font-family:"Icons20";
 font-size:inherit;
 font-style:normal;
 font-weight:400;
 line-height:1; }
 span.bp3-icon:empty::before{
 -moz-osx-font-smoothing:grayscale;
 -webkit-font-smoothing:antialiased; }

.bp3-icon-add::before{
 content:""; }

.bp3-icon-add-column-left::before{
 content:""; }

.bp3-icon-add-column-right::before{
 content:""; }

.bp3-icon-add-row-bottom::before{
 content:""; }

.bp3-icon-add-row-top::before{
 content:""; }

.bp3-icon-add-to-artifact::before{
 content:""; }

.bp3-icon-add-to-folder::before{
 content:""; }

.bp3-icon-airplane::before{
 content:""; }

.bp3-icon-align-center::before{
 content:""; }

.bp3-icon-align-justify::before{
 content:""; }

.bp3-icon-align-left::before{
 content:""; }

.bp3-icon-align-right::before{
 content:""; }

.bp3-icon-alignment-bottom::before{
 content:""; }

.bp3-icon-alignment-horizontal-center::before{
 content:""; }

.bp3-icon-alignment-left::before{
 content:""; }

.bp3-icon-alignment-right::before{
 content:""; }

.bp3-icon-alignment-top::before{
 content:""; }

.bp3-icon-alignment-vertical-center::before{
 content:""; }

.bp3-icon-annotation::before{
 content:""; }

.bp3-icon-application::before{
 content:""; }

.bp3-icon-applications::before{
 content:""; }

.bp3-icon-archive::before{
 content:""; }

.bp3-icon-arrow-bottom-left::before{
 content:"↙"; }

.bp3-icon-arrow-bottom-right::before{
 content:"↘"; }

.bp3-icon-arrow-down::before{
 content:"↓"; }

.bp3-icon-arrow-left::before{
 content:"←"; }

.bp3-icon-arrow-right::before{
 content:"→"; }

.bp3-icon-arrow-top-left::before{
 content:"↖"; }

.bp3-icon-arrow-top-right::before{
 content:"↗"; }

.bp3-icon-arrow-up::before{
 content:"↑"; }

.bp3-icon-arrows-horizontal::before{
 content:"↔"; }

.bp3-icon-arrows-vertical::before{
 content:"↕"; }

.bp3-icon-asterisk::before{
 content:"\*"; }

.bp3-icon-automatic-updates::before{
 content:""; }

.bp3-icon-badge::before{
 content:""; }

.bp3-icon-ban-circle::before{
 content:""; }

.bp3-icon-bank-account::before{
 content:""; }

.bp3-icon-barcode::before{
 content:""; }

.bp3-icon-blank::before{
 content:""; }

.bp3-icon-blocked-person::before{
 content:""; }

.bp3-icon-bold::before{
 content:""; }

.bp3-icon-book::before{
 content:""; }

.bp3-icon-bookmark::before{
 content:""; }

.bp3-icon-box::before{
 content:""; }

.bp3-icon-briefcase::before{
 content:""; }

.bp3-icon-bring-data::before{
 content:""; }

.bp3-icon-build::before{
 content:""; }

.bp3-icon-calculator::before{
 content:""; }

.bp3-icon-calendar::before{
 content:""; }

.bp3-icon-camera::before{
 content:""; }

.bp3-icon-caret-down::before{
 content:"⌄"; }

.bp3-icon-caret-left::before{
 content:"〈"; }

.bp3-icon-caret-right::before{
 content:"〉"; }

.bp3-icon-caret-up::before{
 content:"⌃"; }

.bp3-icon-cell-tower::before{
 content:""; }

.bp3-icon-changes::before{
 content:""; }

.bp3-icon-chart::before{
 content:""; }

.bp3-icon-chat::before{
 content:""; }

.bp3-icon-chevron-backward::before{
 content:""; }

.bp3-icon-chevron-down::before{
 content:""; }

.bp3-icon-chevron-forward::before{
 content:""; }

.bp3-icon-chevron-left::before{
 content:""; }

.bp3-icon-chevron-right::before{
 content:""; }

.bp3-icon-chevron-up::before{
 content:""; }

.bp3-icon-circle::before{
 content:""; }

.bp3-icon-circle-arrow-down::before{
 content:""; }

.bp3-icon-circle-arrow-left::before{
 content:""; }

.bp3-icon-circle-arrow-right::before{
 content:""; }

.bp3-icon-circle-arrow-up::before{
 content:""; }

.bp3-icon-citation::before{
 content:""; }

.bp3-icon-clean::before{
 content:""; }

.bp3-icon-clipboard::before{
 content:""; }

.bp3-icon-cloud::before{
 content:"☁"; }

.bp3-icon-cloud-download::before{
 content:""; }

.bp3-icon-cloud-upload::before{
 content:""; }

.bp3-icon-code::before{
 content:""; }

.bp3-icon-code-block::before{
 content:""; }

.bp3-icon-cog::before{
 content:""; }

.bp3-icon-collapse-all::before{
 content:""; }

.bp3-icon-column-layout::before{
 content:""; }

.bp3-icon-comment::before{
 content:""; }

.bp3-icon-comparison::before{
 content:""; }

.bp3-icon-compass::before{
 content:""; }

.bp3-icon-compressed::before{
 content:""; }

.bp3-icon-confirm::before{
 content:""; }

.bp3-icon-console::before{
 content:""; }

.bp3-icon-contrast::before{
 content:""; }

.bp3-icon-control::before{
 content:""; }

.bp3-icon-credit-card::before{
 content:""; }

.bp3-icon-cross::before{
 content:"✗"; }

.bp3-icon-crown::before{
 content:""; }

.bp3-icon-cube::before{
 content:""; }

.bp3-icon-cube-add::before{
 content:""; }

.bp3-icon-cube-remove::before{
 content:""; }

.bp3-icon-curved-range-chart::before{
 content:""; }

.bp3-icon-cut::before{
 content:""; }

.bp3-icon-dashboard::before{
 content:""; }

.bp3-icon-data-lineage::before{
 content:""; }

.bp3-icon-database::before{
 content:""; }

.bp3-icon-delete::before{
 content:""; }

.bp3-icon-delta::before{
 content:"Δ"; }

.bp3-icon-derive-column::before{
 content:""; }

.bp3-icon-desktop::before{
 content:""; }

.bp3-icon-diagnosis::before{
 content:""; }

.bp3-icon-diagram-tree::before{
 content:""; }

.bp3-icon-direction-left::before{
 content:""; }

.bp3-icon-direction-right::before{
 content:""; }

.bp3-icon-disable::before{
 content:""; }

.bp3-icon-document::before{
 content:""; }

.bp3-icon-document-open::before{
 content:""; }

.bp3-icon-document-share::before{
 content:""; }

.bp3-icon-dollar::before{
 content:"$"; }

.bp3-icon-dot::before{
 content:"•"; }

.bp3-icon-double-caret-horizontal::before{
 content:""; }

.bp3-icon-double-caret-vertical::before{
 content:""; }

.bp3-icon-double-chevron-down::before{
 content:""; }

.bp3-icon-double-chevron-left::before{
 content:""; }

.bp3-icon-double-chevron-right::before{
 content:""; }

.bp3-icon-double-chevron-up::before{
 content:""; }

.bp3-icon-doughnut-chart::before{
 content:""; }

.bp3-icon-download::before{
 content:""; }

.bp3-icon-drag-handle-horizontal::before{
 content:""; }

.bp3-icon-drag-handle-vertical::before{
 content:""; }

.bp3-icon-draw::before{
 content:""; }

.bp3-icon-drive-time::before{
 content:""; }

.bp3-icon-duplicate::before{
 content:""; }

.bp3-icon-edit::before{
 content:"✎"; }

.bp3-icon-eject::before{
 content:"⏏"; }

.bp3-icon-endorsed::before{
 content:""; }

.bp3-icon-envelope::before{
 content:"✉"; }

.bp3-icon-equals::before{
 content:""; }

.bp3-icon-eraser::before{
 content:""; }

.bp3-icon-error::before{
 content:""; }

.bp3-icon-euro::before{
 content:"€"; }

.bp3-icon-exchange::before{
 content:""; }

.bp3-icon-exclude-row::before{
 content:""; }

.bp3-icon-expand-all::before{
 content:""; }

.bp3-icon-export::before{
 content:""; }

.bp3-icon-eye-off::before{
 content:""; }

.bp3-icon-eye-on::before{
 content:""; }

.bp3-icon-eye-open::before{
 content:""; }

.bp3-icon-fast-backward::before{
 content:""; }

.bp3-icon-fast-forward::before{
 content:""; }

.bp3-icon-feed::before{
 content:""; }

.bp3-icon-feed-subscribed::before{
 content:""; }

.bp3-icon-film::before{
 content:""; }

.bp3-icon-filter::before{
 content:""; }

.bp3-icon-filter-keep::before{
 content:""; }

.bp3-icon-filter-list::before{
 content:""; }

.bp3-icon-filter-open::before{
 content:""; }

.bp3-icon-filter-remove::before{
 content:""; }

.bp3-icon-flag::before{
 content:"⚑"; }

.bp3-icon-flame::before{
 content:""; }

.bp3-icon-flash::before{
 content:""; }

.bp3-icon-floppy-disk::before{
 content:""; }

.bp3-icon-flow-branch::before{
 content:""; }

.bp3-icon-flow-end::before{
 content:""; }

.bp3-icon-flow-linear::before{
 content:""; }

.bp3-icon-flow-review::before{
 content:""; }

.bp3-icon-flow-review-branch::before{
 content:""; }

.bp3-icon-flows::before{
 content:""; }

.bp3-icon-folder-close::before{
 content:""; }

.bp3-icon-folder-new::before{
 content:""; }

.bp3-icon-folder-open::before{
 content:""; }

.bp3-icon-folder-shared::before{
 content:""; }

.bp3-icon-folder-shared-open::before{
 content:""; }

.bp3-icon-follower::before{
 content:""; }

.bp3-icon-following::before{
 content:""; }

.bp3-icon-font::before{
 content:""; }

.bp3-icon-fork::before{
 content:""; }

.bp3-icon-form::before{
 content:""; }

.bp3-icon-full-circle::before{
 content:""; }

.bp3-icon-full-stacked-chart::before{
 content:""; }

.bp3-icon-fullscreen::before{
 content:""; }

.bp3-icon-function::before{
 content:""; }

.bp3-icon-gantt-chart::before{
 content:""; }

.bp3-icon-geolocation::before{
 content:""; }

.bp3-icon-geosearch::before{
 content:""; }

.bp3-icon-git-branch::before{
 content:""; }

.bp3-icon-git-commit::before{
 content:""; }

.bp3-icon-git-merge::before{
 content:""; }

.bp3-icon-git-new-branch::before{
 content:""; }

.bp3-icon-git-pull::before{
 content:""; }

.bp3-icon-git-push::before{
 content:""; }

.bp3-icon-git-repo::before{
 content:""; }

.bp3-icon-glass::before{
 content:""; }

.bp3-icon-globe::before{
 content:""; }

.bp3-icon-globe-network::before{
 content:""; }

.bp3-icon-graph::before{
 content:""; }

.bp3-icon-graph-remove::before{
 content:""; }

.bp3-icon-greater-than::before{
 content:""; }

.bp3-icon-greater-than-or-equal-to::before{
 content:""; }

.bp3-icon-grid::before{
 content:""; }

.bp3-icon-grid-view::before{
 content:""; }

.bp3-icon-group-objects::before{
 content:""; }

.bp3-icon-grouped-bar-chart::before{
 content:""; }

.bp3-icon-hand::before{
 content:""; }

.bp3-icon-hand-down::before{
 content:""; }

.bp3-icon-hand-left::before{
 content:""; }

.bp3-icon-hand-right::before{
 content:""; }

.bp3-icon-hand-up::before{
 content:""; }

.bp3-icon-header::before{
 content:""; }

.bp3-icon-header-one::before{
 content:""; }

.bp3-icon-header-two::before{
 content:""; }

.bp3-icon-headset::before{
 content:""; }

.bp3-icon-heart::before{
 content:"♥"; }

.bp3-icon-heart-broken::before{
 content:""; }

.bp3-icon-heat-grid::before{
 content:""; }

.bp3-icon-heatmap::before{
 content:""; }

.bp3-icon-help::before{
 content:"?"; }

.bp3-icon-helper-management::before{
 content:""; }

.bp3-icon-highlight::before{
 content:""; }

.bp3-icon-history::before{
 content:""; }

.bp3-icon-home::before{
 content:"⌂"; }

.bp3-icon-horizontal-bar-chart::before{
 content:""; }

.bp3-icon-horizontal-bar-chart-asc::before{
 content:""; }

.bp3-icon-horizontal-bar-chart-desc::before{
 content:""; }

.bp3-icon-horizontal-distribution::before{
 content:""; }

.bp3-icon-id-number::before{
 content:""; }

.bp3-icon-image-rotate-left::before{
 content:""; }

.bp3-icon-image-rotate-right::before{
 content:""; }

.bp3-icon-import::before{
 content:""; }

.bp3-icon-inbox::before{
 content:""; }

.bp3-icon-inbox-filtered::before{
 content:""; }

.bp3-icon-inbox-geo::before{
 content:""; }

.bp3-icon-inbox-search::before{
 content:""; }

.bp3-icon-inbox-update::before{
 content:""; }

.bp3-icon-info-sign::before{
 content:"ℹ"; }

.bp3-icon-inheritance::before{
 content:""; }

.bp3-icon-inner-join::before{
 content:""; }

.bp3-icon-insert::before{
 content:""; }

.bp3-icon-intersection::before{
 content:""; }

.bp3-icon-ip-address::before{
 content:""; }

.bp3-icon-issue::before{
 content:""; }

.bp3-icon-issue-closed::before{
 content:""; }

.bp3-icon-issue-new::before{
 content:""; }

.bp3-icon-italic::before{
 content:""; }

.bp3-icon-join-table::before{
 content:""; }

.bp3-icon-key::before{
 content:""; }

.bp3-icon-key-backspace::before{
 content:""; }

.bp3-icon-key-command::before{
 content:""; }

.bp3-icon-key-control::before{
 content:""; }

.bp3-icon-key-delete::before{
 content:""; }

.bp3-icon-key-enter::before{
 content:""; }

.bp3-icon-key-escape::before{
 content:""; }

.bp3-icon-key-option::before{
 content:""; }

.bp3-icon-key-shift::before{
 content:""; }

.bp3-icon-key-tab::before{
 content:""; }

.bp3-icon-known-vehicle::before{
 content:""; }

.bp3-icon-lab-test::before{
 content:""; }

.bp3-icon-label::before{
 content:""; }

.bp3-icon-layer::before{
 content:""; }

.bp3-icon-layers::before{
 content:""; }

.bp3-icon-layout::before{
 content:""; }

.bp3-icon-layout-auto::before{
 content:""; }

.bp3-icon-layout-balloon::before{
 content:""; }

.bp3-icon-layout-circle::before{
 content:""; }

.bp3-icon-layout-grid::before{
 content:""; }

.bp3-icon-layout-group-by::before{
 content:""; }

.bp3-icon-layout-hierarchy::before{
 content:""; }

.bp3-icon-layout-linear::before{
 content:""; }

.bp3-icon-layout-skew-grid::before{
 content:""; }

.bp3-icon-layout-sorted-clusters::before{
 content:""; }

.bp3-icon-learning::before{
 content:""; }

.bp3-icon-left-join::before{
 content:""; }

.bp3-icon-less-than::before{
 content:""; }

.bp3-icon-less-than-or-equal-to::before{
 content:""; }

.bp3-icon-lifesaver::before{
 content:""; }

.bp3-icon-lightbulb::before{
 content:""; }

.bp3-icon-link::before{
 content:""; }

.bp3-icon-list::before{
 content:"☰"; }

.bp3-icon-list-columns::before{
 content:""; }

.bp3-icon-list-detail-view::before{
 content:""; }

.bp3-icon-locate::before{
 content:""; }

.bp3-icon-lock::before{
 content:""; }

.bp3-icon-log-in::before{
 content:""; }

.bp3-icon-log-out::before{
 content:""; }

.bp3-icon-manual::before{
 content:""; }

.bp3-icon-manually-entered-data::before{
 content:""; }

.bp3-icon-map::before{
 content:""; }

.bp3-icon-map-create::before{
 content:""; }

.bp3-icon-map-marker::before{
 content:""; }

.bp3-icon-maximize::before{
 content:""; }

.bp3-icon-media::before{
 content:""; }

.bp3-icon-menu::before{
 content:""; }

.bp3-icon-menu-closed::before{
 content:""; }

.bp3-icon-menu-open::before{
 content:""; }

.bp3-icon-merge-columns::before{
 content:""; }

.bp3-icon-merge-links::before{
 content:""; }

.bp3-icon-minimize::before{
 content:""; }

.bp3-icon-minus::before{
 content:"−"; }

.bp3-icon-mobile-phone::before{
 content:""; }

.bp3-icon-mobile-video::before{
 content:""; }

.bp3-icon-moon::before{
 content:""; }

.bp3-icon-more::before{
 content:""; }

.bp3-icon-mountain::before{
 content:""; }

.bp3-icon-move::before{
 content:""; }

.bp3-icon-mugshot::before{
 content:""; }

.bp3-icon-multi-select::before{
 content:""; }

.bp3-icon-music::before{
 content:""; }

.bp3-icon-new-drawing::before{
 content:""; }

.bp3-icon-new-grid-item::before{
 content:""; }

.bp3-icon-new-layer::before{
 content:""; }

.bp3-icon-new-layers::before{
 content:""; }

.bp3-icon-new-link::before{
 content:""; }

.bp3-icon-new-object::before{
 content:""; }

.bp3-icon-new-person::before{
 content:""; }

.bp3-icon-new-prescription::before{
 content:""; }

.bp3-icon-new-text-box::before{
 content:""; }

.bp3-icon-ninja::before{
 content:""; }

.bp3-icon-not-equal-to::before{
 content:""; }

.bp3-icon-notifications::before{
 content:""; }

.bp3-icon-notifications-updated::before{
 content:""; }

.bp3-icon-numbered-list::before{
 content:""; }

.bp3-icon-numerical::before{
 content:""; }

.bp3-icon-office::before{
 content:""; }

.bp3-icon-offline::before{
 content:""; }

.bp3-icon-oil-field::before{
 content:""; }

.bp3-icon-one-column::before{
 content:""; }

.bp3-icon-outdated::before{
 content:""; }

.bp3-icon-page-layout::before{
 content:""; }

.bp3-icon-panel-stats::before{
 content:""; }

.bp3-icon-panel-table::before{
 content:""; }

.bp3-icon-paperclip::before{
 content:""; }

.bp3-icon-paragraph::before{
 content:""; }

.bp3-icon-path::before{
 content:""; }

.bp3-icon-path-search::before{
 content:""; }

.bp3-icon-pause::before{
 content:""; }

.bp3-icon-people::before{
 content:""; }

.bp3-icon-percentage::before{
 content:""; }

.bp3-icon-person::before{
 content:""; }

.bp3-icon-phone::before{
 content:"☎"; }

.bp3-icon-pie-chart::before{
 content:""; }

.bp3-icon-pin::before{
 content:""; }

.bp3-icon-pivot::before{
 content:""; }

.bp3-icon-pivot-table::before{
 content:""; }

.bp3-icon-play::before{
 content:""; }

.bp3-icon-plus::before{
 content:"+"; }

.bp3-icon-polygon-filter::before{
 content:""; }

.bp3-icon-power::before{
 content:""; }

.bp3-icon-predictive-analysis::before{
 content:""; }

.bp3-icon-prescription::before{
 content:""; }

.bp3-icon-presentation::before{
 content:""; }

.bp3-icon-print::before{
 content:"⎙"; }

.bp3-icon-projects::before{
 content:""; }

.bp3-icon-properties::before{
 content:""; }

.bp3-icon-property::before{
 content:""; }

.bp3-icon-publish-function::before{
 content:""; }

.bp3-icon-pulse::before{
 content:""; }

.bp3-icon-random::before{
 content:""; }

.bp3-icon-record::before{
 content:""; }

.bp3-icon-redo::before{
 content:""; }

.bp3-icon-refresh::before{
 content:""; }

.bp3-icon-regression-chart::before{
 content:""; }

.bp3-icon-remove::before{
 content:""; }

.bp3-icon-remove-column::before{
 content:""; }

.bp3-icon-remove-column-left::before{
 content:""; }

.bp3-icon-remove-column-right::before{
 content:""; }

.bp3-icon-remove-row-bottom::before{
 content:""; }

.bp3-icon-remove-row-top::before{
 content:""; }

.bp3-icon-repeat::before{
 content:""; }

.bp3-icon-reset::before{
 content:""; }

.bp3-icon-resolve::before{
 content:""; }

.bp3-icon-rig::before{
 content:""; }

.bp3-icon-right-join::before{
 content:""; }

.bp3-icon-ring::before{
 content:""; }

.bp3-icon-rotate-document::before{
 content:""; }

.bp3-icon-rotate-page::before{
 content:""; }

.bp3-icon-satellite::before{
 content:""; }

.bp3-icon-saved::before{
 content:""; }

.bp3-icon-scatter-plot::before{
 content:""; }

.bp3-icon-search::before{
 content:""; }

.bp3-icon-search-around::before{
 content:""; }

.bp3-icon-search-template::before{
 content:""; }

.bp3-icon-search-text::before{
 content:""; }

.bp3-icon-segmented-control::before{
 content:""; }

.bp3-icon-select::before{
 content:""; }

.bp3-icon-selection::before{
 content:"⦿"; }

.bp3-icon-send-to::before{
 content:""; }

.bp3-icon-send-to-graph::before{
 content:""; }

.bp3-icon-send-to-map::before{
 content:""; }

.bp3-icon-series-add::before{
 content:""; }

.bp3-icon-series-configuration::before{
 content:""; }

.bp3-icon-series-derived::before{
 content:""; }

.bp3-icon-series-filtered::before{
 content:""; }

.bp3-icon-series-search::before{
 content:""; }

.bp3-icon-settings::before{
 content:""; }

.bp3-icon-share::before{
 content:""; }

.bp3-icon-shield::before{
 content:""; }

.bp3-icon-shop::before{
 content:""; }

.bp3-icon-shopping-cart::before{
 content:""; }

.bp3-icon-signal-search::before{
 content:""; }

.bp3-icon-sim-card::before{
 content:""; }

.bp3-icon-slash::before{
 content:""; }

.bp3-icon-small-cross::before{
 content:""; }

.bp3-icon-small-minus::before{
 content:""; }

.bp3-icon-small-plus::before{
 content:""; }

.bp3-icon-small-tick::before{
 content:""; }

.bp3-icon-snowflake::before{
 content:""; }

.bp3-icon-social-media::before{
 content:""; }

.bp3-icon-sort::before{
 content:""; }

.bp3-icon-sort-alphabetical::before{
 content:""; }

.bp3-icon-sort-alphabetical-desc::before{
 content:""; }

.bp3-icon-sort-asc::before{
 content:""; }

.bp3-icon-sort-desc::before{
 content:""; }

.bp3-icon-sort-numerical::before{
 content:""; }

.bp3-icon-sort-numerical-desc::before{
 content:""; }

.bp3-icon-split-columns::before{
 content:""; }

.bp3-icon-square::before{
 content:""; }

.bp3-icon-stacked-chart::before{
 content:""; }

.bp3-icon-star::before{
 content:"★"; }

.bp3-icon-star-empty::before{
 content:"☆"; }

.bp3-icon-step-backward::before{
 content:""; }

.bp3-icon-step-chart::before{
 content:""; }

.bp3-icon-step-forward::before{
 content:""; }

.bp3-icon-stop::before{
 content:""; }

.bp3-icon-stopwatch::before{
 content:""; }

.bp3-icon-strikethrough::before{
 content:""; }

.bp3-icon-style::before{
 content:""; }

.bp3-icon-swap-horizontal::before{
 content:""; }

.bp3-icon-swap-vertical::before{
 content:""; }

.bp3-icon-symbol-circle::before{
 content:""; }

.bp3-icon-symbol-cross::before{
 content:""; }

.bp3-icon-symbol-diamond::before{
 content:""; }

.bp3-icon-symbol-square::before{
 content:""; }

.bp3-icon-symbol-triangle-down::before{
 content:""; }

.bp3-icon-symbol-triangle-up::before{
 content:""; }

.bp3-icon-tag::before{
 content:""; }

.bp3-icon-take-action::before{
 content:""; }

.bp3-icon-taxi::before{
 content:""; }

.bp3-icon-text-highlight::before{
 content:""; }

.bp3-icon-th::before{
 content:""; }

.bp3-icon-th-derived::before{
 content:""; }

.bp3-icon-th-disconnect::before{
 content:""; }

.bp3-icon-th-filtered::before{
 content:""; }

.bp3-icon-th-list::before{
 content:""; }

.bp3-icon-thumbs-down::before{
 content:""; }

.bp3-icon-thumbs-up::before{
 content:""; }

.bp3-icon-tick::before{
 content:"✓"; }

.bp3-icon-tick-circle::before{
 content:""; }

.bp3-icon-time::before{
 content:"⏲"; }

.bp3-icon-timeline-area-chart::before{
 content:""; }

.bp3-icon-timeline-bar-chart::before{
 content:""; }

.bp3-icon-timeline-events::before{
 content:""; }

.bp3-icon-timeline-line-chart::before{
 content:""; }

.bp3-icon-tint::before{
 content:""; }

.bp3-icon-torch::before{
 content:""; }

.bp3-icon-tractor::before{
 content:""; }

.bp3-icon-train::before{
 content:""; }

.bp3-icon-translate::before{
 content:""; }

.bp3-icon-trash::before{
 content:""; }

.bp3-icon-tree::before{
 content:""; }

.bp3-icon-trending-down::before{
 content:""; }

.bp3-icon-trending-up::before{
 content:""; }

.bp3-icon-truck::before{
 content:""; }

.bp3-icon-two-columns::before{
 content:""; }

.bp3-icon-unarchive::before{
 content:""; }

.bp3-icon-underline::before{
 content:"⎁"; }

.bp3-icon-undo::before{
 content:"⎌"; }

.bp3-icon-ungroup-objects::before{
 content:""; }

.bp3-icon-unknown-vehicle::before{
 content:""; }

.bp3-icon-unlock::before{
 content:""; }

.bp3-icon-unpin::before{
 content:""; }

.bp3-icon-unresolve::before{
 content:""; }

.bp3-icon-updated::before{
 content:""; }

.bp3-icon-upload::before{
 content:""; }

.bp3-icon-user::before{
 content:""; }

.bp3-icon-variable::before{
 content:""; }

.bp3-icon-vertical-bar-chart-asc::before{
 content:""; }

.bp3-icon-vertical-bar-chart-desc::before{
 content:""; }

.bp3-icon-vertical-distribution::before{
 content:""; }

.bp3-icon-video::before{
 content:""; }

.bp3-icon-volume-down::before{
 content:""; }

.bp3-icon-volume-off::before{
 content:""; }

.bp3-icon-volume-up::before{
 content:""; }

.bp3-icon-walk::before{
 content:""; }

.bp3-icon-warning-sign::before{
 content:""; }

.bp3-icon-waterfall-chart::before{
 content:""; }

.bp3-icon-widget::before{
 content:""; }

.bp3-icon-widget-button::before{
 content:""; }

.bp3-icon-widget-footer::before{
 content:""; }

.bp3-icon-widget-header::before{
 content:""; }

.bp3-icon-wrench::before{
 content:""; }

.bp3-icon-zoom-in::before{
 content:""; }

.bp3-icon-zoom-out::before{
 content:""; }

.bp3-icon-zoom-to-fit::before{
 content:""; }
.bp3-submenu > .bp3-popover-wrapper{
 display:block; }

.bp3-submenu .bp3-popover-target{
 display:block; }
 .bp3-submenu .bp3-popover-target.bp3-popover-open > .bp3-menu-item{ }

.bp3-submenu.bp3-popover{
 -webkit-box-shadow:none;
 box-shadow:none;
 padding:0 5px; }
 .bp3-submenu.bp3-popover > .bp3-popover-content{
 -webkit-box-shadow:0 0 0 1px rgba(16, 22, 26, 0.1), 0 2px 4px rgba(16, 22, 26, 0.2), 0 8px 24px rgba(16, 22, 26, 0.2);
 box-shadow:0 0 0 1px rgba(16, 22, 26, 0.1), 0 2px 4px rgba(16, 22, 26, 0.2), 0 8px 24px rgba(16, 22, 26, 0.2); }
 .bp3-dark .bp3-submenu.bp3-popover, .bp3-submenu.bp3-popover.bp3-dark{
 -webkit-box-shadow:none;
 box-shadow:none; }
 .bp3-dark .bp3-submenu.bp3-popover > .bp3-popover-content, .bp3-submenu.bp3-popover.bp3-dark > .bp3-popover-content{
 -webkit-box-shadow:0 0 0 1px rgba(16, 22, 26, 0.2), 0 2px 4px rgba(16, 22, 26, 0.4), 0 8px 24px rgba(16, 22, 26, 0.4);
 box-shadow:0 0 0 1px rgba(16, 22, 26, 0.2), 0 2px 4px rgba(16, 22, 26, 0.4), 0 8px 24px rgba(16, 22, 26, 0.4); }
.bp3-menu{
 background:#ffffff;
 border-radius:3px;
 color:#182026;
 list-style:none;
 margin:0;
 min-width:180px;
 padding:5px;
 text-align:left; }

.bp3-menu-divider{
 border-top:1px solid rgba(16, 22, 26, 0.15);
 display:block;
 margin:5px; }
 .bp3-dark .bp3-menu-divider{
 border-top-color:rgba(255, 255, 255, 0.15); }

.bp3-menu-item{
 display:-webkit-box;
 display:-ms-flexbox;
 display:flex;
 -webkit-box-orient:horizontal;
 -webkit-box-direction:normal;
 -ms-flex-direction:row;
 flex-direction:row;
 -webkit-box-align:start;
 -ms-flex-align:start;
 align-items:flex-start;
 border-radius:2px;
 color:inherit;
 line-height:20px;
 padding:5px 7px;
 text-decoration:none;
 -webkit-user-select:none;
 -moz-user-select:none;
 -ms-user-select:none;
 user-select:none; }
 .bp3-menu-item > \*{
 -webkit-box-flex:0;
 -ms-flex-positive:0;
 flex-grow:0;
 -ms-flex-negative:0;
 flex-shrink:0; }
 .bp3-menu-item > .bp3-fill{
 -webkit-box-flex:1;
 -ms-flex-positive:1;
 flex-grow:1;
 -ms-flex-negative:1;
 flex-shrink:1; }
 .bp3-menu-item::before,
 .bp3-menu-item > \*{
 margin-right:7px; }
 .bp3-menu-item:empty::before,
 .bp3-menu-item > :last-child{
 margin-right:0; }
 .bp3-menu-item > .bp3-fill{
 word-break:break-word; }
 .bp3-menu-item:hover, .bp3-submenu .bp3-popover-target.bp3-popover-open > .bp3-menu-item{
 background-color:rgba(167, 182, 194, 0.3);
 cursor:pointer;
 text-decoration:none; }
 .bp3-menu-item.bp3-disabled{
 background-color:inherit;
 color:rgba(92, 112, 128, 0.6);
 cursor:not-allowed; }
 .bp3-dark .bp3-menu-item{
 color:inherit; }
 .bp3-dark .bp3-menu-item:hover, .bp3-dark .bp3-submenu .bp3-popover-target.bp3-popover-open > .bp3-menu-item, .bp3-submenu .bp3-dark .bp3-popover-target.bp3-popover-open > .bp3-menu-item{
 background-color:rgba(138, 155, 168, 0.15);
 color:inherit; }
 .bp3-dark .bp3-menu-item.bp3-disabled{
 background-color:inherit;
 color:rgba(167, 182, 194, 0.6); }
 .bp3-menu-item.bp3-intent-primary{
 color:#106ba3; }
 .bp3-menu-item.bp3-intent-primary .bp3-icon{
 color:inherit; }
 .bp3-menu-item.bp3-intent-primary::before, .bp3-menu-item.bp3-intent-primary::after,
 .bp3-menu-item.bp3-intent-primary .bp3-menu-item-label{
 color:#106ba3; }
 .bp3-menu-item.bp3-intent-primary:hover, .bp3-submenu .bp3-popover-target.bp3-popover-open > .bp3-intent-primary.bp3-menu-item, .bp3-menu-item.bp3-intent-primary.bp3-active{
 background-color:#137cbd; }
 .bp3-menu-item.bp3-intent-primary:active{
 background-color:#106ba3; }
 .bp3-menu-item.bp3-intent-primary:hover, .bp3-submenu .bp3-popover-target.bp3-popover-open > .bp3-intent-primary.bp3-menu-item, .bp3-menu-item.bp3-intent-primary:hover::before, .bp3-submenu .bp3-popover-target.bp3-popover-open > .bp3-intent-primary.bp3-menu-item::before, .bp3-menu-item.bp3-intent-primary:hover::after, .bp3-submenu .bp3-popover-target.bp3-popover-open > .bp3-intent-primary.bp3-menu-item::after,
 .bp3-menu-item.bp3-intent-primary:hover .bp3-menu-item-label,
 .bp3-submenu .bp3-popover-target.bp3-popover-open > .bp3-intent-primary.bp3-menu-item .bp3-menu-item-label, .bp3-menu-item.bp3-intent-primary:active, .bp3-menu-item.bp3-intent-primary:active::before, .bp3-menu-item.bp3-intent-primary:active::after,
 .bp3-menu-item.bp3-intent-primary:active .bp3-menu-item-label, .bp3-menu-item.bp3-intent-primary.bp3-active, .bp3-menu-item.bp3-intent-primary.bp3-active::before, .bp3-menu-item.bp3-intent-primary.bp3-active::after,
 .bp3-menu-item.bp3-intent-primary.bp3-active .bp3-menu-item-label{
 color:#ffffff; }
 .bp3-menu-item.bp3-intent-success{
 color:#0d8050; }
 .bp3-menu-item.bp3-intent-success .bp3-icon{
 color:inherit; }
 .bp3-menu-item.bp3-intent-success::before, .bp3-menu-item.bp3-intent-success::after,
 .bp3-menu-item.bp3-intent-success .bp3-menu-item-label{
 color:#0d8050; }
 .bp3-menu-item.bp3-intent-success:hover, .bp3-submenu .bp3-popover-target.bp3-popover-open > .bp3-intent-success.bp3-menu-item, .bp3-menu-item.bp3-intent-success.bp3-active{
 background-color:#0f9960; }
 .bp3-menu-item.bp3-intent-success:active{
 background-color:#0d8050; }
 .bp3-menu-item.bp3-intent-success:hover, .bp3-submenu .bp3-popover-target.bp3-popover-open > .bp3-intent-success.bp3-menu-item, .bp3-menu-item.bp3-intent-success:hover::before, .bp3-submenu .bp3-popover-target.bp3-popover-open > .bp3-intent-success.bp3-menu-item::before, .bp3-menu-item.bp3-intent-success:hover::after, .bp3-submenu .bp3-popover-target.bp3-popover-open > .bp3-intent-success.bp3-menu-item::after,
 .bp3-menu-item.bp3-intent-success:hover .bp3-menu-item-label,
 .bp3-submenu .bp3-popover-target.bp3-popover-open > .bp3-intent-success.bp3-menu-item .bp3-menu-item-label, .bp3-menu-item.bp3-intent-success:active, .bp3-menu-item.bp3-intent-success:active::before, .bp3-menu-item.bp3-intent-success:active::after,
 .bp3-menu-item.bp3-intent-success:active .bp3-menu-item-label, .bp3-menu-item.bp3-intent-success.bp3-active, .bp3-menu-item.bp3-intent-success.bp3-active::before, .bp3-menu-item.bp3-intent-success.bp3-active::after,
 .bp3-menu-item.bp3-intent-success.bp3-active .bp3-menu-item-label{
 color:#ffffff; }
 .bp3-menu-item.bp3-intent-warning{
 color:#bf7326; }
 .bp3-menu-item.bp3-intent-warning .bp3-icon{
 color:inherit; }
 .bp3-menu-item.bp3-intent-warning::before, .bp3-menu-item.bp3-intent-warning::after,
 .bp3-menu-item.bp3-intent-warning .bp3-menu-item-label{
 color:#bf7326; }
 .bp3-menu-item.bp3-intent-warning:hover, .bp3-submenu .bp3-popover-target.bp3-popover-open > .bp3-intent-warning.bp3-menu-item, .bp3-menu-item.bp3-intent-warning.bp3-active{
 background-color:#d9822b; }
 .bp3-menu-item.bp3-intent-warning:active{
 background-color:#bf7326; }
 .bp3-menu-item.bp3-intent-warning:hover, .bp3-submenu .bp3-popover-target.bp3-popover-open > .bp3-intent-warning.bp3-menu-item, .bp3-menu-item.bp3-intent-warning:hover::before, .bp3-submenu .bp3-popover-target.bp3-popover-open > .bp3-intent-warning.bp3-menu-item::before, .bp3-menu-item.bp3-intent-warning:hover::after, .bp3-submenu .bp3-popover-target.bp3-popover-open > .bp3-intent-warning.bp3-menu-item::after,
 .bp3-menu-item.bp3-intent-warning:hover .bp3-menu-item-label,
 .bp3-submenu .bp3-popover-target.bp3-popover-open > .bp3-intent-warning.bp3-menu-item .bp3-menu-item-label, .bp3-menu-item.bp3-intent-warning:active, .bp3-menu-item.bp3-intent-warning:active::before, .bp3-menu-item.bp3-intent-warning:active::after,
 .bp3-menu-item.bp3-intent-warning:active .bp3-menu-item-label, .bp3-menu-item.bp3-intent-warning.bp3-active, .bp3-menu-item.bp3-intent-warning.bp3-active::before, .bp3-menu-item.bp3-intent-warning.bp3-active::after,
 .bp3-menu-item.bp3-intent-warning.bp3-active .bp3-menu-item-label{
 color:#ffffff; }
 .bp3-menu-item.bp3-intent-danger{
 color:#c23030; }
 .bp3-menu-item.bp3-intent-danger .bp3-icon{
 color:inherit; }
 .bp3-menu-item.bp3-intent-danger::before, .bp3-menu-item.bp3-intent-danger::after,
 .bp3-menu-item.bp3-intent-danger .bp3-menu-item-label{
 color:#c23030; }
 .bp3-menu-item.bp3-intent-danger:hover, .bp3-submenu .bp3-popover-target.bp3-popover-open > .bp3-intent-danger.bp3-menu-item, .bp3-menu-item.bp3-intent-danger.bp3-active{
 background-color:#db3737; }
 .bp3-menu-item.bp3-intent-danger:active{
 background-color:#c23030; }
 .bp3-menu-item.bp3-intent-danger:hover, .bp3-submenu .bp3-popover-target.bp3-popover-open > .bp3-intent-danger.bp3-menu-item, .bp3-menu-item.bp3-intent-danger:hover::before, .bp3-submenu .bp3-popover-target.bp3-popover-open > .bp3-intent-danger.bp3-menu-item::before, .bp3-menu-item.bp3-intent-danger:hover::after, .bp3-submenu .bp3-popover-target.bp3-popover-open > .bp3-intent-danger.bp3-menu-item::after,
 .bp3-menu-item.bp3-intent-danger:hover .bp3-menu-item-label,
 .bp3-submenu .bp3-popover-target.bp3-popover-open > .bp3-intent-danger.bp3-menu-item .bp3-menu-item-label, .bp3-menu-item.bp3-intent-danger:active, .bp3-menu-item.bp3-intent-danger:active::before, .bp3-menu-item.bp3-intent-danger:active::after,
 .bp3-menu-item.bp3-intent-danger:active .bp3-menu-item-label, .bp3-menu-item.bp3-intent-danger.bp3-active, .bp3-menu-item.bp3-intent-danger.bp3-active::before, .bp3-menu-item.bp3-intent-danger.bp3-active::after,
 .bp3-menu-item.bp3-intent-danger.bp3-active .bp3-menu-item-label{
 color:#ffffff; }
 .bp3-menu-item::before{
 font-family:"Icons16", sans-serif;
 font-size:16px;
 font-style:normal;
 font-weight:400;
 line-height:1;
 -moz-osx-font-smoothing:grayscale;
 -webkit-font-smoothing:antialiased;
 margin-right:7px; }
 .bp3-menu-item::before,
 .bp3-menu-item > .bp3-icon{
 color:#5c7080;
 margin-top:2px; }
 .bp3-menu-item .bp3-menu-item-label{
 color:#5c7080; }
 .bp3-menu-item:hover, .bp3-submenu .bp3-popover-target.bp3-popover-open > .bp3-menu-item{
 color:inherit; }
 .bp3-menu-item.bp3-active, .bp3-menu-item:active{
 background-color:rgba(115, 134, 148, 0.3); }
 .bp3-menu-item.bp3-disabled{
 background-color:inherit !important;
 color:rgba(92, 112, 128, 0.6) !important;
 cursor:not-allowed !important;
 outline:none !important; }
 .bp3-menu-item.bp3-disabled::before,
 .bp3-menu-item.bp3-disabled > .bp3-icon,
 .bp3-menu-item.bp3-disabled .bp3-menu-item-label{
 color:rgba(92, 112, 128, 0.6) !important; }
 .bp3-large .bp3-menu-item{
 font-size:16px;
 line-height:22px;
 padding:9px 7px; }
 .bp3-large .bp3-menu-item .bp3-icon{
 margin-top:3px; }
 .bp3-large .bp3-menu-item::before{
 font-family:"Icons20", sans-serif;
 font-size:20px;
 font-style:normal;
 font-weight:400;
 line-height:1;
 -moz-osx-font-smoothing:grayscale;
 -webkit-font-smoothing:antialiased;
 margin-right:10px;
 margin-top:1px; }

button.bp3-menu-item{
 background:none;
 border:none;
 text-align:left;
 width:100%; }
.bp3-menu-header{
 border-top:1px solid rgba(16, 22, 26, 0.15);
 display:block;
 margin:5px;
 cursor:default;
 padding-left:2px; }
 .bp3-dark .bp3-menu-header{
 border-top-color:rgba(255, 255, 255, 0.15); }
 .bp3-menu-header:first-of-type{
 border-top:none; }
 .bp3-menu-header > h6{
 color:#182026;
 font-weight:600;
 overflow:hidden;
 text-overflow:ellipsis;
 white-space:nowrap;
 word-wrap:normal;
 line-height:17px;
 margin:0;
 padding:10px 7px 0 1px; }
 .bp3-dark .bp3-menu-header > h6{
 color:#f5f8fa; }
 .bp3-menu-header:first-of-type > h6{
 padding-top:0; }
 .bp3-large .bp3-menu-header > h6{
 font-size:18px;
 padding-bottom:5px;
 padding-top:15px; }
 .bp3-large .bp3-menu-header:first-of-type > h6{
 padding-top:0; }

.bp3-dark .bp3-menu{
 background:#30404d;
 color:#f5f8fa; }

.bp3-dark .bp3-menu-item{ }
 .bp3-dark .bp3-menu-item.bp3-intent-primary{
 color:#48aff0; }
 .bp3-dark .bp3-menu-item.bp3-intent-primary .bp3-icon{
 color:inherit; }
 .bp3-dark .bp3-menu-item.bp3-intent-primary::before, .bp3-dark .bp3-menu-item.bp3-intent-primary::after,
 .bp3-dark .bp3-menu-item.bp3-intent-primary .bp3-menu-item-label{
 color:#48aff0; }
 .bp3-dark .bp3-menu-item.bp3-intent-primary:hover, .bp3-dark .bp3-submenu .bp3-popover-target.bp3-popover-open > .bp3-intent-primary.bp3-menu-item, .bp3-submenu .bp3-dark .bp3-popover-target.bp3-popover-open > .bp3-intent-primary.bp3-menu-item, .bp3-dark .bp3-menu-item.bp3-intent-primary.bp3-active{
 background-color:#137cbd; }
 .bp3-dark .bp3-menu-item.bp3-intent-primary:active{
 background-color:#106ba3; }
 .bp3-dark .bp3-menu-item.bp3-intent-primary:hover, .bp3-dark .bp3-submenu .bp3-popover-target.bp3-popover-open > .bp3-intent-primary.bp3-menu-item, .bp3-submenu .bp3-dark .bp3-popover-target.bp3-popover-open > .bp3-intent-primary.bp3-menu-item, .bp3-dark .bp3-menu-item.bp3-intent-primary:hover::before, .bp3-dark .bp3-submenu .bp3-popover-target.bp3-popover-open > .bp3-intent-primary.bp3-menu-item::before, .bp3-submenu .bp3-dark .bp3-popover-target.bp3-popover-open > .bp3-intent-primary.bp3-menu-item::before, .bp3-dark .bp3-menu-item.bp3-intent-primary:hover::after, .bp3-dark .bp3-submenu .bp3-popover-target.bp3-popover-open > .bp3-intent-primary.bp3-menu-item::after, .bp3-submenu .bp3-dark .bp3-popover-target.bp3-popover-open > .bp3-intent-primary.bp3-menu-item::after,
 .bp3-dark .bp3-menu-item.bp3-intent-primary:hover .bp3-menu-item-label,
 .bp3-dark .bp3-submenu .bp3-popover-target.bp3-popover-open > .bp3-intent-primary.bp3-menu-item .bp3-menu-item-label,
 .bp3-submenu .bp3-dark .bp3-popover-target.bp3-popover-open > .bp3-intent-primary.bp3-menu-item .bp3-menu-item-label, .bp3-dark .bp3-menu-item.bp3-intent-primary:active, .bp3-dark .bp3-menu-item.bp3-intent-primary:active::before, .bp3-dark .bp3-menu-item.bp3-intent-primary:active::after,
 .bp3-dark .bp3-menu-item.bp3-intent-primary:active .bp3-menu-item-label, .bp3-dark .bp3-menu-item.bp3-intent-primary.bp3-active, .bp3-dark .bp3-menu-item.bp3-intent-primary.bp3-active::before, .bp3-dark .bp3-menu-item.bp3-intent-primary.bp3-active::after,
 .bp3-dark .bp3-menu-item.bp3-intent-primary.bp3-active .bp3-menu-item-label{
 color:#ffffff; }
 .bp3-dark .bp3-menu-item.bp3-intent-success{
 color:#3dcc91; }
 .bp3-dark .bp3-menu-item.bp3-intent-success .bp3-icon{
 color:inherit; }
 .bp3-dark .bp3-menu-item.bp3-intent-success::before, .bp3-dark .bp3-menu-item.bp3-intent-success::after,
 .bp3-dark .bp3-menu-item.bp3-intent-success .bp3-menu-item-label{
 color:#3dcc91; }
 .bp3-dark .bp3-menu-item.bp3-intent-success:hover, .bp3-dark .bp3-submenu .bp3-popover-target.bp3-popover-open > .bp3-intent-success.bp3-menu-item, .bp3-submenu .bp3-dark .bp3-popover-target.bp3-popover-open > .bp3-intent-success.bp3-menu-item, .bp3-dark .bp3-menu-item.bp3-intent-success.bp3-active{
 background-color:#0f9960; }
 .bp3-dark .bp3-menu-item.bp3-intent-success:active{
 background-color:#0d8050; }
 .bp3-dark .bp3-menu-item.bp3-intent-success:hover, .bp3-dark .bp3-submenu .bp3-popover-target.bp3-popover-open > .bp3-intent-success.bp3-menu-item, .bp3-submenu .bp3-dark .bp3-popover-target.bp3-popover-open > .bp3-intent-success.bp3-menu-item, .bp3-dark .bp3-menu-item.bp3-intent-success:hover::before, .bp3-dark .bp3-submenu .bp3-popover-target.bp3-popover-open > .bp3-intent-success.bp3-menu-item::before, .bp3-submenu .bp3-dark .bp3-popover-target.bp3-popover-open > .bp3-intent-success.bp3-menu-item::before, .bp3-dark .bp3-menu-item.bp3-intent-success:hover::after, .bp3-dark .bp3-submenu .bp3-popover-target.bp3-popover-open > .bp3-intent-success.bp3-menu-item::after, .bp3-submenu .bp3-dark .bp3-popover-target.bp3-popover-open > .bp3-intent-success.bp3-menu-item::after,
 .bp3-dark .bp3-menu-item.bp3-intent-success:hover .bp3-menu-item-label,
 .bp3-dark .bp3-submenu .bp3-popover-target.bp3-popover-open > .bp3-intent-success.bp3-menu-item .bp3-menu-item-label,
 .bp3-submenu .bp3-dark .bp3-popover-target.bp3-popover-open > .bp3-intent-success.bp3-menu-item .bp3-menu-item-label, .bp3-dark .bp3-menu-item.bp3-intent-success:active, .bp3-dark .bp3-menu-item.bp3-intent-success:active::before, .bp3-dark .bp3-menu-item.bp3-intent-success:active::after,
 .bp3-dark .bp3-menu-item.bp3-intent-success:active .bp3-menu-item-label, .bp3-dark .bp3-menu-item.bp3-intent-success.bp3-active, .bp3-dark .bp3-menu-item.bp3-intent-success.bp3-active::before, .bp3-dark .bp3-menu-item.bp3-intent-success.bp3-active::after,
 .bp3-dark .bp3-menu-item.bp3-intent-success.bp3-active .bp3-menu-item-label{
 color:#ffffff; }
 .bp3-dark .bp3-menu-item.bp3-intent-warning{
 color:#ffb366; }
 .bp3-dark .bp3-menu-item.bp3-intent-warning .bp3-icon{
 color:inherit; }
 .bp3-dark .bp3-menu-item.bp3-intent-warning::before, .bp3-dark .bp3-menu-item.bp3-intent-warning::after,
 .bp3-dark .bp3-menu-item.bp3-intent-warning .bp3-menu-item-label{
 color:#ffb366; }
 .bp3-dark .bp3-menu-item.bp3-intent-warning:hover, .bp3-dark .bp3-submenu .bp3-popover-target.bp3-popover-open > .bp3-intent-warning.bp3-menu-item, .bp3-submenu .bp3-dark .bp3-popover-target.bp3-popover-open > .bp3-intent-warning.bp3-menu-item, .bp3-dark .bp3-menu-item.bp3-intent-warning.bp3-active{
 background-color:#d9822b; }
 .bp3-dark .bp3-menu-item.bp3-intent-warning:active{
 background-color:#bf7326; }
 .bp3-dark .bp3-menu-item.bp3-intent-warning:hover, .bp3-dark .bp3-submenu .bp3-popover-target.bp3-popover-open > .bp3-intent-warning.bp3-menu-item, .bp3-submenu .bp3-dark .bp3-popover-target.bp3-popover-open > .bp3-intent-warning.bp3-menu-item, .bp3-dark .bp3-menu-item.bp3-intent-warning:hover::before, .bp3-dark .bp3-submenu .bp3-popover-target.bp3-popover-open > .bp3-intent-warning.bp3-menu-item::before, .bp3-submenu .bp3-dark .bp3-popover-target.bp3-popover-open > .bp3-intent-warning.bp3-menu-item::before, .bp3-dark .bp3-menu-item.bp3-intent-warning:hover::after, .bp3-dark .bp3-submenu .bp3-popover-target.bp3-popover-open > .bp3-intent-warning.bp3-menu-item::after, .bp3-submenu .bp3-dark .bp3-popover-target.bp3-popover-open > .bp3-intent-warning.bp3-menu-item::after,
 .bp3-dark .bp3-menu-item.bp3-intent-warning:hover .bp3-menu-item-label,
 .bp3-dark .bp3-submenu .bp3-popover-target.bp3-popover-open > .bp3-intent-warning.bp3-menu-item .bp3-menu-item-label,
 .bp3-submenu .bp3-dark .bp3-popover-target.bp3-popover-open > .bp3-intent-warning.bp3-menu-item .bp3-menu-item-label, .bp3-dark .bp3-menu-item.bp3-intent-warning:active, .bp3-dark .bp3-menu-item.bp3-intent-warning:active::before, .bp3-dark .bp3-menu-item.bp3-intent-warning:active::after,
 .bp3-dark .bp3-menu-item.bp3-intent-warning:active .bp3-menu-item-label, .bp3-dark .bp3-menu-item.bp3-intent-warning.bp3-active, .bp3-dark .bp3-menu-item.bp3-intent-warning.bp3-active::before, .bp3-dark .bp3-menu-item.bp3-intent-warning.bp3-active::after,
 .bp3-dark .bp3-menu-item.bp3-intent-warning.bp3-active .bp3-menu-item-label{
 color:#ffffff; }
 .bp3-dark .bp3-menu-item.bp3-intent-danger{
 color:#ff7373; }
 .bp3-dark .bp3-menu-item.bp3-intent-danger .bp3-icon{
 color:inherit; }
 .bp3-dark .bp3-menu-item.bp3-intent-danger::before, .bp3-dark .bp3-menu-item.bp3-intent-danger::after,
 .bp3-dark .bp3-menu-item.bp3-intent-danger .bp3-menu-item-label{
 color:#ff7373; }
 .bp3-dark .bp3-menu-item.bp3-intent-danger:hover, .bp3-dark .bp3-submenu .bp3-popover-target.bp3-popover-open > .bp3-intent-danger.bp3-menu-item, .bp3-submenu .bp3-dark .bp3-popover-target.bp3-popover-open > .bp3-intent-danger.bp3-menu-item, .bp3-dark .bp3-menu-item.bp3-intent-danger.bp3-active{
 background-color:#db3737; }
 .bp3-dark .bp3-menu-item.bp3-intent-danger:active{
 background-color:#c23030; }
 .bp3-dark .bp3-menu-item.bp3-intent-danger:hover, .bp3-dark .bp3-submenu .bp3-popover-target.bp3-popover-open > .bp3-intent-danger.bp3-menu-item, .bp3-submenu .bp3-dark .bp3-popover-target.bp3-popover-open > .bp3-intent-danger.bp3-menu-item, .bp3-dark .bp3-menu-item.bp3-intent-danger:hover::before, .bp3-dark .bp3-submenu .bp3-popover-target.bp3-popover-open > .bp3-intent-danger.bp3-menu-item::before, .bp3-submenu .bp3-dark .bp3-popover-target.bp3-popover-open > .bp3-intent-danger.bp3-menu-item::before, .bp3-dark .bp3-menu-item.bp3-intent-danger:hover::after, .bp3-dark .bp3-submenu .bp3-popover-target.bp3-popover-open > .bp3-intent-danger.bp3-menu-item::after, .bp3-submenu .bp3-dark .bp3-popover-target.bp3-popover-open > .bp3-intent-danger.bp3-menu-item::after,
 .bp3-dark .bp3-menu-item.bp3-intent-danger:hover .bp3-menu-item-label,
 .bp3-dark .bp3-submenu .bp3-popover-target.bp3-popover-open > .bp3-intent-danger.bp3-menu-item .bp3-menu-item-label,
 .bp3-submenu .bp3-dark .bp3-popover-target.bp3-popover-open > .bp3-intent-danger.bp3-menu-item .bp3-menu-item-label, .bp3-dark .bp3-menu-item.bp3-intent-danger:active, .bp3-dark .bp3-menu-item.bp3-intent-danger:active::before, .bp3-dark .bp3-menu-item.bp3-intent-danger:active::after,
 .bp3-dark .bp3-menu-item.bp3-intent-danger:active .bp3-menu-item-label, .bp3-dark .bp3-menu-item.bp3-intent-danger.bp3-active, .bp3-dark .bp3-menu-item.bp3-intent-danger.bp3-active::before, .bp3-dark .bp3-menu-item.bp3-intent-danger.bp3-active::after,
 .bp3-dark .bp3-menu-item.bp3-intent-danger.bp3-active .bp3-menu-item-label{
 color:#ffffff; }
 .bp3-dark .bp3-menu-item::before,
 .bp3-dark .bp3-menu-item > .bp3-icon{
 color:#a7b6c2; }
 .bp3-dark .bp3-menu-item .bp3-menu-item-label{
 color:#a7b6c2; }
 .bp3-dark .bp3-menu-item.bp3-active, .bp3-dark .bp3-menu-item:active{
 background-color:rgba(138, 155, 168, 0.3); }
 .bp3-dark .bp3-menu-item.bp3-disabled{
 color:rgba(167, 182, 194, 0.6) !important; }
 .bp3-dark .bp3-menu-item.bp3-disabled::before,
 .bp3-dark .bp3-menu-item.bp3-disabled > .bp3-icon,
 .bp3-dark .bp3-menu-item.bp3-disabled .bp3-menu-item-label{
 color:rgba(167, 182, 194, 0.6) !important; }

.bp3-dark .bp3-menu-divider,
.bp3-dark .bp3-menu-header{
 border-color:rgba(255, 255, 255, 0.15); }

.bp3-dark .bp3-menu-header > h6{
 color:#f5f8fa; }

.bp3-label .bp3-menu{
 margin-top:5px; }
.bp3-navbar{
 background-color:#ffffff;
 -webkit-box-shadow:0 0 0 1px rgba(16, 22, 26, 0.1), 0 0 0 rgba(16, 22, 26, 0), 0 1px 1px rgba(16, 22, 26, 0.2);
 box-shadow:0 0 0 1px rgba(16, 22, 26, 0.1), 0 0 0 rgba(16, 22, 26, 0), 0 1px 1px rgba(16, 22, 26, 0.2);
 height:50px;
 padding:0 15px;
 position:relative;
 width:100%;
 z-index:10; }
 .bp3-navbar.bp3-dark,
 .bp3-dark .bp3-navbar{
 background-color:#394b59; }
 .bp3-navbar.bp3-dark{
 -webkit-box-shadow:inset 0 0 0 1px rgba(16, 22, 26, 0.2), 0 0 0 rgba(16, 22, 26, 0), 0 1px 1px rgba(16, 22, 26, 0.4);
 box-shadow:inset 0 0 0 1px rgba(16, 22, 26, 0.2), 0 0 0 rgba(16, 22, 26, 0), 0 1px 1px rgba(16, 22, 26, 0.4); }
 .bp3-dark .bp3-navbar{
 -webkit-box-shadow:0 0 0 1px rgba(16, 22, 26, 0.2), 0 0 0 rgba(16, 22, 26, 0), 0 1px 1px rgba(16, 22, 26, 0.4);
 box-shadow:0 0 0 1px rgba(16, 22, 26, 0.2), 0 0 0 rgba(16, 22, 26, 0), 0 1px 1px rgba(16, 22, 26, 0.4); }
 .bp3-navbar.bp3-fixed-top{
 left:0;
 position:fixed;
 right:0;
 top:0; }

.bp3-navbar-heading{
 font-size:16px;
 margin-right:15px; }

.bp3-navbar-group{
 -webkit-box-align:center;
 -ms-flex-align:center;
 align-items:center;
 display:-webkit-box;
 display:-ms-flexbox;
 display:flex;
 height:50px; }
 .bp3-navbar-group.bp3-align-left{
 float:left; }
 .bp3-navbar-group.bp3-align-right{
 float:right; }

.bp3-navbar-divider{
 border-left:1px solid rgba(16, 22, 26, 0.15);
 height:20px;
 margin:0 10px; }
 .bp3-dark .bp3-navbar-divider{
 border-left-color:rgba(255, 255, 255, 0.15); }
.bp3-non-ideal-state{
 display:-webkit-box;
 display:-ms-flexbox;
 display:flex;
 -webkit-box-orient:vertical;
 -webkit-box-direction:normal;
 -ms-flex-direction:column;
 flex-direction:column;
 -webkit-box-align:center;
 -ms-flex-align:center;
 align-items:center;
 height:100%;
 -webkit-box-pack:center;
 -ms-flex-pack:center;
 justify-content:center;
 text-align:center;
 width:100%; }
 .bp3-non-ideal-state > \*{
 -webkit-box-flex:0;
 -ms-flex-positive:0;
 flex-grow:0;
 -ms-flex-negative:0;
 flex-shrink:0; }
 .bp3-non-ideal-state > .bp3-fill{
 -webkit-box-flex:1;
 -ms-flex-positive:1;
 flex-grow:1;
 -ms-flex-negative:1;
 flex-shrink:1; }
 .bp3-non-ideal-state::before,
 .bp3-non-ideal-state > \*{
 margin-bottom:20px; }
 .bp3-non-ideal-state:empty::before,
 .bp3-non-ideal-state > :last-child{
 margin-bottom:0; }
 .bp3-non-ideal-state > \*{
 max-width:400px; }

.bp3-non-ideal-state-visual{
 color:rgba(92, 112, 128, 0.6);
 font-size:60px; }
 .bp3-dark .bp3-non-ideal-state-visual{
 color:rgba(167, 182, 194, 0.6); }

.bp3-overflow-list{
 display:-webkit-box;
 display:-ms-flexbox;
 display:flex;
 -ms-flex-wrap:nowrap;
 flex-wrap:nowrap;
 min-width:0; }

.bp3-overflow-list-spacer{
 -ms-flex-negative:1;
 flex-shrink:1;
 width:1px; }

body.bp3-overlay-open{
 overflow:hidden; }

.bp3-overlay{
 bottom:0;
 left:0;
 position:static;
 right:0;
 top:0;
 z-index:20; }
 .bp3-overlay:not(.bp3-overlay-open){
 pointer-events:none; }
 .bp3-overlay.bp3-overlay-container{
 overflow:hidden;
 position:fixed; }
 .bp3-overlay.bp3-overlay-container.bp3-overlay-inline{
 position:absolute; }
 .bp3-overlay.bp3-overlay-scroll-container{
 overflow:auto;
 position:fixed; }
 .bp3-overlay.bp3-overlay-scroll-container.bp3-overlay-inline{
 position:absolute; }
 .bp3-overlay.bp3-overlay-inline{
 display:inline;
 overflow:visible; }

.bp3-overlay-content{
 position:fixed;
 z-index:20; }
 .bp3-overlay-inline .bp3-overlay-content,
 .bp3-overlay-scroll-container .bp3-overlay-content{
 position:absolute; }

.bp3-overlay-backdrop{
 bottom:0;
 left:0;
 position:fixed;
 right:0;
 top:0;
 opacity:1;
 background-color:rgba(16, 22, 26, 0.7);
 overflow:auto;
 -webkit-user-select:none;
 -moz-user-select:none;
 -ms-user-select:none;
 user-select:none;
 z-index:20; }
 .bp3-overlay-backdrop.bp3-overlay-enter, .bp3-overlay-backdrop.bp3-overlay-appear{
 opacity:0; }
 .bp3-overlay-backdrop.bp3-overlay-enter-active, .bp3-overlay-backdrop.bp3-overlay-appear-active{
 opacity:1;
 -webkit-transition-delay:0;
 transition-delay:0;
 -webkit-transition-duration:200ms;
 transition-duration:200ms;
 -webkit-transition-property:opacity;
 transition-property:opacity;
 -webkit-transition-timing-function:cubic-bezier(0.4, 1, 0.75, 0.9);
 transition-timing-function:cubic-bezier(0.4, 1, 0.75, 0.9); }
 .bp3-overlay-backdrop.bp3-overlay-exit{
 opacity:1; }
 .bp3-overlay-backdrop.bp3-overlay-exit-active{
 opacity:0;
 -webkit-transition-delay:0;
 transition-delay:0;
 -webkit-transition-duration:200ms;
 transition-duration:200ms;
 -webkit-transition-property:opacity;
 transition-property:opacity;
 -webkit-transition-timing-function:cubic-bezier(0.4, 1, 0.75, 0.9);
 transition-timing-function:cubic-bezier(0.4, 1, 0.75, 0.9); }
 .bp3-overlay-backdrop:focus{
 outline:none; }
 .bp3-overlay-inline .bp3-overlay-backdrop{
 position:absolute; }
.bp3-panel-stack{
 overflow:hidden;
 position:relative; }

.bp3-panel-stack-header{
 -webkit-box-align:center;
 -ms-flex-align:center;
 align-items:center;
 -webkit-box-shadow:0 1px rgba(16, 22, 26, 0.15);
 box-shadow:0 1px rgba(16, 22, 26, 0.15);
 display:-webkit-box;
 display:-ms-flexbox;
 display:flex;
 -ms-flex-negative:0;
 flex-shrink:0;
 height:30px;
 z-index:1; }
 .bp3-dark .bp3-panel-stack-header{
 -webkit-box-shadow:0 1px rgba(255, 255, 255, 0.15);
 box-shadow:0 1px rgba(255, 255, 255, 0.15); }
 .bp3-panel-stack-header > span{
 -webkit-box-align:stretch;
 -ms-flex-align:stretch;
 align-items:stretch;
 display:-webkit-box;
 display:-ms-flexbox;
 display:flex;
 -webkit-box-flex:1;
 -ms-flex:1;
 flex:1; }
 .bp3-panel-stack-header .bp3-heading{
 margin:0 5px; }

.bp3-button.bp3-panel-stack-header-back{
 margin-left:5px;
 padding-left:0;
 white-space:nowrap; }
 .bp3-button.bp3-panel-stack-header-back .bp3-icon{
 margin:0 2px; }

.bp3-panel-stack-view{
 bottom:0;
 left:0;
 position:absolute;
 right:0;
 top:0;
 background-color:#ffffff;
 border-right:1px solid rgba(16, 22, 26, 0.15);
 display:-webkit-box;
 display:-ms-flexbox;
 display:flex;
 -webkit-box-orient:vertical;
 -webkit-box-direction:normal;
 -ms-flex-direction:column;
 flex-direction:column;
 margin-right:-1px;
 overflow-y:auto;
 z-index:1; }
 .bp3-dark .bp3-panel-stack-view{
 background-color:#30404d; }
 .bp3-panel-stack-view:nth-last-child(n + 4){
 display:none; }

.bp3-panel-stack-push .bp3-panel-stack-enter, .bp3-panel-stack-push .bp3-panel-stack-appear{
 -webkit-transform:translateX(100%);
 transform:translateX(100%);
 opacity:0; }

.bp3-panel-stack-push .bp3-panel-stack-enter-active, .bp3-panel-stack-push .bp3-panel-stack-appear-active{
 -webkit-transform:translate(0%);
 transform:translate(0%);
 opacity:1;
 -webkit-transition-delay:0;
 transition-delay:0;
 -webkit-transition-duration:400ms;
 transition-duration:400ms;
 -webkit-transition-property:opacity, -webkit-transform;
 transition-property:opacity, -webkit-transform;
 transition-property:transform, opacity;
 transition-property:transform, opacity, -webkit-transform;
 -webkit-transition-timing-function:ease;
 transition-timing-function:ease; }

.bp3-panel-stack-push .bp3-panel-stack-exit{
 -webkit-transform:translate(0%);
 transform:translate(0%);
 opacity:1; }

.bp3-panel-stack-push .bp3-panel-stack-exit-active{
 -webkit-transform:translateX(-50%);
 transform:translateX(-50%);
 opacity:0;
 -webkit-transition-delay:0;
 transition-delay:0;
 -webkit-transition-duration:400ms;
 transition-duration:400ms;
 -webkit-transition-property:opacity, -webkit-transform;
 transition-property:opacity, -webkit-transform;
 transition-property:transform, opacity;
 transition-property:transform, opacity, -webkit-transform;
 -webkit-transition-timing-function:ease;
 transition-timing-function:ease; }

.bp3-panel-stack-pop .bp3-panel-stack-enter, .bp3-panel-stack-pop .bp3-panel-stack-appear{
 -webkit-transform:translateX(-50%);
 transform:translateX(-50%);
 opacity:0; }

.bp3-panel-stack-pop .bp3-panel-stack-enter-active, .bp3-panel-stack-pop .bp3-panel-stack-appear-active{
 -webkit-transform:translate(0%);
 transform:translate(0%);
 opacity:1;
 -webkit-transition-delay:0;
 transition-delay:0;
 -webkit-transition-duration:400ms;
 transition-duration:400ms;
 -webkit-transition-property:opacity, -webkit-transform;
 transition-property:opacity, -webkit-transform;
 transition-property:transform, opacity;
 transition-property:transform, opacity, -webkit-transform;
 -webkit-transition-timing-function:ease;
 transition-timing-function:ease; }

.bp3-panel-stack-pop .bp3-panel-stack-exit{
 -webkit-transform:translate(0%);
 transform:translate(0%);
 opacity:1; }

.bp3-panel-stack-pop .bp3-panel-stack-exit-active{
 -webkit-transform:translateX(100%);
 transform:translateX(100%);
 opacity:0;
 -webkit-transition-delay:0;
 transition-delay:0;
 -webkit-transition-duration:400ms;
 transition-duration:400ms;
 -webkit-transition-property:opacity, -webkit-transform;
 transition-property:opacity, -webkit-transform;
 transition-property:transform, opacity;
 transition-property:transform, opacity, -webkit-transform;
 -webkit-transition-timing-function:ease;
 transition-timing-function:ease; }
.bp3-panel-stack2{
 overflow:hidden;
 position:relative; }

.bp3-panel-stack2-header{
 -webkit-box-align:center;
 -ms-flex-align:center;
 align-items:center;
 -webkit-box-shadow:0 1px rgba(16, 22, 26, 0.15);
 box-shadow:0 1px rgba(16, 22, 26, 0.15);
 display:-webkit-box;
 display:-ms-flexbox;
 display:flex;
 -ms-flex-negative:0;
 flex-shrink:0;
 height:30px;
 z-index:1; }
 .bp3-dark .bp3-panel-stack2-header{
 -webkit-box-shadow:0 1px rgba(255, 255, 255, 0.15);
 box-shadow:0 1px rgba(255, 255, 255, 0.15); }
 .bp3-panel-stack2-header > span{
 -webkit-box-align:stretch;
 -ms-flex-align:stretch;
 align-items:stretch;
 display:-webkit-box;
 display:-ms-flexbox;
 display:flex;
 -webkit-box-flex:1;
 -ms-flex:1;
 flex:1; }
 .bp3-panel-stack2-header .bp3-heading{
 margin:0 5px; }

.bp3-button.bp3-panel-stack2-header-back{
 margin-left:5px;
 padding-left:0;
 white-space:nowrap; }
 .bp3-button.bp3-panel-stack2-header-back .bp3-icon{
 margin:0 2px; }

.bp3-panel-stack2-view{
 bottom:0;
 left:0;
 position:absolute;
 right:0;
 top:0;
 background-color:#ffffff;
 border-right:1px solid rgba(16, 22, 26, 0.15);
 display:-webkit-box;
 display:-ms-flexbox;
 display:flex;
 -webkit-box-orient:vertical;
 -webkit-box-direction:normal;
 -ms-flex-direction:column;
 flex-direction:column;
 margin-right:-1px;
 overflow-y:auto;
 z-index:1; }
 .bp3-dark .bp3-panel-stack2-view{
 background-color:#30404d; }
 .bp3-panel-stack2-view:nth-last-child(n + 4){
 display:none; }

.bp3-panel-stack2-push .bp3-panel-stack2-enter, .bp3-panel-stack2-push .bp3-panel-stack2-appear{
 -webkit-transform:translateX(100%);
 transform:translateX(100%);
 opacity:0; }

.bp3-panel-stack2-push .bp3-panel-stack2-enter-active, .bp3-panel-stack2-push .bp3-panel-stack2-appear-active{
 -webkit-transform:translate(0%);
 transform:translate(0%);
 opacity:1;
 -webkit-transition-delay:0;
 transition-delay:0;
 -webkit-transition-duration:400ms;
 transition-duration:400ms;
 -webkit-transition-property:opacity, -webkit-transform;
 transition-property:opacity, -webkit-transform;
 transition-property:transform, opacity;
 transition-property:transform, opacity, -webkit-transform;
 -webkit-transition-timing-function:ease;
 transition-timing-function:ease; }

.bp3-panel-stack2-push .bp3-panel-stack2-exit{
 -webkit-transform:translate(0%);
 transform:translate(0%);
 opacity:1; }

.bp3-panel-stack2-push .bp3-panel-stack2-exit-active{
 -webkit-transform:translateX(-50%);
 transform:translateX(-50%);
 opacity:0;
 -webkit-transition-delay:0;
 transition-delay:0;
 -webkit-transition-duration:400ms;
 transition-duration:400ms;
 -webkit-transition-property:opacity, -webkit-transform;
 transition-property:opacity, -webkit-transform;
 transition-property:transform, opacity;
 transition-property:transform, opacity, -webkit-transform;
 -webkit-transition-timing-function:ease;
 transition-timing-function:ease; }

.bp3-panel-stack2-pop .bp3-panel-stack2-enter, .bp3-panel-stack2-pop .bp3-panel-stack2-appear{
 -webkit-transform:translateX(-50%);
 transform:translateX(-50%);
 opacity:0; }

.bp3-panel-stack2-pop .bp3-panel-stack2-enter-active, .bp3-panel-stack2-pop .bp3-panel-stack2-appear-active{
 -webkit-transform:translate(0%);
 transform:translate(0%);
 opacity:1;
 -webkit-transition-delay:0;
 transition-delay:0;
 -webkit-transition-duration:400ms;
 transition-duration:400ms;
 -webkit-transition-property:opacity, -webkit-transform;
 transition-property:opacity, -webkit-transform;
 transition-property:transform, opacity;
 transition-property:transform, opacity, -webkit-transform;
 -webkit-transition-timing-function:ease;
 transition-timing-function:ease; }

.bp3-panel-stack2-pop .bp3-panel-stack2-exit{
 -webkit-transform:translate(0%);
 transform:translate(0%);
 opacity:1; }

.bp3-panel-stack2-pop .bp3-panel-stack2-exit-active{
 -webkit-transform:translateX(100%);
 transform:translateX(100%);
 opacity:0;
 -webkit-transition-delay:0;
 transition-delay:0;
 -webkit-transition-duration:400ms;
 transition-duration:400ms;
 -webkit-transition-property:opacity, -webkit-transform;
 transition-property:opacity, -webkit-transform;
 transition-property:transform, opacity;
 transition-property:transform, opacity, -webkit-transform;
 -webkit-transition-timing-function:ease;
 transition-timing-function:ease; }
.bp3-popover{
 -webkit-box-shadow:0 0 0 1px rgba(16, 22, 26, 0.1), 0 2px 4px rgba(16, 22, 26, 0.2), 0 8px 24px rgba(16, 22, 26, 0.2);
 box-shadow:0 0 0 1px rgba(16, 22, 26, 0.1), 0 2px 4px rgba(16, 22, 26, 0.2), 0 8px 24px rgba(16, 22, 26, 0.2);
 -webkit-transform:scale(1);
 transform:scale(1);
 border-radius:3px;
 display:inline-block;
 z-index:20; }
 .bp3-popover .bp3-popover-arrow{
 height:30px;
 position:absolute;
 width:30px; }
 .bp3-popover .bp3-popover-arrow::before{
 height:20px;
 margin:5px;
 width:20px; }
 .bp3-tether-element-attached-bottom.bp3-tether-target-attached-top > .bp3-popover{
 margin-bottom:17px;
 margin-top:-17px; }
 .bp3-tether-element-attached-bottom.bp3-tether-target-attached-top > .bp3-popover > .bp3-popover-arrow{
 bottom:-11px; }
 .bp3-tether-element-attached-bottom.bp3-tether-target-attached-top > .bp3-popover > .bp3-popover-arrow svg{
 -webkit-transform:rotate(-90deg);
 transform:rotate(-90deg); }
 .bp3-tether-element-attached-left.bp3-tether-target-attached-right > .bp3-popover{
 margin-left:17px; }
 .bp3-tether-element-attached-left.bp3-tether-target-attached-right > .bp3-popover > .bp3-popover-arrow{
 left:-11px; }
 .bp3-tether-element-attached-left.bp3-tether-target-attached-right > .bp3-popover > .bp3-popover-arrow svg{
 -webkit-transform:rotate(0);
 transform:rotate(0); }
 .bp3-tether-element-attached-top.bp3-tether-target-attached-bottom > .bp3-popover{
 margin-top:17px; }
 .bp3-tether-element-attached-top.bp3-tether-target-attached-bottom > .bp3-popover > .bp3-popover-arrow{
 top:-11px; }
 .bp3-tether-element-attached-top.bp3-tether-target-attached-bottom > .bp3-popover > .bp3-popover-arrow svg{
 -webkit-transform:rotate(90deg);
 transform:rotate(90deg); }
 .bp3-tether-element-attached-right.bp3-tether-target-attached-left > .bp3-popover{
 margin-left:-17px;
 margin-right:17px; }
 .bp3-tether-element-attached-right.bp3-tether-target-attached-left > .bp3-popover > .bp3-popover-arrow{
 right:-11px; }
 .bp3-tether-element-attached-right.bp3-tether-target-attached-left > .bp3-popover > .bp3-popover-arrow svg{
 -webkit-transform:rotate(180deg);
 transform:rotate(180deg); }
 .bp3-tether-element-attached-middle > .bp3-popover > .bp3-popover-arrow{
 top:50%;
 -webkit-transform:translateY(-50%);
 transform:translateY(-50%); }
 .bp3-tether-element-attached-center > .bp3-popover > .bp3-popover-arrow{
 right:50%;
 -webkit-transform:translateX(50%);
 transform:translateX(50%); }
 .bp3-tether-element-attached-top.bp3-tether-target-attached-top > .bp3-popover > .bp3-popover-arrow{
 top:-0.3934px; }
 .bp3-tether-element-attached-right.bp3-tether-target-attached-right > .bp3-popover > .bp3-popover-arrow{
 right:-0.3934px; }
 .bp3-tether-element-attached-left.bp3-tether-target-attached-left > .bp3-popover > .bp3-popover-arrow{
 left:-0.3934px; }
 .bp3-tether-element-attached-bottom.bp3-tether-target-attached-bottom > .bp3-popover > .bp3-popover-arrow{
 bottom:-0.3934px; }
 .bp3-tether-element-attached-top.bp3-tether-element-attached-left > .bp3-popover{
 -webkit-transform-origin:top left;
 transform-origin:top left; }
 .bp3-tether-element-attached-top.bp3-tether-element-attached-center > .bp3-popover{
 -webkit-transform-origin:top center;
 transform-origin:top center; }
 .bp3-tether-element-attached-top.bp3-tether-element-attached-right > .bp3-popover{
 -webkit-transform-origin:top right;
 transform-origin:top right; }
 .bp3-tether-element-attached-middle.bp3-tether-element-attached-left > .bp3-popover{
 -webkit-transform-origin:center left;
 transform-origin:center left; }
 .bp3-tether-element-attached-middle.bp3-tether-element-attached-center > .bp3-popover{
 -webkit-transform-origin:center center;
 transform-origin:center center; }
 .bp3-tether-element-attached-middle.bp3-tether-element-attached-right > .bp3-popover{
 -webkit-transform-origin:center right;
 transform-origin:center right; }
 .bp3-tether-element-attached-bottom.bp3-tether-element-attached-left > .bp3-popover{
 -webkit-transform-origin:bottom left;
 transform-origin:bottom left; }
 .bp3-tether-element-attached-bottom.bp3-tether-element-attached-center > .bp3-popover{
 -webkit-transform-origin:bottom center;
 transform-origin:bottom center; }
 .bp3-tether-element-attached-bottom.bp3-tether-element-attached-right > .bp3-popover{
 -webkit-transform-origin:bottom right;
 transform-origin:bottom right; }
 .bp3-popover .bp3-popover-content{
 background:#ffffff;
 color:inherit; }
 .bp3-popover .bp3-popover-arrow::before{
 -webkit-box-shadow:1px 1px 6px rgba(16, 22, 26, 0.2);
 box-shadow:1px 1px 6px rgba(16, 22, 26, 0.2); }
 .bp3-popover .bp3-popover-arrow-border{
 fill:#10161a;
 fill-opacity:0.1; }
 .bp3-popover .bp3-popover-arrow-fill{
 fill:#ffffff; }
 .bp3-popover-enter > .bp3-popover, .bp3-popover-appear > .bp3-popover{
 -webkit-transform:scale(0.3);
 transform:scale(0.3); }
 .bp3-popover-enter-active > .bp3-popover, .bp3-popover-appear-active > .bp3-popover{
 -webkit-transform:scale(1);
 transform:scale(1);
 -webkit-transition-delay:0;
 transition-delay:0;
 -webkit-transition-duration:300ms;
 transition-duration:300ms;
 -webkit-transition-property:-webkit-transform;
 transition-property:-webkit-transform;
 transition-property:transform;
 transition-property:transform, -webkit-transform;
 -webkit-transition-timing-function:cubic-bezier(0.54, 1.12, 0.38, 1.11);
 transition-timing-function:cubic-bezier(0.54, 1.12, 0.38, 1.11); }
 .bp3-popover-exit > .bp3-popover{
 -webkit-transform:scale(1);
 transform:scale(1); }
 .bp3-popover-exit-active > .bp3-popover{
 -webkit-transform:scale(0.3);
 transform:scale(0.3);
 -webkit-transition-delay:0;
 transition-delay:0;
 -webkit-transition-duration:300ms;
 transition-duration:300ms;
 -webkit-transition-property:-webkit-transform;
 transition-property:-webkit-transform;
 transition-property:transform;
 transition-property:transform, -webkit-transform;
 -webkit-transition-timing-function:cubic-bezier(0.54, 1.12, 0.38, 1.11);
 transition-timing-function:cubic-bezier(0.54, 1.12, 0.38, 1.11); }
 .bp3-popover .bp3-popover-content{
 border-radius:3px;
 position:relative; }
 .bp3-popover.bp3-popover-content-sizing .bp3-popover-content{
 max-width:350px;
 padding:20px; }
 .bp3-popover-target + .bp3-overlay .bp3-popover.bp3-popover-content-sizing{
 width:350px; }
 .bp3-popover.bp3-minimal{
 margin:0 !important; }
 .bp3-popover.bp3-minimal .bp3-popover-arrow{
 display:none; }
 .bp3-popover.bp3-minimal.bp3-popover{
 -webkit-transform:scale(1);
 transform:scale(1); }
 .bp3-popover-enter > .bp3-popover.bp3-minimal.bp3-popover, .bp3-popover-appear > .bp3-popover.bp3-minimal.bp3-popover{
 -webkit-transform:scale(1);
 transform:scale(1); }
 .bp3-popover-enter-active > .bp3-popover.bp3-minimal.bp3-popover, .bp3-popover-appear-active > .bp3-popover.bp3-minimal.bp3-popover{
 -webkit-transform:scale(1);
 transform:scale(1);
 -webkit-transition-delay:0;
 transition-delay:0;
 -webkit-transition-duration:100ms;
 transition-duration:100ms;
 -webkit-transition-property:-webkit-transform;
 transition-property:-webkit-transform;
 transition-property:transform;
 transition-property:transform, -webkit-transform;
 -webkit-transition-timing-function:cubic-bezier(0.4, 1, 0.75, 0.9);
 transition-timing-function:cubic-bezier(0.4, 1, 0.75, 0.9); }
 .bp3-popover-exit > .bp3-popover.bp3-minimal.bp3-popover{
 -webkit-transform:scale(1);
 transform:scale(1); }
 .bp3-popover-exit-active > .bp3-popover.bp3-minimal.bp3-popover{
 -webkit-transform:scale(1);
 transform:scale(1);
 -webkit-transition-delay:0;
 transition-delay:0;
 -webkit-transition-duration:100ms;
 transition-duration:100ms;
 -webkit-transition-property:-webkit-transform;
 transition-property:-webkit-transform;
 transition-property:transform;
 transition-property:transform, -webkit-transform;
 -webkit-transition-timing-function:cubic-bezier(0.4, 1, 0.75, 0.9);
 transition-timing-function:cubic-bezier(0.4, 1, 0.75, 0.9); }
 .bp3-popover.bp3-dark,
 .bp3-dark .bp3-popover{
 -webkit-box-shadow:0 0 0 1px rgba(16, 22, 26, 0.2), 0 2px 4px rgba(16, 22, 26, 0.4), 0 8px 24px rgba(16, 22, 26, 0.4);
 box-shadow:0 0 0 1px rgba(16, 22, 26, 0.2), 0 2px 4px rgba(16, 22, 26, 0.4), 0 8px 24px rgba(16, 22, 26, 0.4); }
 .bp3-popover.bp3-dark .bp3-popover-content,
 .bp3-dark .bp3-popover .bp3-popover-content{
 background:#30404d;
 color:inherit; }
 .bp3-popover.bp3-dark .bp3-popover-arrow::before,
 .bp3-dark .bp3-popover .bp3-popover-arrow::before{
 -webkit-box-shadow:1px 1px 6px rgba(16, 22, 26, 0.4);
 box-shadow:1px 1px 6px rgba(16, 22, 26, 0.4); }
 .bp3-popover.bp3-dark .bp3-popover-arrow-border,
 .bp3-dark .bp3-popover .bp3-popover-arrow-border{
 fill:#10161a;
 fill-opacity:0.2; }
 .bp3-popover.bp3-dark .bp3-popover-arrow-fill,
 .bp3-dark .bp3-popover .bp3-popover-arrow-fill{
 fill:#30404d; }

.bp3-popover-arrow::before{
 border-radius:2px;
 content:"";
 display:block;
 position:absolute;
 -webkit-transform:rotate(45deg);
 transform:rotate(45deg); }

.bp3-tether-pinned .bp3-popover-arrow{
 display:none; }

.bp3-popover-backdrop{
 background:rgba(255, 255, 255, 0); }

.bp3-transition-container{
 opacity:1;
 display:-webkit-box;
 display:-ms-flexbox;
 display:flex;
 z-index:20; }
 .bp3-transition-container.bp3-popover-enter, .bp3-transition-container.bp3-popover-appear{
 opacity:0; }
 .bp3-transition-container.bp3-popover-enter-active, .bp3-transition-container.bp3-popover-appear-active{
 opacity:1;
 -webkit-transition-delay:0;
 transition-delay:0;
 -webkit-transition-duration:100ms;
 transition-duration:100ms;
 -webkit-transition-property:opacity;
 transition-property:opacity;
 -webkit-transition-timing-function:cubic-bezier(0.4, 1, 0.75, 0.9);
 transition-timing-function:cubic-bezier(0.4, 1, 0.75, 0.9); }
 .bp3-transition-container.bp3-popover-exit{
 opacity:1; }
 .bp3-transition-container.bp3-popover-exit-active{
 opacity:0;
 -webkit-transition-delay:0;
 transition-delay:0;
 -webkit-transition-duration:100ms;
 transition-duration:100ms;
 -webkit-transition-property:opacity;
 transition-property:opacity;
 -webkit-transition-timing-function:cubic-bezier(0.4, 1, 0.75, 0.9);
 transition-timing-function:cubic-bezier(0.4, 1, 0.75, 0.9); }
 .bp3-transition-container:focus{
 outline:none; }
 .bp3-transition-container.bp3-popover-leave .bp3-popover-content{
 pointer-events:none; }
 .bp3-transition-container[data-x-out-of-boundaries]{
 display:none; }

span.bp3-popover-target{
 display:inline-block; }

.bp3-popover-wrapper.bp3-fill{
 width:100%; }

.bp3-portal{
 left:0;
 position:absolute;
 right:0;
 top:0; }
@-webkit-keyframes linear-progress-bar-stripes{
 from{
 background-position:0 0; }
 to{
 background-position:30px 0; } }
@keyframes linear-progress-bar-stripes{
 from{
 background-position:0 0; }
 to{
 background-position:30px 0; } }

.bp3-progress-bar{
 background:rgba(92, 112, 128, 0.2);
 border-radius:40px;
 display:block;
 height:8px;
 overflow:hidden;
 position:relative;
 width:100%; }
 .bp3-progress-bar .bp3-progress-meter{
 background:linear-gradient(-45deg, rgba(255, 255, 255, 0.2) 25%, transparent 25%, transparent 50%, rgba(255, 255, 255, 0.2) 50%, rgba(255, 255, 255, 0.2) 75%, transparent 75%);
 background-color:rgba(92, 112, 128, 0.8);
 background-size:30px 30px;
 border-radius:40px;
 height:100%;
 position:absolute;
 -webkit-transition:width 200ms cubic-bezier(0.4, 1, 0.75, 0.9);
 transition:width 200ms cubic-bezier(0.4, 1, 0.75, 0.9);
 width:100%; }
 .bp3-progress-bar:not(.bp3-no-animation):not(.bp3-no-stripes) .bp3-progress-meter{
 animation:linear-progress-bar-stripes 300ms linear infinite reverse; }
 .bp3-progress-bar.bp3-no-stripes .bp3-progress-meter{
 background-image:none; }

.bp3-dark .bp3-progress-bar{
 background:rgba(16, 22, 26, 0.5); }
 .bp3-dark .bp3-progress-bar .bp3-progress-meter{
 background-color:#8a9ba8; }

.bp3-progress-bar.bp3-intent-primary .bp3-progress-meter{
 background-color:#137cbd; }

.bp3-progress-bar.bp3-intent-success .bp3-progress-meter{
 background-color:#0f9960; }

.bp3-progress-bar.bp3-intent-warning .bp3-progress-meter{
 background-color:#d9822b; }

.bp3-progress-bar.bp3-intent-danger .bp3-progress-meter{
 background-color:#db3737; }
@-webkit-keyframes skeleton-glow{
 from{
 background:rgba(206, 217, 224, 0.2);
 border-color:rgba(206, 217, 224, 0.2); }
 to{
 background:rgba(92, 112, 128, 0.2);
 border-color:rgba(92, 112, 128, 0.2); } }
@keyframes skeleton-glow{
 from{
 background:rgba(206, 217, 224, 0.2);
 border-color:rgba(206, 217, 224, 0.2); }
 to{
 background:rgba(92, 112, 128, 0.2);
 border-color:rgba(92, 112, 128, 0.2); } }
.bp3-skeleton{
 -webkit-animation:1000ms linear infinite alternate skeleton-glow;
 animation:1000ms linear infinite alternate skeleton-glow;
 background:rgba(206, 217, 224, 0.2);
 background-clip:padding-box !important;
 border-color:rgba(206, 217, 224, 0.2) !important;
 border-radius:2px;
 -webkit-box-shadow:none !important;
 box-shadow:none !important;
 color:transparent !important;
 cursor:default;
 pointer-events:none;
 -webkit-user-select:none;
 -moz-user-select:none;
 -ms-user-select:none;
 user-select:none; }
 .bp3-skeleton::before, .bp3-skeleton::after,
 .bp3-skeleton \*{
 visibility:hidden !important; }
.bp3-slider{
 height:40px;
 min-width:150px;
 width:100%;
 cursor:default;
 outline:none;
 position:relative;
 -webkit-user-select:none;
 -moz-user-select:none;
 -ms-user-select:none;
 user-select:none; }
 .bp3-slider:hover{
 cursor:pointer; }
 .bp3-slider:active{
 cursor:-webkit-grabbing;
 cursor:grabbing; }
 .bp3-slider.bp3-disabled{
 cursor:not-allowed;
 opacity:0.5; }
 .bp3-slider.bp3-slider-unlabeled{
 height:16px; }

.bp3-slider-track,
.bp3-slider-progress{
 height:6px;
 left:0;
 right:0;
 top:5px;
 position:absolute; }

.bp3-slider-track{
 border-radius:3px;
 overflow:hidden; }

.bp3-slider-progress{
 background:rgba(92, 112, 128, 0.2); }
 .bp3-dark .bp3-slider-progress{
 background:rgba(16, 22, 26, 0.5); }
 .bp3-slider-progress.bp3-intent-primary{
 background-color:#137cbd; }
 .bp3-slider-progress.bp3-intent-success{
 background-color:#0f9960; }
 .bp3-slider-progress.bp3-intent-warning{
 background-color:#d9822b; }
 .bp3-slider-progress.bp3-intent-danger{
 background-color:#db3737; }

.bp3-slider-handle{
 background-color:#f5f8fa;
 background-image:-webkit-gradient(linear, left top, left bottom, from(rgba(255, 255, 255, 0.8)), to(rgba(255, 255, 255, 0)));
 background-image:linear-gradient(to bottom, rgba(255, 255, 255, 0.8), rgba(255, 255, 255, 0));
 -webkit-box-shadow:inset 0 0 0 1px rgba(16, 22, 26, 0.2), inset 0 -1px 0 rgba(16, 22, 26, 0.1);
 box-shadow:inset 0 0 0 1px rgba(16, 22, 26, 0.2), inset 0 -1px 0 rgba(16, 22, 26, 0.1);
 color:#182026;
 border-radius:3px;
 -webkit-box-shadow:0 0 0 1px rgba(16, 22, 26, 0.2), 0 1px 1px rgba(16, 22, 26, 0.2);
 box-shadow:0 0 0 1px rgba(16, 22, 26, 0.2), 0 1px 1px rgba(16, 22, 26, 0.2);
 cursor:pointer;
 height:16px;
 left:0;
 position:absolute;
 top:0;
 width:16px; }
 .bp3-slider-handle:hover{
 background-clip:padding-box;
 background-color:#ebf1f5;
 -webkit-box-shadow:inset 0 0 0 1px rgba(16, 22, 26, 0.2), inset 0 -1px 0 rgba(16, 22, 26, 0.1);
 box-shadow:inset 0 0 0 1px rgba(16, 22, 26, 0.2), inset 0 -1px 0 rgba(16, 22, 26, 0.1); }
 .bp3-slider-handle:active, .bp3-slider-handle.bp3-active{
 background-color:#d8e1e8;
 background-image:none;
 -webkit-box-shadow:inset 0 0 0 1px rgba(16, 22, 26, 0.2), inset 0 1px 2px rgba(16, 22, 26, 0.2);
 box-shadow:inset 0 0 0 1px rgba(16, 22, 26, 0.2), inset 0 1px 2px rgba(16, 22, 26, 0.2); }
 .bp3-slider-handle:disabled, .bp3-slider-handle.bp3-disabled{
 background-color:rgba(206, 217, 224, 0.5);
 background-image:none;
 -webkit-box-shadow:none;
 box-shadow:none;
 color:rgba(92, 112, 128, 0.6);
 cursor:not-allowed;
 outline:none; }
 .bp3-slider-handle:disabled.bp3-active, .bp3-slider-handle:disabled.bp3-active:hover, .bp3-slider-handle.bp3-disabled.bp3-active, .bp3-slider-handle.bp3-disabled.bp3-active:hover{
 background:rgba(206, 217, 224, 0.7); }
 .bp3-slider-handle:focus{
 z-index:1; }
 .bp3-slider-handle:hover{
 background-clip:padding-box;
 background-color:#ebf1f5;
 -webkit-box-shadow:inset 0 0 0 1px rgba(16, 22, 26, 0.2), inset 0 -1px 0 rgba(16, 22, 26, 0.1);
 box-shadow:inset 0 0 0 1px rgba(16, 22, 26, 0.2), inset 0 -1px 0 rgba(16, 22, 26, 0.1);
 -webkit-box-shadow:0 0 0 1px rgba(16, 22, 26, 0.2), 0 1px 1px rgba(16, 22, 26, 0.2);
 box-shadow:0 0 0 1px rgba(16, 22, 26, 0.2), 0 1px 1px rgba(16, 22, 26, 0.2);
 cursor:-webkit-grab;
 cursor:grab;
 z-index:2; }
 .bp3-slider-handle.bp3-active{
 background-color:#d8e1e8;
 background-image:none;
 -webkit-box-shadow:inset 0 0 0 1px rgba(16, 22, 26, 0.2), inset 0 1px 2px rgba(16, 22, 26, 0.2);
 box-shadow:inset 0 0 0 1px rgba(16, 22, 26, 0.2), inset 0 1px 2px rgba(16, 22, 26, 0.2);
 -webkit-box-shadow:0 0 0 1px rgba(16, 22, 26, 0.2), inset 0 1px 1px rgba(16, 22, 26, 0.1);
 box-shadow:0 0 0 1px rgba(16, 22, 26, 0.2), inset 0 1px 1px rgba(16, 22, 26, 0.1);
 cursor:-webkit-grabbing;
 cursor:grabbing; }
 .bp3-disabled .bp3-slider-handle{
 background:#bfccd6;
 -webkit-box-shadow:none;
 box-shadow:none;
 pointer-events:none; }
 .bp3-dark .bp3-slider-handle{
 background-color:#394b59;
 background-image:-webkit-gradient(linear, left top, left bottom, from(rgba(255, 255, 255, 0.05)), to(rgba(255, 255, 255, 0)));
 background-image:linear-gradient(to bottom, rgba(255, 255, 255, 0.05), rgba(255, 255, 255, 0));
 -webkit-box-shadow:0 0 0 1px rgba(16, 22, 26, 0.4);
 box-shadow:0 0 0 1px rgba(16, 22, 26, 0.4);
 color:#f5f8fa; }
 .bp3-dark .bp3-slider-handle:hover, .bp3-dark .bp3-slider-handle:active, .bp3-dark .bp3-slider-handle.bp3-active{
 color:#f5f8fa; }
 .bp3-dark .bp3-slider-handle:hover{
 background-color:#30404d;
 -webkit-box-shadow:0 0 0 1px rgba(16, 22, 26, 0.4);
 box-shadow:0 0 0 1px rgba(16, 22, 26, 0.4); }
 .bp3-dark .bp3-slider-handle:active, .bp3-dark .bp3-slider-handle.bp3-active{
 background-color:#202b33;
 background-image:none;
 -webkit-box-shadow:0 0 0 1px rgba(16, 22, 26, 0.6), inset 0 1px 2px rgba(16, 22, 26, 0.2);
 box-shadow:0 0 0 1px rgba(16, 22, 26, 0.6), inset 0 1px 2px rgba(16, 22, 26, 0.2); }
 .bp3-dark .bp3-slider-handle:disabled, .bp3-dark .bp3-slider-handle.bp3-disabled{
 background-color:rgba(57, 75, 89, 0.5);
 background-image:none;
 -webkit-box-shadow:none;
 box-shadow:none;
 color:rgba(167, 182, 194, 0.6); }
 .bp3-dark .bp3-slider-handle:disabled.bp3-active, .bp3-dark .bp3-slider-handle.bp3-disabled.bp3-active{
 background:rgba(57, 75, 89, 0.7); }
 .bp3-dark .bp3-slider-handle .bp3-button-spinner .bp3-spinner-head{
 background:rgba(16, 22, 26, 0.5);
 stroke:#8a9ba8; }
 .bp3-dark .bp3-slider-handle, .bp3-dark .bp3-slider-handle:hover{
 background-color:#394b59; }
 .bp3-dark .bp3-slider-handle.bp3-active{
 background-color:#293742; }
 .bp3-dark .bp3-disabled .bp3-slider-handle{
 background:#5c7080;
 border-color:#5c7080;
 -webkit-box-shadow:none;
 box-shadow:none; }
 .bp3-slider-handle .bp3-slider-label{
 background:#394b59;
 border-radius:3px;
 -webkit-box-shadow:0 0 0 1px rgba(16, 22, 26, 0.1), 0 2px 4px rgba(16, 22, 26, 0.2), 0 8px 24px rgba(16, 22, 26, 0.2);
 box-shadow:0 0 0 1px rgba(16, 22, 26, 0.1), 0 2px 4px rgba(16, 22, 26, 0.2), 0 8px 24px rgba(16, 22, 26, 0.2);
 color:#f5f8fa;
 margin-left:8px; }
 .bp3-dark .bp3-slider-handle .bp3-slider-label{
 background:#e1e8ed;
 -webkit-box-shadow:0 0 0 1px rgba(16, 22, 26, 0.2), 0 2px 4px rgba(16, 22, 26, 0.4), 0 8px 24px rgba(16, 22, 26, 0.4);
 box-shadow:0 0 0 1px rgba(16, 22, 26, 0.2), 0 2px 4px rgba(16, 22, 26, 0.4), 0 8px 24px rgba(16, 22, 26, 0.4);
 color:#394b59; }
 .bp3-disabled .bp3-slider-handle .bp3-slider-label{
 -webkit-box-shadow:none;
 box-shadow:none; }
 .bp3-slider-handle.bp3-start, .bp3-slider-handle.bp3-end{
 width:8px; }
 .bp3-slider-handle.bp3-start{
 border-bottom-right-radius:0;
 border-top-right-radius:0; }
 .bp3-slider-handle.bp3-end{
 border-bottom-left-radius:0;
 border-top-left-radius:0;
 margin-left:8px; }
 .bp3-slider-handle.bp3-end .bp3-slider-label{
 margin-left:0; }

.bp3-slider-label{
 -webkit-transform:translate(-50%, 20px);
 transform:translate(-50%, 20px);
 display:inline-block;
 font-size:12px;
 line-height:1;
 padding:2px 5px;
 position:absolute;
 vertical-align:top; }

.bp3-slider.bp3-vertical{
 height:150px;
 min-width:40px;
 width:40px; }
 .bp3-slider.bp3-vertical .bp3-slider-track,
 .bp3-slider.bp3-vertical .bp3-slider-progress{
 bottom:0;
 height:auto;
 left:5px;
 top:0;
 width:6px; }
 .bp3-slider.bp3-vertical .bp3-slider-progress{
 top:auto; }
 .bp3-slider.bp3-vertical .bp3-slider-label{
 -webkit-transform:translate(20px, 50%);
 transform:translate(20px, 50%); }
 .bp3-slider.bp3-vertical .bp3-slider-handle{
 top:auto; }
 .bp3-slider.bp3-vertical .bp3-slider-handle .bp3-slider-label{
 margin-left:0;
 margin-top:-8px; }
 .bp3-slider.bp3-vertical .bp3-slider-handle.bp3-end, .bp3-slider.bp3-vertical .bp3-slider-handle.bp3-start{
 height:8px;
 margin-left:0;
 width:16px; }
 .bp3-slider.bp3-vertical .bp3-slider-handle.bp3-start{
 border-bottom-right-radius:3px;
 border-top-left-radius:0; }
 .bp3-slider.bp3-vertical .bp3-slider-handle.bp3-start .bp3-slider-label{
 -webkit-transform:translate(20px);
 transform:translate(20px); }
 .bp3-slider.bp3-vertical .bp3-slider-handle.bp3-end{
 border-bottom-left-radius:0;
 border-bottom-right-radius:0;
 border-top-left-radius:3px;
 margin-bottom:8px; }

@-webkit-keyframes pt-spinner-animation{
 from{
 -webkit-transform:rotate(0deg);
 transform:rotate(0deg); }
 to{
 -webkit-transform:rotate(360deg);
 transform:rotate(360deg); } }

@keyframes pt-spinner-animation{
 from{
 -webkit-transform:rotate(0deg);
 transform:rotate(0deg); }
 to{
 -webkit-transform:rotate(360deg);
 transform:rotate(360deg); } }

.bp3-spinner{
 -webkit-box-align:center;
 -ms-flex-align:center;
 align-items:center;
 display:-webkit-box;
 display:-ms-flexbox;
 display:flex;
 -webkit-box-pack:center;
 -ms-flex-pack:center;
 justify-content:center;
 overflow:visible;
 vertical-align:middle; }
 .bp3-spinner svg{
 display:block; }
 .bp3-spinner path{
 fill-opacity:0; }
 .bp3-spinner .bp3-spinner-head{
 stroke:rgba(92, 112, 128, 0.8);
 stroke-linecap:round;
 -webkit-transform-origin:center;
 transform-origin:center;
 -webkit-transition:stroke-dashoffset 200ms cubic-bezier(0.4, 1, 0.75, 0.9);
 transition:stroke-dashoffset 200ms cubic-bezier(0.4, 1, 0.75, 0.9); }
 .bp3-spinner .bp3-spinner-track{
 stroke:rgba(92, 112, 128, 0.2); }

.bp3-spinner-animation{
 -webkit-animation:pt-spinner-animation 500ms linear infinite;
 animation:pt-spinner-animation 500ms linear infinite; }
 .bp3-no-spin > .bp3-spinner-animation{
 -webkit-animation:none;
 animation:none; }

.bp3-dark .bp3-spinner .bp3-spinner-head{
 stroke:#8a9ba8; }

.bp3-dark .bp3-spinner .bp3-spinner-track{
 stroke:rgba(16, 22, 26, 0.5); }

.bp3-spinner.bp3-intent-primary .bp3-spinner-head{
 stroke:#137cbd; }

.bp3-spinner.bp3-intent-success .bp3-spinner-head{
 stroke:#0f9960; }

.bp3-spinner.bp3-intent-warning .bp3-spinner-head{
 stroke:#d9822b; }

.bp3-spinner.bp3-intent-danger .bp3-spinner-head{
 stroke:#db3737; }
.bp3-tabs.bp3-vertical{
 display:-webkit-box;
 display:-ms-flexbox;
 display:flex; }
 .bp3-tabs.bp3-vertical > .bp3-tab-list{
 -webkit-box-align:start;
 -ms-flex-align:start;
 align-items:flex-start;
 -webkit-box-orient:vertical;
 -webkit-box-direction:normal;
 -ms-flex-direction:column;
 flex-direction:column; }
 .bp3-tabs.bp3-vertical > .bp3-tab-list .bp3-tab{
 border-radius:3px;
 padding:0 10px;
 width:100%; }
 .bp3-tabs.bp3-vertical > .bp3-tab-list .bp3-tab[aria-selected="true"]{
 background-color:rgba(19, 124, 189, 0.2);
 -webkit-box-shadow:none;
 box-shadow:none; }
 .bp3-tabs.bp3-vertical > .bp3-tab-list .bp3-tab-indicator-wrapper .bp3-tab-indicator{
 background-color:rgba(19, 124, 189, 0.2);
 border-radius:3px;
 bottom:0;
 height:auto;
 left:0;
 right:0;
 top:0; }
 .bp3-tabs.bp3-vertical > .bp3-tab-panel{
 margin-top:0;
 padding-left:20px; }

.bp3-tab-list{
 -webkit-box-align:end;
 -ms-flex-align:end;
 align-items:flex-end;
 border:none;
 display:-webkit-box;
 display:-ms-flexbox;
 display:flex;
 -webkit-box-flex:0;
 -ms-flex:0 0 auto;
 flex:0 0 auto;
 list-style:none;
 margin:0;
 padding:0;
 position:relative; }
 .bp3-tab-list > \*:not(:last-child){
 margin-right:20px; }

.bp3-tab{
 overflow:hidden;
 text-overflow:ellipsis;
 white-space:nowrap;
 word-wrap:normal;
 color:#182026;
 cursor:pointer;
 -webkit-box-flex:0;
 -ms-flex:0 0 auto;
 flex:0 0 auto;
 font-size:14px;
 line-height:30px;
 max-width:100%;
 position:relative;
 vertical-align:top; }
 .bp3-tab a{
 color:inherit;
 display:block;
 text-decoration:none; }
 .bp3-tab-indicator-wrapper ~ .bp3-tab{
 background-color:transparent !important;
 -webkit-box-shadow:none !important;
 box-shadow:none !important; }
 .bp3-tab[aria-disabled="true"]{
 color:rgba(92, 112, 128, 0.6);
 cursor:not-allowed; }
 .bp3-tab[aria-selected="true"]{
 border-radius:0;
 -webkit-box-shadow:inset 0 -3px 0 #106ba3;
 box-shadow:inset 0 -3px 0 #106ba3; }
 .bp3-tab[aria-selected="true"], .bp3-tab:not([aria-disabled="true"]):hover{
 color:#106ba3; }
 .bp3-tab:focus{
 -moz-outline-radius:0; }
 .bp3-large > .bp3-tab{
 font-size:16px;
 line-height:40px; }

.bp3-tab-panel{
 margin-top:20px; }
 .bp3-tab-panel[aria-hidden="true"]{
 display:none; }

.bp3-tab-indicator-wrapper{
 left:0;
 pointer-events:none;
 position:absolute;
 top:0;
 -webkit-transform:translateX(0), translateY(0);
 transform:translateX(0), translateY(0);
 -webkit-transition:height, width, -webkit-transform;
 transition:height, width, -webkit-transform;
 transition:height, transform, width;
 transition:height, transform, width, -webkit-transform;
 -webkit-transition-duration:200ms;
 transition-duration:200ms;
 -webkit-transition-timing-function:cubic-bezier(0.4, 1, 0.75, 0.9);
 transition-timing-function:cubic-bezier(0.4, 1, 0.75, 0.9); }
 .bp3-tab-indicator-wrapper .bp3-tab-indicator{
 background-color:#106ba3;
 bottom:0;
 height:3px;
 left:0;
 position:absolute;
 right:0; }
 .bp3-tab-indicator-wrapper.bp3-no-animation{
 -webkit-transition:none;
 transition:none; }

.bp3-dark .bp3-tab{
 color:#f5f8fa; }
 .bp3-dark .bp3-tab[aria-disabled="true"]{
 color:rgba(167, 182, 194, 0.6); }
 .bp3-dark .bp3-tab[aria-selected="true"]{
 -webkit-box-shadow:inset 0 -3px 0 #48aff0;
 box-shadow:inset 0 -3px 0 #48aff0; }
 .bp3-dark .bp3-tab[aria-selected="true"], .bp3-dark .bp3-tab:not([aria-disabled="true"]):hover{
 color:#48aff0; }

.bp3-dark .bp3-tab-indicator{
 background-color:#48aff0; }

.bp3-flex-expander{
 -webkit-box-flex:1;
 -ms-flex:1 1;
 flex:1 1; }
.bp3-tag{
 display:-webkit-inline-box;
 display:-ms-inline-flexbox;
 display:inline-flex;
 -webkit-box-orient:horizontal;
 -webkit-box-direction:normal;
 -ms-flex-direction:row;
 flex-direction:row;
 -webkit-box-align:center;
 -ms-flex-align:center;
 align-items:center;
 background-color:#5c7080;
 border:none;
 border-radius:3px;
 -webkit-box-shadow:none;
 box-shadow:none;
 color:#f5f8fa;
 font-size:12px;
 line-height:16px;
 max-width:100%;
 min-height:20px;
 min-width:20px;
 padding:2px 6px;
 position:relative; }
 .bp3-tag.bp3-interactive{
 cursor:pointer; }
 .bp3-tag.bp3-interactive:hover{
 background-color:rgba(92, 112, 128, 0.85); }
 .bp3-tag.bp3-interactive.bp3-active, .bp3-tag.bp3-interactive:active{
 background-color:rgba(92, 112, 128, 0.7); }
 .bp3-tag > \*{
 -webkit-box-flex:0;
 -ms-flex-positive:0;
 flex-grow:0;
 -ms-flex-negative:0;
 flex-shrink:0; }
 .bp3-tag > .bp3-fill{
 -webkit-box-flex:1;
 -ms-flex-positive:1;
 flex-grow:1;
 -ms-flex-negative:1;
 flex-shrink:1; }
 .bp3-tag::before,
 .bp3-tag > \*{
 margin-right:4px; }
 .bp3-tag:empty::before,
 .bp3-tag > :last-child{
 margin-right:0; }
 .bp3-tag:focus{
 outline:rgba(19, 124, 189, 0.6) auto 2px;
 outline-offset:0;
 -moz-outline-radius:6px; }
 .bp3-tag.bp3-round{
 border-radius:30px;
 padding-left:8px;
 padding-right:8px; }
 .bp3-dark .bp3-tag{
 background-color:#bfccd6;
 color:#182026; }
 .bp3-dark .bp3-tag.bp3-interactive{
 cursor:pointer; }
 .bp3-dark .bp3-tag.bp3-interactive:hover{
 background-color:rgba(191, 204, 214, 0.85); }
 .bp3-dark .bp3-tag.bp3-interactive.bp3-active, .bp3-dark .bp3-tag.bp3-interactive:active{
 background-color:rgba(191, 204, 214, 0.7); }
 .bp3-dark .bp3-tag > .bp3-icon, .bp3-dark .bp3-tag .bp3-icon-standard, .bp3-dark .bp3-tag .bp3-icon-large{
 fill:currentColor; }
 .bp3-tag > .bp3-icon, .bp3-tag .bp3-icon-standard, .bp3-tag .bp3-icon-large{
 fill:#ffffff; }
 .bp3-tag.bp3-large,
 .bp3-large .bp3-tag{
 font-size:14px;
 line-height:20px;
 min-height:30px;
 min-width:30px;
 padding:5px 10px; }
 .bp3-tag.bp3-large::before,
 .bp3-tag.bp3-large > \*,
 .bp3-large .bp3-tag::before,
 .bp3-large .bp3-tag > \*{
 margin-right:7px; }
 .bp3-tag.bp3-large:empty::before,
 .bp3-tag.bp3-large > :last-child,
 .bp3-large .bp3-tag:empty::before,
 .bp3-large .bp3-tag > :last-child{
 margin-right:0; }
 .bp3-tag.bp3-large.bp3-round,
 .bp3-large .bp3-tag.bp3-round{
 padding-left:12px;
 padding-right:12px; }
 .bp3-tag.bp3-intent-primary{
 background:#137cbd;
 color:#ffffff; }
 .bp3-tag.bp3-intent-primary.bp3-interactive{
 cursor:pointer; }
 .bp3-tag.bp3-intent-primary.bp3-interactive:hover{
 background-color:rgba(19, 124, 189, 0.85); }
 .bp3-tag.bp3-intent-primary.bp3-interactive.bp3-active, .bp3-tag.bp3-intent-primary.bp3-interactive:active{
 background-color:rgba(19, 124, 189, 0.7); }
 .bp3-tag.bp3-intent-success{
 background:#0f9960;
 color:#ffffff; }
 .bp3-tag.bp3-intent-success.bp3-interactive{
 cursor:pointer; }
 .bp3-tag.bp3-intent-success.bp3-interactive:hover{
 background-color:rgba(15, 153, 96, 0.85); }
 .bp3-tag.bp3-intent-success.bp3-interactive.bp3-active, .bp3-tag.bp3-intent-success.bp3-interactive:active{
 background-color:rgba(15, 153, 96, 0.7); }
 .bp3-tag.bp3-intent-warning{
 background:#d9822b;
 color:#ffffff; }
 .bp3-tag.bp3-intent-warning.bp3-interactive{
 cursor:pointer; }
 .bp3-tag.bp3-intent-warning.bp3-interactive:hover{
 background-color:rgba(217, 130, 43, 0.85); }
 .bp3-tag.bp3-intent-warning.bp3-interactive.bp3-active, .bp3-tag.bp3-intent-warning.bp3-interactive:active{
 background-color:rgba(217, 130, 43, 0.7); }
 .bp3-tag.bp3-intent-danger{
 background:#db3737;
 color:#ffffff; }
 .bp3-tag.bp3-intent-danger.bp3-interactive{
 cursor:pointer; }
 .bp3-tag.bp3-intent-danger.bp3-interactive:hover{
 background-color:rgba(219, 55, 55, 0.85); }
 .bp3-tag.bp3-intent-danger.bp3-interactive.bp3-active, .bp3-tag.bp3-intent-danger.bp3-interactive:active{
 background-color:rgba(219, 55, 55, 0.7); }
 .bp3-tag.bp3-fill{
 display:-webkit-box;
 display:-ms-flexbox;
 display:flex;
 width:100%; }
 .bp3-tag.bp3-minimal > .bp3-icon, .bp3-tag.bp3-minimal .bp3-icon-standard, .bp3-tag.bp3-minimal .bp3-icon-large{
 fill:#5c7080; }
 .bp3-tag.bp3-minimal:not([class\*="bp3-intent-"]){
 background-color:rgba(138, 155, 168, 0.2);
 color:#182026; }
 .bp3-tag.bp3-minimal:not([class\*="bp3-intent-"]).bp3-interactive{
 cursor:pointer; }
 .bp3-tag.bp3-minimal:not([class\*="bp3-intent-"]).bp3-interactive:hover{
 background-color:rgba(92, 112, 128, 0.3); }
 .bp3-tag.bp3-minimal:not([class\*="bp3-intent-"]).bp3-interactive.bp3-active, .bp3-tag.bp3-minimal:not([class\*="bp3-intent-"]).bp3-interactive:active{
 background-color:rgba(92, 112, 128, 0.4); }
 .bp3-dark .bp3-tag.bp3-minimal:not([class\*="bp3-intent-"]){
 color:#f5f8fa; }
 .bp3-dark .bp3-tag.bp3-minimal:not([class\*="bp3-intent-"]).bp3-interactive{
 cursor:pointer; }
 .bp3-dark .bp3-tag.bp3-minimal:not([class\*="bp3-intent-"]).bp3-interactive:hover{
 background-color:rgba(191, 204, 214, 0.3); }
 .bp3-dark .bp3-tag.bp3-minimal:not([class\*="bp3-intent-"]).bp3-interactive.bp3-active, .bp3-dark .bp3-tag.bp3-minimal:not([class\*="bp3-intent-"]).bp3-interactive:active{
 background-color:rgba(191, 204, 214, 0.4); }
 .bp3-dark .bp3-tag.bp3-minimal:not([class\*="bp3-intent-"]) > .bp3-icon, .bp3-dark .bp3-tag.bp3-minimal:not([class\*="bp3-intent-"]) .bp3-icon-standard, .bp3-dark .bp3-tag.bp3-minimal:not([class\*="bp3-intent-"]) .bp3-icon-large{
 fill:#a7b6c2; }
 .bp3-tag.bp3-minimal.bp3-intent-primary{
 background-color:rgba(19, 124, 189, 0.15);
 color:#106ba3; }
 .bp3-tag.bp3-minimal.bp3-intent-primary.bp3-interactive{
 cursor:pointer; }
 .bp3-tag.bp3-minimal.bp3-intent-primary.bp3-interactive:hover{
 background-color:rgba(19, 124, 189, 0.25); }
 .bp3-tag.bp3-minimal.bp3-intent-primary.bp3-interactive.bp3-active, .bp3-tag.bp3-minimal.bp3-intent-primary.bp3-interactive:active{
 background-color:rgba(19, 124, 189, 0.35); }
 .bp3-tag.bp3-minimal.bp3-intent-primary > .bp3-icon, .bp3-tag.bp3-minimal.bp3-intent-primary .bp3-icon-standard, .bp3-tag.bp3-minimal.bp3-intent-primary .bp3-icon-large{
 fill:#137cbd; }
 .bp3-dark .bp3-tag.bp3-minimal.bp3-intent-primary{
 background-color:rgba(19, 124, 189, 0.25);
 color:#48aff0; }
 .bp3-dark .bp3-tag.bp3-minimal.bp3-intent-primary.bp3-interactive{
 cursor:pointer; }
 .bp3-dark .bp3-tag.bp3-minimal.bp3-intent-primary.bp3-interactive:hover{
 background-color:rgba(19, 124, 189, 0.35); }
 .bp3-dark .bp3-tag.bp3-minimal.bp3-intent-primary.bp3-interactive.bp3-active, .bp3-dark .bp3-tag.bp3-minimal.bp3-intent-primary.bp3-interactive:active{
 background-color:rgba(19, 124, 189, 0.45); }
 .bp3-tag.bp3-minimal.bp3-intent-success{
 background-color:rgba(15, 153, 96, 0.15);
 color:#0d8050; }
 .bp3-tag.bp3-minimal.bp3-intent-success.bp3-interactive{
 cursor:pointer; }
 .bp3-tag.bp3-minimal.bp3-intent-success.bp3-interactive:hover{
 background-color:rgba(15, 153, 96, 0.25); }
 .bp3-tag.bp3-minimal.bp3-intent-success.bp3-interactive.bp3-active, .bp3-tag.bp3-minimal.bp3-intent-success.bp3-interactive:active{
 background-color:rgba(15, 153, 96, 0.35); }
 .bp3-tag.bp3-minimal.bp3-intent-success > .bp3-icon, .bp3-tag.bp3-minimal.bp3-intent-success .bp3-icon-standard, .bp3-tag.bp3-minimal.bp3-intent-success .bp3-icon-large{
 fill:#0f9960; }
 .bp3-dark .bp3-tag.bp3-minimal.bp3-intent-success{
 background-color:rgba(15, 153, 96, 0.25);
 color:#3dcc91; }
 .bp3-dark .bp3-tag.bp3-minimal.bp3-intent-success.bp3-interactive{
 cursor:pointer; }
 .bp3-dark .bp3-tag.bp3-minimal.bp3-intent-success.bp3-interactive:hover{
 background-color:rgba(15, 153, 96, 0.35); }
 .bp3-dark .bp3-tag.bp3-minimal.bp3-intent-success.bp3-interactive.bp3-active, .bp3-dark .bp3-tag.bp3-minimal.bp3-intent-success.bp3-interactive:active{
 background-color:rgba(15, 153, 96, 0.45); }
 .bp3-tag.bp3-minimal.bp3-intent-warning{
 background-color:rgba(217, 130, 43, 0.15);
 color:#bf7326; }
 .bp3-tag.bp3-minimal.bp3-intent-warning.bp3-interactive{
 cursor:pointer; }
 .bp3-tag.bp3-minimal.bp3-intent-warning.bp3-interactive:hover{
 background-color:rgba(217, 130, 43, 0.25); }
 .bp3-tag.bp3-minimal.bp3-intent-warning.bp3-interactive.bp3-active, .bp3-tag.bp3-minimal.bp3-intent-warning.bp3-interactive:active{
 background-color:rgba(217, 130, 43, 0.35); }
 .bp3-tag.bp3-minimal.bp3-intent-warning > .bp3-icon, .bp3-tag.bp3-minimal.bp3-intent-warning .bp3-icon-standard, .bp3-tag.bp3-minimal.bp3-intent-warning .bp3-icon-large{
 fill:#d9822b; }
 .bp3-dark .bp3-tag.bp3-minimal.bp3-intent-warning{
 background-color:rgba(217, 130, 43, 0.25);
 color:#ffb366; }
 .bp3-dark .bp3-tag.bp3-minimal.bp3-intent-warning.bp3-interactive{
 cursor:pointer; }
 .bp3-dark .bp3-tag.bp3-minimal.bp3-intent-warning.bp3-interactive:hover{
 background-color:rgba(217, 130, 43, 0.35); }
 .bp3-dark .bp3-tag.bp3-minimal.bp3-intent-warning.bp3-interactive.bp3-active, .bp3-dark .bp3-tag.bp3-minimal.bp3-intent-warning.bp3-interactive:active{
 background-color:rgba(217, 130, 43, 0.45); }
 .bp3-tag.bp3-minimal.bp3-intent-danger{
 background-color:rgba(219, 55, 55, 0.15);
 color:#c23030; }
 .bp3-tag.bp3-minimal.bp3-intent-danger.bp3-interactive{
 cursor:pointer; }
 .bp3-tag.bp3-minimal.bp3-intent-danger.bp3-interactive:hover{
 background-color:rgba(219, 55, 55, 0.25); }
 .bp3-tag.bp3-minimal.bp3-intent-danger.bp3-interactive.bp3-active, .bp3-tag.bp3-minimal.bp3-intent-danger.bp3-interactive:active{
 background-color:rgba(219, 55, 55, 0.35); }
 .bp3-tag.bp3-minimal.bp3-intent-danger > .bp3-icon, .bp3-tag.bp3-minimal.bp3-intent-danger .bp3-icon-standard, .bp3-tag.bp3-minimal.bp3-intent-danger .bp3-icon-large{
 fill:#db3737; }
 .bp3-dark .bp3-tag.bp3-minimal.bp3-intent-danger{
 background-color:rgba(219, 55, 55, 0.25);
 color:#ff7373; }
 .bp3-dark .bp3-tag.bp3-minimal.bp3-intent-danger.bp3-interactive{
 cursor:pointer; }
 .bp3-dark .bp3-tag.bp3-minimal.bp3-intent-danger.bp3-interactive:hover{
 background-color:rgba(219, 55, 55, 0.35); }
 .bp3-dark .bp3-tag.bp3-minimal.bp3-intent-danger.bp3-interactive.bp3-active, .bp3-dark .bp3-tag.bp3-minimal.bp3-intent-danger.bp3-interactive:active{
 background-color:rgba(219, 55, 55, 0.45); }

.bp3-tag-remove{
 background:none;
 border:none;
 color:inherit;
 cursor:pointer;
 display:-webkit-box;
 display:-ms-flexbox;
 display:flex;
 margin-bottom:-2px;
 margin-right:-6px !important;
 margin-top:-2px;
 opacity:0.5;
 padding:2px;
 padding-left:0; }
 .bp3-tag-remove:hover{
 background:none;
 opacity:0.8;
 text-decoration:none; }
 .bp3-tag-remove:active{
 opacity:1; }
 .bp3-tag-remove:empty::before{
 font-family:"Icons16", sans-serif;
 font-size:16px;
 font-style:normal;
 font-weight:400;
 line-height:1;
 -moz-osx-font-smoothing:grayscale;
 -webkit-font-smoothing:antialiased;
 content:""; }
 .bp3-large .bp3-tag-remove{
 margin-right:-10px !important;
 padding:0 5px 0 0; }
 .bp3-large .bp3-tag-remove:empty::before{
 font-family:"Icons20", sans-serif;
 font-size:20px;
 font-style:normal;
 font-weight:400;
 line-height:1; }
.bp3-tag-input{
 display:-webkit-box;
 display:-ms-flexbox;
 display:flex;
 -webkit-box-orient:horizontal;
 -webkit-box-direction:normal;
 -ms-flex-direction:row;
 flex-direction:row;
 -webkit-box-align:start;
 -ms-flex-align:start;
 align-items:flex-start;
 cursor:text;
 height:auto;
 line-height:inherit;
 min-height:30px;
 padding-left:5px;
 padding-right:0; }
 .bp3-tag-input > \*{
 -webkit-box-flex:0;
 -ms-flex-positive:0;
 flex-grow:0;
 -ms-flex-negative:0;
 flex-shrink:0; }
 .bp3-tag-input > .bp3-tag-input-values{
 -webkit-box-flex:1;
 -ms-flex-positive:1;
 flex-grow:1;
 -ms-flex-negative:1;
 flex-shrink:1; }
 .bp3-tag-input .bp3-tag-input-icon{
 color:#5c7080;
 margin-left:2px;
 margin-right:7px;
 margin-top:7px; }
 .bp3-tag-input .bp3-tag-input-values{
 display:-webkit-box;
 display:-ms-flexbox;
 display:flex;
 -webkit-box-orient:horizontal;
 -webkit-box-direction:normal;
 -ms-flex-direction:row;
 flex-direction:row;
 -webkit-box-align:center;
 -ms-flex-align:center;
 align-items:center;
 -ms-flex-item-align:stretch;
 align-self:stretch;
 -ms-flex-wrap:wrap;
 flex-wrap:wrap;
 margin-right:7px;
 margin-top:5px;
 min-width:0; }
 .bp3-tag-input .bp3-tag-input-values > \*{
 -webkit-box-flex:0;
 -ms-flex-positive:0;
 flex-grow:0;
 -ms-flex-negative:0;
 flex-shrink:0; }
 .bp3-tag-input .bp3-tag-input-values > .bp3-fill{
 -webkit-box-flex:1;
 -ms-flex-positive:1;
 flex-grow:1;
 -ms-flex-negative:1;
 flex-shrink:1; }
 .bp3-tag-input .bp3-tag-input-values::before,
 .bp3-tag-input .bp3-tag-input-values > \*{
 margin-right:5px; }
 .bp3-tag-input .bp3-tag-input-values:empty::before,
 .bp3-tag-input .bp3-tag-input-values > :last-child{
 margin-right:0; }
 .bp3-tag-input .bp3-tag-input-values:first-child .bp3-input-ghost:first-child{
 padding-left:5px; }
 .bp3-tag-input .bp3-tag-input-values > \*{
 margin-bottom:5px; }
 .bp3-tag-input .bp3-tag{
 overflow-wrap:break-word; }
 .bp3-tag-input .bp3-tag.bp3-active{
 outline:rgba(19, 124, 189, 0.6) auto 2px;
 outline-offset:0;
 -moz-outline-radius:6px; }
 .bp3-tag-input .bp3-input-ghost{
 -webkit-box-flex:1;
 -ms-flex:1 1 auto;
 flex:1 1 auto;
 line-height:20px;
 width:80px; }
 .bp3-tag-input .bp3-input-ghost:disabled, .bp3-tag-input .bp3-input-ghost.bp3-disabled{
 cursor:not-allowed; }
 .bp3-tag-input .bp3-button,
 .bp3-tag-input .bp3-spinner{
 margin:3px;
 margin-left:0; }
 .bp3-tag-input .bp3-button{
 min-height:24px;
 min-width:24px;
 padding:0 7px; }
 .bp3-tag-input.bp3-large{
 height:auto;
 min-height:40px; }
 .bp3-tag-input.bp3-large::before,
 .bp3-tag-input.bp3-large > \*{
 margin-right:10px; }
 .bp3-tag-input.bp3-large:empty::before,
 .bp3-tag-input.bp3-large > :last-child{
 margin-right:0; }
 .bp3-tag-input.bp3-large .bp3-tag-input-icon{
 margin-left:5px;
 margin-top:10px; }
 .bp3-tag-input.bp3-large .bp3-input-ghost{
 line-height:30px; }
 .bp3-tag-input.bp3-large .bp3-button{
 min-height:30px;
 min-width:30px;
 padding:5px 10px;
 margin:5px;
 margin-left:0; }
 .bp3-tag-input.bp3-large .bp3-spinner{
 margin:8px;
 margin-left:0; }
 .bp3-tag-input.bp3-active{
 background-color:#ffffff;
 -webkit-box-shadow:0 0 0 1px #137cbd, 0 0 0 3px rgba(19, 124, 189, 0.3), inset 0 1px 1px rgba(16, 22, 26, 0.2);
 box-shadow:0 0 0 1px #137cbd, 0 0 0 3px rgba(19, 124, 189, 0.3), inset 0 1px 1px rgba(16, 22, 26, 0.2); }
 .bp3-tag-input.bp3-active.bp3-intent-primary{
 -webkit-box-shadow:0 0 0 1px #106ba3, 0 0 0 3px rgba(16, 107, 163, 0.3), inset 0 1px 1px rgba(16, 22, 26, 0.2);
 box-shadow:0 0 0 1px #106ba3, 0 0 0 3px rgba(16, 107, 163, 0.3), inset 0 1px 1px rgba(16, 22, 26, 0.2); }
 .bp3-tag-input.bp3-active.bp3-intent-success{
 -webkit-box-shadow:0 0 0 1px #0d8050, 0 0 0 3px rgba(13, 128, 80, 0.3), inset 0 1px 1px rgba(16, 22, 26, 0.2);
 box-shadow:0 0 0 1px #0d8050, 0 0 0 3px rgba(13, 128, 80, 0.3), inset 0 1px 1px rgba(16, 22, 26, 0.2); }
 .bp3-tag-input.bp3-active.bp3-intent-warning{
 -webkit-box-shadow:0 0 0 1px #bf7326, 0 0 0 3px rgba(191, 115, 38, 0.3), inset 0 1px 1px rgba(16, 22, 26, 0.2);
 box-shadow:0 0 0 1px #bf7326, 0 0 0 3px rgba(191, 115, 38, 0.3), inset 0 1px 1px rgba(16, 22, 26, 0.2); }
 .bp3-tag-input.bp3-active.bp3-intent-danger{
 -webkit-box-shadow:0 0 0 1px #c23030, 0 0 0 3px rgba(194, 48, 48, 0.3), inset 0 1px 1px rgba(16, 22, 26, 0.2);
 box-shadow:0 0 0 1px #c23030, 0 0 0 3px rgba(194, 48, 48, 0.3), inset 0 1px 1px rgba(16, 22, 26, 0.2); }
 .bp3-dark .bp3-tag-input .bp3-tag-input-icon, .bp3-tag-input.bp3-dark .bp3-tag-input-icon{
 color:#a7b6c2; }
 .bp3-dark .bp3-tag-input .bp3-input-ghost, .bp3-tag-input.bp3-dark .bp3-input-ghost{
 color:#f5f8fa; }
 .bp3-dark .bp3-tag-input .bp3-input-ghost::-webkit-input-placeholder, .bp3-tag-input.bp3-dark .bp3-input-ghost::-webkit-input-placeholder{
 color:rgba(167, 182, 194, 0.6); }
 .bp3-dark .bp3-tag-input .bp3-input-ghost::-moz-placeholder, .bp3-tag-input.bp3-dark .bp3-input-ghost::-moz-placeholder{
 color:rgba(167, 182, 194, 0.6); }
 .bp3-dark .bp3-tag-input .bp3-input-ghost:-ms-input-placeholder, .bp3-tag-input.bp3-dark .bp3-input-ghost:-ms-input-placeholder{
 color:rgba(167, 182, 194, 0.6); }
 .bp3-dark .bp3-tag-input .bp3-input-ghost::-ms-input-placeholder, .bp3-tag-input.bp3-dark .bp3-input-ghost::-ms-input-placeholder{
 color:rgba(167, 182, 194, 0.6); }
 .bp3-dark .bp3-tag-input .bp3-input-ghost::placeholder, .bp3-tag-input.bp3-dark .bp3-input-ghost::placeholder{
 color:rgba(167, 182, 194, 0.6); }
 .bp3-dark .bp3-tag-input.bp3-active, .bp3-tag-input.bp3-dark.bp3-active{
 background-color:rgba(16, 22, 26, 0.3);
 -webkit-box-shadow:0 0 0 1px #137cbd, 0 0 0 1px #137cbd, 0 0 0 3px rgba(19, 124, 189, 0.3), inset 0 0 0 1px rgba(16, 22, 26, 0.3), inset 0 1px 1px rgba(16, 22, 26, 0.4);
 box-shadow:0 0 0 1px #137cbd, 0 0 0 1px #137cbd, 0 0 0 3px rgba(19, 124, 189, 0.3), inset 0 0 0 1px rgba(16, 22, 26, 0.3), inset 0 1px 1px rgba(16, 22, 26, 0.4); }
 .bp3-dark .bp3-tag-input.bp3-active.bp3-intent-primary, .bp3-tag-input.bp3-dark.bp3-active.bp3-intent-primary{
 -webkit-box-shadow:0 0 0 1px #106ba3, 0 0 0 3px rgba(16, 107, 163, 0.3), inset 0 0 0 1px rgba(16, 22, 26, 0.3), inset 0 1px 1px rgba(16, 22, 26, 0.4);
 box-shadow:0 0 0 1px #106ba3, 0 0 0 3px rgba(16, 107, 163, 0.3), inset 0 0 0 1px rgba(16, 22, 26, 0.3), inset 0 1px 1px rgba(16, 22, 26, 0.4); }
 .bp3-dark .bp3-tag-input.bp3-active.bp3-intent-success, .bp3-tag-input.bp3-dark.bp3-active.bp3-intent-success{
 -webkit-box-shadow:0 0 0 1px #0d8050, 0 0 0 3px rgba(13, 128, 80, 0.3), inset 0 0 0 1px rgba(16, 22, 26, 0.3), inset 0 1px 1px rgba(16, 22, 26, 0.4);
 box-shadow:0 0 0 1px #0d8050, 0 0 0 3px rgba(13, 128, 80, 0.3), inset 0 0 0 1px rgba(16, 22, 26, 0.3), inset 0 1px 1px rgba(16, 22, 26, 0.4); }
 .bp3-dark .bp3-tag-input.bp3-active.bp3-intent-warning, .bp3-tag-input.bp3-dark.bp3-active.bp3-intent-warning{
 -webkit-box-shadow:0 0 0 1px #bf7326, 0 0 0 3px rgba(191, 115, 38, 0.3), inset 0 0 0 1px rgba(16, 22, 26, 0.3), inset 0 1px 1px rgba(16, 22, 26, 0.4);
 box-shadow:0 0 0 1px #bf7326, 0 0 0 3px rgba(191, 115, 38, 0.3), inset 0 0 0 1px rgba(16, 22, 26, 0.3), inset 0 1px 1px rgba(16, 22, 26, 0.4); }
 .bp3-dark .bp3-tag-input.bp3-active.bp3-intent-danger, .bp3-tag-input.bp3-dark.bp3-active.bp3-intent-danger{
 -webkit-box-shadow:0 0 0 1px #c23030, 0 0 0 3px rgba(194, 48, 48, 0.3), inset 0 0 0 1px rgba(16, 22, 26, 0.3), inset 0 1px 1px rgba(16, 22, 26, 0.4);
 box-shadow:0 0 0 1px #c23030, 0 0 0 3px rgba(194, 48, 48, 0.3), inset 0 0 0 1px rgba(16, 22, 26, 0.3), inset 0 1px 1px rgba(16, 22, 26, 0.4); }

.bp3-input-ghost{
 background:none;
 border:none;
 -webkit-box-shadow:none;
 box-shadow:none;
 padding:0; }
 .bp3-input-ghost::-webkit-input-placeholder{
 color:rgba(92, 112, 128, 0.6);
 opacity:1; }
 .bp3-input-ghost::-moz-placeholder{
 color:rgba(92, 112, 128, 0.6);
 opacity:1; }
 .bp3-input-ghost:-ms-input-placeholder{
 color:rgba(92, 112, 128, 0.6);
 opacity:1; }
 .bp3-input-ghost::-ms-input-placeholder{
 color:rgba(92, 112, 128, 0.6);
 opacity:1; }
 .bp3-input-ghost::placeholder{
 color:rgba(92, 112, 128, 0.6);
 opacity:1; }
 .bp3-input-ghost:focus{
 outline:none !important; }
.bp3-toast{
 -webkit-box-align:start;
 -ms-flex-align:start;
 align-items:flex-start;
 background-color:#ffffff;
 border-radius:3px;
 -webkit-box-shadow:0 0 0 1px rgba(16, 22, 26, 0.1), 0 2px 4px rgba(16, 22, 26, 0.2), 0 8px 24px rgba(16, 22, 26, 0.2);
 box-shadow:0 0 0 1px rgba(16, 22, 26, 0.1), 0 2px 4px rgba(16, 22, 26, 0.2), 0 8px 24px rgba(16, 22, 26, 0.2);
 display:-webkit-box;
 display:-ms-flexbox;
 display:flex;
 margin:20px 0 0;
 max-width:500px;
 min-width:300px;
 pointer-events:all;
 position:relative !important; }
 .bp3-toast.bp3-toast-enter, .bp3-toast.bp3-toast-appear{
 -webkit-transform:translateY(-40px);
 transform:translateY(-40px); }
 .bp3-toast.bp3-toast-enter-active, .bp3-toast.bp3-toast-appear-active{
 -webkit-transform:translateY(0);
 transform:translateY(0);
 -webkit-transition-delay:0;
 transition-delay:0;
 -webkit-transition-duration:300ms;
 transition-duration:300ms;
 -webkit-transition-property:-webkit-transform;
 transition-property:-webkit-transform;
 transition-property:transform;
 transition-property:transform, -webkit-transform;
 -webkit-transition-timing-function:cubic-bezier(0.54, 1.12, 0.38, 1.11);
 transition-timing-function:cubic-bezier(0.54, 1.12, 0.38, 1.11); }
 .bp3-toast.bp3-toast-enter ~ .bp3-toast, .bp3-toast.bp3-toast-appear ~ .bp3-toast{
 -webkit-transform:translateY(-40px);
 transform:translateY(-40px); }
 .bp3-toast.bp3-toast-enter-active ~ .bp3-toast, .bp3-toast.bp3-toast-appear-active ~ .bp3-toast{
 -webkit-transform:translateY(0);
 transform:translateY(0);
 -webkit-transition-delay:0;
 transition-delay:0;
 -webkit-transition-duration:300ms;
 transition-duration:300ms;
 -webkit-transition-property:-webkit-transform;
 transition-property:-webkit-transform;
 transition-property:transform;
 transition-property:transform, -webkit-transform;
 -webkit-transition-timing-function:cubic-bezier(0.54, 1.12, 0.38, 1.11);
 transition-timing-function:cubic-bezier(0.54, 1.12, 0.38, 1.11); }
 .bp3-toast.bp3-toast-exit{
 opacity:1;
 -webkit-filter:blur(0);
 filter:blur(0); }
 .bp3-toast.bp3-toast-exit-active{
 opacity:0;
 -webkit-filter:blur(10px);
 filter:blur(10px);
 -webkit-transition-delay:0;
 transition-delay:0;
 -webkit-transition-duration:300ms;
 transition-duration:300ms;
 -webkit-transition-property:opacity, -webkit-filter;
 transition-property:opacity, -webkit-filter;
 transition-property:opacity, filter;
 transition-property:opacity, filter, -webkit-filter;
 -webkit-transition-timing-function:cubic-bezier(0.4, 1, 0.75, 0.9);
 transition-timing-function:cubic-bezier(0.4, 1, 0.75, 0.9); }
 .bp3-toast.bp3-toast-exit ~ .bp3-toast{
 -webkit-transform:translateY(0);
 transform:translateY(0); }
 .bp3-toast.bp3-toast-exit-active ~ .bp3-toast{
 -webkit-transform:translateY(-40px);
 transform:translateY(-40px);
 -webkit-transition-delay:50ms;
 transition-delay:50ms;
 -webkit-transition-duration:100ms;
 transition-duration:100ms;
 -webkit-transition-property:-webkit-transform;
 transition-property:-webkit-transform;
 transition-property:transform;
 transition-property:transform, -webkit-transform;
 -webkit-transition-timing-function:cubic-bezier(0.4, 1, 0.75, 0.9);
 transition-timing-function:cubic-bezier(0.4, 1, 0.75, 0.9); }
 .bp3-toast .bp3-button-group{
 -webkit-box-flex:0;
 -ms-flex:0 0 auto;
 flex:0 0 auto;
 padding:5px;
 padding-left:0; }
 .bp3-toast > .bp3-icon{
 color:#5c7080;
 margin:12px;
 margin-right:0; }
 .bp3-toast.bp3-dark,
 .bp3-dark .bp3-toast{
 background-color:#394b59;
 -webkit-box-shadow:0 0 0 1px rgba(16, 22, 26, 0.2), 0 2px 4px rgba(16, 22, 26, 0.4), 0 8px 24px rgba(16, 22, 26, 0.4);
 box-shadow:0 0 0 1px rgba(16, 22, 26, 0.2), 0 2px 4px rgba(16, 22, 26, 0.4), 0 8px 24px rgba(16, 22, 26, 0.4); }
 .bp3-toast.bp3-dark > .bp3-icon,
 .bp3-dark .bp3-toast > .bp3-icon{
 color:#a7b6c2; }
 .bp3-toast[class\*="bp3-intent-"] a{
 color:rgba(255, 255, 255, 0.7); }
 .bp3-toast[class\*="bp3-intent-"] a:hover{
 color:#ffffff; }
 .bp3-toast[class\*="bp3-intent-"] > .bp3-icon{
 color:#ffffff; }
 .bp3-toast[class\*="bp3-intent-"] .bp3-button, .bp3-toast[class\*="bp3-intent-"] .bp3-button::before,
 .bp3-toast[class\*="bp3-intent-"] .bp3-button .bp3-icon, .bp3-toast[class\*="bp3-intent-"] .bp3-button:active{
 color:rgba(255, 255, 255, 0.7) !important; }
 .bp3-toast[class\*="bp3-intent-"] .bp3-button:focus{
 outline-color:rgba(255, 255, 255, 0.5); }
 .bp3-toast[class\*="bp3-intent-"] .bp3-button:hover{
 background-color:rgba(255, 255, 255, 0.15) !important;
 color:#ffffff !important; }
 .bp3-toast[class\*="bp3-intent-"] .bp3-button:active{
 background-color:rgba(255, 255, 255, 0.3) !important;
 color:#ffffff !important; }
 .bp3-toast[class\*="bp3-intent-"] .bp3-button::after{
 background:rgba(255, 255, 255, 0.3) !important; }
 .bp3-toast.bp3-intent-primary{
 background-color:#137cbd;
 color:#ffffff; }
 .bp3-toast.bp3-intent-success{
 background-color:#0f9960;
 color:#ffffff; }
 .bp3-toast.bp3-intent-warning{
 background-color:#d9822b;
 color:#ffffff; }
 .bp3-toast.bp3-intent-danger{
 background-color:#db3737;
 color:#ffffff; }

.bp3-toast-message{
 -webkit-box-flex:1;
 -ms-flex:1 1 auto;
 flex:1 1 auto;
 padding:11px;
 word-break:break-word; }

.bp3-toast-container{
 -webkit-box-align:center;
 -ms-flex-align:center;
 align-items:center;
 display:-webkit-box !important;
 display:-ms-flexbox !important;
 display:flex !important;
 -webkit-box-orient:vertical;
 -webkit-box-direction:normal;
 -ms-flex-direction:column;
 flex-direction:column;
 left:0;
 overflow:hidden;
 padding:0 20px 20px;
 pointer-events:none;
 right:0;
 z-index:40; }
 .bp3-toast-container.bp3-toast-container-in-portal{
 position:fixed; }
 .bp3-toast-container.bp3-toast-container-inline{
 position:absolute; }
 .bp3-toast-container.bp3-toast-container-top{
 top:0; }
 .bp3-toast-container.bp3-toast-container-bottom{
 bottom:0;
 -webkit-box-orient:vertical;
 -webkit-box-direction:reverse;
 -ms-flex-direction:column-reverse;
 flex-direction:column-reverse;
 top:auto; }
 .bp3-toast-container.bp3-toast-container-left{
 -webkit-box-align:start;
 -ms-flex-align:start;
 align-items:flex-start; }
 .bp3-toast-container.bp3-toast-container-right{
 -webkit-box-align:end;
 -ms-flex-align:end;
 align-items:flex-end; }

.bp3-toast-container-bottom .bp3-toast.bp3-toast-enter:not(.bp3-toast-enter-active),
.bp3-toast-container-bottom .bp3-toast.bp3-toast-enter:not(.bp3-toast-enter-active) ~ .bp3-toast, .bp3-toast-container-bottom .bp3-toast.bp3-toast-appear:not(.bp3-toast-appear-active),
.bp3-toast-container-bottom .bp3-toast.bp3-toast-appear:not(.bp3-toast-appear-active) ~ .bp3-toast,
.bp3-toast-container-bottom .bp3-toast.bp3-toast-exit-active ~ .bp3-toast,
.bp3-toast-container-bottom .bp3-toast.bp3-toast-leave-active ~ .bp3-toast{
 -webkit-transform:translateY(60px);
 transform:translateY(60px); }
.bp3-tooltip{
 -webkit-box-shadow:0 0 0 1px rgba(16, 22, 26, 0.1), 0 2px 4px rgba(16, 22, 26, 0.2), 0 8px 24px rgba(16, 22, 26, 0.2);
 box-shadow:0 0 0 1px rgba(16, 22, 26, 0.1), 0 2px 4px rgba(16, 22, 26, 0.2), 0 8px 24px rgba(16, 22, 26, 0.2);
 -webkit-transform:scale(1);
 transform:scale(1); }
 .bp3-tooltip .bp3-popover-arrow{
 height:22px;
 position:absolute;
 width:22px; }
 .bp3-tooltip .bp3-popover-arrow::before{
 height:14px;
 margin:4px;
 width:14px; }
 .bp3-tether-element-attached-bottom.bp3-tether-target-attached-top > .bp3-tooltip{
 margin-bottom:11px;
 margin-top:-11px; }
 .bp3-tether-element-attached-bottom.bp3-tether-target-attached-top > .bp3-tooltip > .bp3-popover-arrow{
 bottom:-8px; }
 .bp3-tether-element-attached-bottom.bp3-tether-target-attached-top > .bp3-tooltip > .bp3-popover-arrow svg{
 -webkit-transform:rotate(-90deg);
 transform:rotate(-90deg); }
 .bp3-tether-element-attached-left.bp3-tether-target-attached-right > .bp3-tooltip{
 margin-left:11px; }
 .bp3-tether-element-attached-left.bp3-tether-target-attached-right > .bp3-tooltip > .bp3-popover-arrow{
 left:-8px; }
 .bp3-tether-element-attached-left.bp3-tether-target-attached-right > .bp3-tooltip > .bp3-popover-arrow svg{
 -webkit-transform:rotate(0);
 transform:rotate(0); }
 .bp3-tether-element-attached-top.bp3-tether-target-attached-bottom > .bp3-tooltip{
 margin-top:11px; }
 .bp3-tether-element-attached-top.bp3-tether-target-attached-bottom > .bp3-tooltip > .bp3-popover-arrow{
 top:-8px; }
 .bp3-tether-element-attached-top.bp3-tether-target-attached-bottom > .bp3-tooltip > .bp3-popover-arrow svg{
 -webkit-transform:rotate(90deg);
 transform:rotate(90deg); }
 .bp3-tether-element-attached-right.bp3-tether-target-attached-left > .bp3-tooltip{
 margin-left:-11px;
 margin-right:11px; }
 .bp3-tether-element-attached-right.bp3-tether-target-attached-left > .bp3-tooltip > .bp3-popover-arrow{
 right:-8px; }
 .bp3-tether-element-attached-right.bp3-tether-target-attached-left > .bp3-tooltip > .bp3-popover-arrow svg{
 -webkit-transform:rotate(180deg);
 transform:rotate(180deg); }
 .bp3-tether-element-attached-middle > .bp3-tooltip > .bp3-popover-arrow{
 top:50%;
 -webkit-transform:translateY(-50%);
 transform:translateY(-50%); }
 .bp3-tether-element-attached-center > .bp3-tooltip > .bp3-popover-arrow{
 right:50%;
 -webkit-transform:translateX(50%);
 transform:translateX(50%); }
 .bp3-tether-element-attached-top.bp3-tether-target-attached-top > .bp3-tooltip > .bp3-popover-arrow{
 top:-0.22183px; }
 .bp3-tether-element-attached-right.bp3-tether-target-attached-right > .bp3-tooltip > .bp3-popover-arrow{
 right:-0.22183px; }
 .bp3-tether-element-attached-left.bp3-tether-target-attached-left > .bp3-tooltip > .bp3-popover-arrow{
 left:-0.22183px; }
 .bp3-tether-element-attached-bottom.bp3-tether-target-attached-bottom > .bp3-tooltip > .bp3-popover-arrow{
 bottom:-0.22183px; }
 .bp3-tether-element-attached-top.bp3-tether-element-attached-left > .bp3-tooltip{
 -webkit-transform-origin:top left;
 transform-origin:top left; }
 .bp3-tether-element-attached-top.bp3-tether-element-attached-center > .bp3-tooltip{
 -webkit-transform-origin:top center;
 transform-origin:top center; }
 .bp3-tether-element-attached-top.bp3-tether-element-attached-right > .bp3-tooltip{
 -webkit-transform-origin:top right;
 transform-origin:top right; }
 .bp3-tether-element-attached-middle.bp3-tether-element-attached-left > .bp3-tooltip{
 -webkit-transform-origin:center left;
 transform-origin:center left; }
 .bp3-tether-element-attached-middle.bp3-tether-element-attached-center > .bp3-tooltip{
 -webkit-transform-origin:center center;
 transform-origin:center center; }
 .bp3-tether-element-attached-middle.bp3-tether-element-attached-right > .bp3-tooltip{
 -webkit-transform-origin:center right;
 transform-origin:center right; }
 .bp3-tether-element-attached-bottom.bp3-tether-element-attached-left > .bp3-tooltip{
 -webkit-transform-origin:bottom left;
 transform-origin:bottom left; }
 .bp3-tether-element-attached-bottom.bp3-tether-element-attached-center > .bp3-tooltip{
 -webkit-transform-origin:bottom center;
 transform-origin:bottom center; }
 .bp3-tether-element-attached-bottom.bp3-tether-element-attached-right > .bp3-tooltip{
 -webkit-transform-origin:bottom right;
 transform-origin:bottom right; }
 .bp3-tooltip .bp3-popover-content{
 background:#394b59;
 color:#f5f8fa; }
 .bp3-tooltip .bp3-popover-arrow::before{
 -webkit-box-shadow:1px 1px 6px rgba(16, 22, 26, 0.2);
 box-shadow:1px 1px 6px rgba(16, 22, 26, 0.2); }
 .bp3-tooltip .bp3-popover-arrow-border{
 fill:#10161a;
 fill-opacity:0.1; }
 .bp3-tooltip .bp3-popover-arrow-fill{
 fill:#394b59; }
 .bp3-popover-enter > .bp3-tooltip, .bp3-popover-appear > .bp3-tooltip{
 -webkit-transform:scale(0.8);
 transform:scale(0.8); }
 .bp3-popover-enter-active > .bp3-tooltip, .bp3-popover-appear-active > .bp3-tooltip{
 -webkit-transform:scale(1);
 transform:scale(1);
 -webkit-transition-delay:0;
 transition-delay:0;
 -webkit-transition-duration:100ms;
 transition-duration:100ms;
 -webkit-transition-property:-webkit-transform;
 transition-property:-webkit-transform;
 transition-property:transform;
 transition-property:transform, -webkit-transform;
 -webkit-transition-timing-function:cubic-bezier(0.4, 1, 0.75, 0.9);
 transition-timing-function:cubic-bezier(0.4, 1, 0.75, 0.9); }
 .bp3-popover-exit > .bp3-tooltip{
 -webkit-transform:scale(1);
 transform:scale(1); }
 .bp3-popover-exit-active > .bp3-tooltip{
 -webkit-transform:scale(0.8);
 transform:scale(0.8);
 -webkit-transition-delay:0;
 transition-delay:0;
 -webkit-transition-duration:100ms;
 transition-duration:100ms;
 -webkit-transition-property:-webkit-transform;
 transition-property:-webkit-transform;
 transition-property:transform;
 transition-property:transform, -webkit-transform;
 -webkit-transition-timing-function:cubic-bezier(0.4, 1, 0.75, 0.9);
 transition-timing-function:cubic-bezier(0.4, 1, 0.75, 0.9); }
 .bp3-tooltip .bp3-popover-content{
 padding:10px 12px; }
 .bp3-tooltip.bp3-dark,
 .bp3-dark .bp3-tooltip{
 -webkit-box-shadow:0 0 0 1px rgba(16, 22, 26, 0.2), 0 2px 4px rgba(16, 22, 26, 0.4), 0 8px 24px rgba(16, 22, 26, 0.4);
 box-shadow:0 0 0 1px rgba(16, 22, 26, 0.2), 0 2px 4px rgba(16, 22, 26, 0.4), 0 8px 24px rgba(16, 22, 26, 0.4); }
 .bp3-tooltip.bp3-dark .bp3-popover-content,
 .bp3-dark .bp3-tooltip .bp3-popover-content{
 background:#e1e8ed;
 color:#394b59; }
 .bp3-tooltip.bp3-dark .bp3-popover-arrow::before,
 .bp3-dark .bp3-tooltip .bp3-popover-arrow::before{
 -webkit-box-shadow:1px 1px 6px rgba(16, 22, 26, 0.4);
 box-shadow:1px 1px 6px rgba(16, 22, 26, 0.4); }
 .bp3-tooltip.bp3-dark .bp3-popover-arrow-border,
 .bp3-dark .bp3-tooltip .bp3-popover-arrow-border{
 fill:#10161a;
 fill-opacity:0.2; }
 .bp3-tooltip.bp3-dark .bp3-popover-arrow-fill,
 .bp3-dark .bp3-tooltip .bp3-popover-arrow-fill{
 fill:#e1e8ed; }
 .bp3-tooltip.bp3-intent-primary .bp3-popover-content{
 background:#137cbd;
 color:#ffffff; }
 .bp3-tooltip.bp3-intent-primary .bp3-popover-arrow-fill{
 fill:#137cbd; }
 .bp3-tooltip.bp3-intent-success .bp3-popover-content{
 background:#0f9960;
 color:#ffffff; }
 .bp3-tooltip.bp3-intent-success .bp3-popover-arrow-fill{
 fill:#0f9960; }
 .bp3-tooltip.bp3-intent-warning .bp3-popover-content{
 background:#d9822b;
 color:#ffffff; }
 .bp3-tooltip.bp3-intent-warning .bp3-popover-arrow-fill{
 fill:#d9822b; }
 .bp3-tooltip.bp3-intent-danger .bp3-popover-content{
 background:#db3737;
 color:#ffffff; }
 .bp3-tooltip.bp3-intent-danger .bp3-popover-arrow-fill{
 fill:#db3737; }

.bp3-tooltip-indicator{
 border-bottom:dotted 1px;
 cursor:help; }
.bp3-tree .bp3-icon, .bp3-tree .bp3-icon-standard, .bp3-tree .bp3-icon-large{
 color:#5c7080; }
 .bp3-tree .bp3-icon.bp3-intent-primary, .bp3-tree .bp3-icon-standard.bp3-intent-primary, .bp3-tree .bp3-icon-large.bp3-intent-primary{
 color:#137cbd; }
 .bp3-tree .bp3-icon.bp3-intent-success, .bp3-tree .bp3-icon-standard.bp3-intent-success, .bp3-tree .bp3-icon-large.bp3-intent-success{
 color:#0f9960; }
 .bp3-tree .bp3-icon.bp3-intent-warning, .bp3-tree .bp3-icon-standard.bp3-intent-warning, .bp3-tree .bp3-icon-large.bp3-intent-warning{
 color:#d9822b; }
 .bp3-tree .bp3-icon.bp3-intent-danger, .bp3-tree .bp3-icon-standard.bp3-intent-danger, .bp3-tree .bp3-icon-large.bp3-intent-danger{
 color:#db3737; }

.bp3-tree-node-list{
 list-style:none;
 margin:0;
 padding-left:0; }

.bp3-tree-root{
 background-color:transparent;
 cursor:default;
 padding-left:0;
 position:relative; }

.bp3-tree-node-content-0{
 padding-left:0px; }

.bp3-tree-node-content-1{
 padding-left:23px; }

.bp3-tree-node-content-2{
 padding-left:46px; }

.bp3-tree-node-content-3{
 padding-left:69px; }

.bp3-tree-node-content-4{
 padding-left:92px; }

.bp3-tree-node-content-5{
 padding-left:115px; }

.bp3-tree-node-content-6{
 padding-left:138px; }

.bp3-tree-node-content-7{
 padding-left:161px; }

.bp3-tree-node-content-8{
 padding-left:184px; }

.bp3-tree-node-content-9{
 padding-left:207px; }

.bp3-tree-node-content-10{
 padding-left:230px; }

.bp3-tree-node-content-11{
 padding-left:253px; }

.bp3-tree-node-content-12{
 padding-left:276px; }

.bp3-tree-node-content-13{
 padding-left:299px; }

.bp3-tree-node-content-14{
 padding-left:322px; }

.bp3-tree-node-content-15{
 padding-left:345px; }

.bp3-tree-node-content-16{
 padding-left:368px; }

.bp3-tree-node-content-17{
 padding-left:391px; }

.bp3-tree-node-content-18{
 padding-left:414px; }

.bp3-tree-node-content-19{
 padding-left:437px; }

.bp3-tree-node-content-20{
 padding-left:460px; }

.bp3-tree-node-content{
 -webkit-box-align:center;
 -ms-flex-align:center;
 align-items:center;
 display:-webkit-box;
 display:-ms-flexbox;
 display:flex;
 height:30px;
 padding-right:5px;
 width:100%; }
 .bp3-tree-node-content:hover{
 background-color:rgba(191, 204, 214, 0.4); }

.bp3-tree-node-caret,
.bp3-tree-node-caret-none{
 min-width:30px; }

.bp3-tree-node-caret{
 color:#5c7080;
 cursor:pointer;
 padding:7px;
 -webkit-transform:rotate(0deg);
 transform:rotate(0deg);
 -webkit-transition:-webkit-transform 200ms cubic-bezier(0.4, 1, 0.75, 0.9);
 transition:-webkit-transform 200ms cubic-bezier(0.4, 1, 0.75, 0.9);
 transition:transform 200ms cubic-bezier(0.4, 1, 0.75, 0.9);
 transition:transform 200ms cubic-bezier(0.4, 1, 0.75, 0.9), -webkit-transform 200ms cubic-bezier(0.4, 1, 0.75, 0.9); }
 .bp3-tree-node-caret:hover{
 color:#182026; }
 .bp3-dark .bp3-tree-node-caret{
 color:#a7b6c2; }
 .bp3-dark .bp3-tree-node-caret:hover{
 color:#f5f8fa; }
 .bp3-tree-node-caret.bp3-tree-node-caret-open{
 -webkit-transform:rotate(90deg);
 transform:rotate(90deg); }
 .bp3-tree-node-caret.bp3-icon-standard::before{
 content:""; }

.bp3-tree-node-icon{
 margin-right:7px;
 position:relative; }

.bp3-tree-node-label{
 overflow:hidden;
 text-overflow:ellipsis;
 white-space:nowrap;
 word-wrap:normal;
 -webkit-box-flex:1;
 -ms-flex:1 1 auto;
 flex:1 1 auto;
 position:relative;
 -webkit-user-select:none;
 -moz-user-select:none;
 -ms-user-select:none;
 user-select:none; }
 .bp3-tree-node-label span{
 display:inline; }

.bp3-tree-node-secondary-label{
 padding:0 5px;
 -webkit-user-select:none;
 -moz-user-select:none;
 -ms-user-select:none;
 user-select:none; }
 .bp3-tree-node-secondary-label .bp3-popover-wrapper,
 .bp3-tree-node-secondary-label .bp3-popover-target{
 -webkit-box-align:center;
 -ms-flex-align:center;
 align-items:center;
 display:-webkit-box;
 display:-ms-flexbox;
 display:flex; }

.bp3-tree-node.bp3-disabled .bp3-tree-node-content{
 background-color:inherit;
 color:rgba(92, 112, 128, 0.6);
 cursor:not-allowed; }

.bp3-tree-node.bp3-disabled .bp3-tree-node-caret,
.bp3-tree-node.bp3-disabled .bp3-tree-node-icon{
 color:rgba(92, 112, 128, 0.6);
 cursor:not-allowed; }

.bp3-tree-node.bp3-tree-node-selected > .bp3-tree-node-content{
 background-color:#137cbd; }
 .bp3-tree-node.bp3-tree-node-selected > .bp3-tree-node-content,
 .bp3-tree-node.bp3-tree-node-selected > .bp3-tree-node-content .bp3-icon, .bp3-tree-node.bp3-tree-node-selected > .bp3-tree-node-content .bp3-icon-standard, .bp3-tree-node.bp3-tree-node-selected > .bp3-tree-node-content .bp3-icon-large{
 color:#ffffff; }
 .bp3-tree-node.bp3-tree-node-selected > .bp3-tree-node-content .bp3-tree-node-caret::before{
 color:rgba(255, 255, 255, 0.7); }
 .bp3-tree-node.bp3-tree-node-selected > .bp3-tree-node-content .bp3-tree-node-caret:hover::before{
 color:#ffffff; }

.bp3-dark .bp3-tree-node-content:hover{
 background-color:rgba(92, 112, 128, 0.3); }

.bp3-dark .bp3-tree .bp3-icon, .bp3-dark .bp3-tree .bp3-icon-standard, .bp3-dark .bp3-tree .bp3-icon-large{
 color:#a7b6c2; }
 .bp3-dark .bp3-tree .bp3-icon.bp3-intent-primary, .bp3-dark .bp3-tree .bp3-icon-standard.bp3-intent-primary, .bp3-dark .bp3-tree .bp3-icon-large.bp3-intent-primary{
 color:#137cbd; }
 .bp3-dark .bp3-tree .bp3-icon.bp3-intent-success, .bp3-dark .bp3-tree .bp3-icon-standard.bp3-intent-success, .bp3-dark .bp3-tree .bp3-icon-large.bp3-intent-success{
 color:#0f9960; }
 .bp3-dark .bp3-tree .bp3-icon.bp3-intent-warning, .bp3-dark .bp3-tree .bp3-icon-standard.bp3-intent-warning, .bp3-dark .bp3-tree .bp3-icon-large.bp3-intent-warning{
 color:#d9822b; }
 .bp3-dark .bp3-tree .bp3-icon.bp3-intent-danger, .bp3-dark .bp3-tree .bp3-icon-standard.bp3-intent-danger, .bp3-dark .bp3-tree .bp3-icon-large.bp3-intent-danger{
 color:#db3737; }

.bp3-dark .bp3-tree-node.bp3-tree-node-selected > .bp3-tree-node-content{
 background-color:#137cbd; }
.bp3-omnibar{
 -webkit-filter:blur(0);
 filter:blur(0);
 opacity:1;
 background-color:#ffffff;
 border-radius:3px;
 -webkit-box-shadow:0 0 0 1px rgba(16, 22, 26, 0.1), 0 4px 8px rgba(16, 22, 26, 0.2), 0 18px 46px 6px rgba(16, 22, 26, 0.2);
 box-shadow:0 0 0 1px rgba(16, 22, 26, 0.1), 0 4px 8px rgba(16, 22, 26, 0.2), 0 18px 46px 6px rgba(16, 22, 26, 0.2);
 left:calc(50% - 250px);
 top:20vh;
 width:500px;
 z-index:21; }
 .bp3-omnibar.bp3-overlay-enter, .bp3-omnibar.bp3-overlay-appear{
 -webkit-filter:blur(20px);
 filter:blur(20px);
 opacity:0.2; }
 .bp3-omnibar.bp3-overlay-enter-active, .bp3-omnibar.bp3-overlay-appear-active{
 -webkit-filter:blur(0);
 filter:blur(0);
 opacity:1;
 -webkit-transition-delay:0;
 transition-delay:0;
 -webkit-transition-duration:200ms;
 transition-duration:200ms;
 -webkit-transition-property:opacity, -webkit-filter;
 transition-property:opacity, -webkit-filter;
 transition-property:filter, opacity;
 transition-property:filter, opacity, -webkit-filter;
 -webkit-transition-timing-function:cubic-bezier(0.4, 1, 0.75, 0.9);
 transition-timing-function:cubic-bezier(0.4, 1, 0.75, 0.9); }
 .bp3-omnibar.bp3-overlay-exit{
 -webkit-filter:blur(0);
 filter:blur(0);
 opacity:1; }
 .bp3-omnibar.bp3-overlay-exit-active{
 -webkit-filter:blur(20px);
 filter:blur(20px);
 opacity:0.2;
 -webkit-transition-delay:0;
 transition-delay:0;
 -webkit-transition-duration:200ms;
 transition-duration:200ms;
 -webkit-transition-property:opacity, -webkit-filter;
 transition-property:opacity, -webkit-filter;
 transition-property:filter, opacity;
 transition-property:filter, opacity, -webkit-filter;
 -webkit-transition-timing-function:cubic-bezier(0.4, 1, 0.75, 0.9);
 transition-timing-function:cubic-bezier(0.4, 1, 0.75, 0.9); }
 .bp3-omnibar .bp3-input{
 background-color:transparent;
 border-radius:0; }
 .bp3-omnibar .bp3-input, .bp3-omnibar .bp3-input:focus{
 -webkit-box-shadow:none;
 box-shadow:none; }
 .bp3-omnibar .bp3-menu{
 background-color:transparent;
 border-radius:0;
 -webkit-box-shadow:inset 0 1px 0 rgba(16, 22, 26, 0.15);
 box-shadow:inset 0 1px 0 rgba(16, 22, 26, 0.15);
 max-height:calc(60vh - 40px);
 overflow:auto; }
 .bp3-omnibar .bp3-menu:empty{
 display:none; }
 .bp3-dark .bp3-omnibar, .bp3-omnibar.bp3-dark{
 background-color:#30404d;
 -webkit-box-shadow:0 0 0 1px rgba(16, 22, 26, 0.2), 0 4px 8px rgba(16, 22, 26, 0.4), 0 18px 46px 6px rgba(16, 22, 26, 0.4);
 box-shadow:0 0 0 1px rgba(16, 22, 26, 0.2), 0 4px 8px rgba(16, 22, 26, 0.4), 0 18px 46px 6px rgba(16, 22, 26, 0.4); }

.bp3-omnibar-overlay .bp3-overlay-backdrop{
 background-color:rgba(16, 22, 26, 0.2); }

.bp3-select-popover .bp3-popover-content{
 padding:5px; }

.bp3-select-popover .bp3-input-group{
 margin-bottom:0; }

.bp3-select-popover .bp3-menu{
 max-height:300px;
 max-width:400px;
 overflow:auto;
 padding:0; }
 .bp3-select-popover .bp3-menu:not(:first-child){
 padding-top:5px; }

.bp3-multi-select{
 min-width:150px; }

.bp3-multi-select-popover .bp3-menu{
 max-height:300px;
 max-width:400px;
 overflow:auto; }

.bp3-select-popover .bp3-popover-content{
 padding:5px; }

.bp3-select-popover .bp3-input-group{
 margin-bottom:0; }

.bp3-select-popover .bp3-menu{
 max-height:300px;
 max-width:400px;
 overflow:auto;
 padding:0; }
 .bp3-select-popover .bp3-menu:not(:first-child){
 padding-top:5px; }
/\*-----------------------------------------------------------------------------
| Copyright (c) Jupyter Development Team.
| Distributed under the terms of the Modified BSD License.
|----------------------------------------------------------------------------\*/

/\* This file was auto-generated by ensureUiComponents() in @jupyterlab/buildutils \*/

/\*\*
 \* (DEPRECATED) Support for consuming icons as CSS background images
 \*/

/\* Icons urls \*/

:root {
 --jp-icon-add: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxNiIgdmlld0JveD0iMCAwIDI0IDI0Ij4KICA8ZyBjbGFzcz0ianAtaWNvbjMiIGZpbGw9IiM2MTYxNjEiPgogICAgPHBhdGggZD0iTTE5IDEzaC02djZoLTJ2LTZINXYtMmg2VjVoMnY2aDZ2MnoiLz4KICA8L2c+Cjwvc3ZnPgo=);
 --jp-icon-bug: url(data:image/svg+xml;base64,PHN2ZyB2aWV3Qm94PSIwIDAgMjQgMjQiIHdpZHRoPSIxNiIgeG1sbnM9Imh0dHA6Ly93d3cudzMub3JnLzIwMDAvc3ZnIj4KICA8ZyBjbGFzcz0ianAtaWNvbjMganAtaWNvbi1zZWxlY3RhYmxlIiBmaWxsPSIjNjE2MTYxIj4KICAgIDxwYXRoIGQ9Ik0yMCA4aC0yLjgxYy0uNDUtLjc4LTEuMDctMS40NS0xLjgyLTEuOTZMMTcgNC40MSAxNS41OSAzbC0yLjE3IDIuMTdDMTIuOTYgNS4wNiAxMi40OSA1IDEyIDVjLS40OSAwLS45Ni4wNi0xLjQxLjE3TDguNDEgMyA3IDQuNDFsMS42MiAxLjYzQzcuODggNi41NSA3LjI2IDcuMjIgNi44MSA4SDR2MmgyLjA5Yy0uMDUuMzMtLjA5LjY2LS4wOSAxdjFINHYyaDJ2MWMwIC4zNC4wNC42Ny4wOSAxSDR2MmgyLjgxYzEuMDQgMS43OSAyLjk3IDMgNS4xOSAzczQuMTUtMS4yMSA1LjE5LTNIMjB2LTJoLTIuMDljLjA1LS4zMy4wOS0uNjYuMDktMXYtMWgydi0yaC0ydi0xYzAtLjM0LS4wNC0uNjctLjA5LTFIMjBWOHptLTYgOGgtNHYtMmg0djJ6bTAtNGgtNHYtMmg0djJ6Ii8+CiAgPC9nPgo8L3N2Zz4K);
 --jp-icon-build: url(data:image/svg+xml;base64,PHN2ZyB3aWR0aD0iMTYiIHZpZXdCb3g9IjAgMCAyNCAyNCIgeG1sbnM9Imh0dHA6Ly93d3cudzMub3JnLzIwMDAvc3ZnIj4KICA8ZyBjbGFzcz0ianAtaWNvbjMiIGZpbGw9IiM2MTYxNjEiPgogICAgPHBhdGggZD0iTTE0LjkgMTcuNDVDMTYuMjUgMTcuNDUgMTcuMzUgMTYuMzUgMTcuMzUgMTVDMTcuMzUgMTMuNjUgMTYuMjUgMTIuNTUgMTQuOSAxMi41NUMxMy41NCAxMi41NSAxMi40NSAxMy42NSAxMi40NSAxNUMxMi40NSAxNi4zNSAxMy41NCAxNy40NSAxNC45IDE3LjQ1Wk0yMC4xIDE1LjY4TDIxLjU4IDE2Ljg0QzIxLjcxIDE2Ljk1IDIxLjc1IDE3LjEzIDIxLjY2IDE3LjI5TDIwLjI2IDE5LjcxQzIwLjE3IDE5Ljg2IDIwIDE5LjkyIDE5LjgzIDE5Ljg2TDE4LjA5IDE5LjE2QzE3LjczIDE5LjQ0IDE3LjMzIDE5LjY3IDE2LjkxIDE5Ljg1TDE2LjY0IDIxLjdDMTYuNjIgMjEuODcgMTYuNDcgMjIgMTYuMyAyMkgxMy41QzEzLjMyIDIyIDEzLjE4IDIxLjg3IDEzLjE1IDIxLjdMMTIuODkgMTkuODVDMTIuNDYgMTkuNjcgMTIuMDcgMTkuNDQgMTEuNzEgMTkuMTZMOS45NjAwMiAxOS44NkM5LjgxMDAyIDE5LjkyIDkuNjIwMDIgMTkuODYgOS41NDAwMiAxOS43MUw4LjE0MDAyIDE3LjI5QzguMDUwMDIgMTcuMTMgOC4wOTAwMiAxNi45NSA4LjIyMDAyIDE2Ljg0TDkuNzAwMDIgMTUuNjhMOS42NTAwMSAxNUw5LjcwMDAyIDE0LjMxTDguMjIwMDIgMTMuMTZDOC4wOTAwMiAxMy4wNSA4LjA1MDAyIDEyLjg2IDguMTQwMDIgMTIuNzFMOS41NDAwMiAxMC4yOUM5LjYyMDAyIDEwLjEzIDkuODEwMDIgMTAuMDcgOS45NjAwMiAxMC4xM0wxMS43MSAxMC44NEMxMi4wNyAxMC41NiAxMi40NiAxMC4zMiAxMi44OSAxMC4xNUwxMy4xNSA4LjI4OTk4QzEzLjE4IDguMTI5OTggMTMuMzIgNy45OTk5OCAxMy41IDcuOTk5OThIMTYuM0MxNi40NyA3Ljk5OTk4IDE2LjYyIDguMTI5OTggMTYuNjQgOC4yODk5OEwxNi45MSAxMC4xNUMxNy4zMyAxMC4zMiAxNy43MyAxMC41NiAxOC4wOSAxMC44NEwxOS44MyAxMC4xM0MyMCAxMC4wNyAyMC4xNyAxMC4xMyAyMC4yNiAxMC4yOUwyMS42NiAxMi43MUMyMS43NSAxMi44NiAyMS43MSAxMy4wNSAyMS41OCAxMy4xNkwyMC4xIDE0LjMxTDIwLjE1IDE1TDIwLjEgMTUuNjhaIi8+CiAgICA8cGF0aCBkPSJNNy4zMjk2NiA3LjQ0NDU0QzguMDgzMSA3LjAwOTU0IDguMzM5MzIgNi4wNTMzMiA3LjkwNDMyIDUuMjk5ODhDNy40NjkzMiA0LjU0NjQzIDYuNTA4MSA0LjI4MTU2IDUuNzU0NjYgNC43MTY1NkM1LjM5MTc2IDQuOTI2MDggNS4xMjY5NSA1LjI3MTE4IDUuMDE4NDkgNS42NzU5NEM0LjkxMDA0IDYuMDgwNzEgNC45NjY4MiA2LjUxMTk4IDUuMTc2MzQgNi44NzQ4OEM1LjYxMTM0IDcuNjI4MzIgNi41NzYyMiA3Ljg3OTU0IDcuMzI5NjYgNy40NDQ1NFpNOS42NTcxOCA0Ljc5NTkzTDEwLjg2NzIgNC45NTE3OUMxMC45NjI4IDQuOTc3NDEgMTEuMDQwMiA1LjA3MTMzIDExLjAzODIgNS4xODc5M0wxMS4wMzg4IDYuOTg4OTNDMTEuMDQ1NSA3LjEwMDU0IDEwLjk2MTYgNy4xOTUxOCAxMC44NTUgNy4yMTA1NEw5LjY2MDAxIDcuMzgwODNMOS4yMzkxNSA4LjEzMTg4TDkuNjY5NjEgOS4yNTc0NUM5LjcwNzI5IDkuMzYyNzEgOS42NjkzNCA5LjQ3Njk5IDkuNTc0MDggOS41MzE5OUw4LjAxNTIzIDEwLjQzMkM3LjkxMTMxIDEwLjQ5MiA3Ljc5MzM3IDEwLjQ2NzcgNy43MjEwNSAxMC4zODI0TDYuOTg3NDggOS40MzE4OEw2LjEwOTMxIDkuNDMwODNMNS4zNDcwNCAxMC4zOTA1QzUuMjg5MDkgMTAuNDcwMiA1LjE3MzgzIDEwLjQ5MDUgNS4wNzE4NyAxMC40MzM5TDMuNTEyNDUgOS41MzI5M0MzLjQxMDQ5IDkuNDc2MzMgMy4zNzY0NyA5LjM1NzQxIDMuNDEwNzUgOS4yNTY3OUwzLjg2MzQ3IDguMTQwOTNMMy42MTc0OSA3Ljc3NDg4TDMuNDIzNDcgNy4zNzg4M0wyLjIzMDc1IDcuMjEyOTdDMi4xMjY0NyA3LjE5MjM1IDIuMDQwNDkgNy4xMDM0MiAyLjA0MjQ1IDYuOTg2ODJMMi4wNDE4NyA1LjE4NTgyQzIuMDQzODMgNS4wNjkyMiAyLjExOTA5IDQuOTc5NTggMi4yMTcwNCA0Ljk2OTIyTDMuNDIwNjUgNC43OTM5M0wzLjg2NzQ5IDQuMDI3ODhMMy40MTEwNSAyLjkxNzMxQzMuMzczMzcgMi44MTIwNCAzLjQxMTMxIDIuNjk3NzYgMy41MTUyMyAyLjYzNzc2TDUuMDc0MDggMS43Mzc3NkM1LjE2OTM0IDEuNjgyNzYgNS4yODcyOSAxLjcwNzA0IDUuMzU5NjEgMS43OTIzMUw2LjExOTE1IDIuNzI3ODhMNi45ODAwMSAyLjczODkzTDcuNzI0OTYgMS43ODkyMkM3Ljc5MTU2IDEuNzA0NTggNy45MTU0OCAxLjY3OTIyIDguMDA4NzkgMS43NDA4Mkw5LjU2ODIxIDIuNjQxODJDOS42NzAxNyAyLjY5ODQyIDkuNzEyODUgMi44MTIzNCA5LjY4NzIzIDIuOTA3OTdMOS4yMTcxOCA0LjAzMzgzTDkuNDYzMTYgNC4zOTk4OEw5LjY1NzE4IDQuNzk1OTNaIi8+CiAgPC9nPgo8L3N2Zz4K);
 --jp-icon-caret-down-empty-thin: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxNiIgdmlld0JveD0iMCAwIDIwIDIwIj4KCTxnIGNsYXNzPSJqcC1pY29uMyIgZmlsbD0iIzYxNjE2MSIgc2hhcGUtcmVuZGVyaW5nPSJnZW9tZXRyaWNQcmVjaXNpb24iPgoJCTxwb2x5Z29uIGNsYXNzPSJzdDEiIHBvaW50cz0iOS45LDEzLjYgMy42LDcuNCA0LjQsNi42IDkuOSwxMi4yIDE1LjQsNi43IDE2LjEsNy40ICIvPgoJPC9nPgo8L3N2Zz4K);
 --jp-icon-caret-down-empty: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxNiIgdmlld0JveD0iMCAwIDE4IDE4Ij4KICA8ZyBjbGFzcz0ianAtaWNvbjMiIGZpbGw9IiM2MTYxNjEiIHNoYXBlLXJlbmRlcmluZz0iZ2VvbWV0cmljUHJlY2lzaW9uIj4KICAgIDxwYXRoIGQ9Ik01LjIsNS45TDksOS43bDMuOC0zLjhsMS4yLDEuMmwtNC45LDVsLTQuOS01TDUuMiw1Ljl6Ii8+CiAgPC9nPgo8L3N2Zz4K);
 --jp-icon-caret-down: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxNiIgdmlld0JveD0iMCAwIDE4IDE4Ij4KICA8ZyBjbGFzcz0ianAtaWNvbjMiIGZpbGw9IiM2MTYxNjEiIHNoYXBlLXJlbmRlcmluZz0iZ2VvbWV0cmljUHJlY2lzaW9uIj4KICAgIDxwYXRoIGQ9Ik01LjIsNy41TDksMTEuMmwzLjgtMy44SDUuMnoiLz4KICA8L2c+Cjwvc3ZnPgo=);
 --jp-icon-caret-left: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxNiIgdmlld0JveD0iMCAwIDE4IDE4Ij4KCTxnIGNsYXNzPSJqcC1pY29uMyIgZmlsbD0iIzYxNjE2MSIgc2hhcGUtcmVuZGVyaW5nPSJnZW9tZXRyaWNQcmVjaXNpb24iPgoJCTxwYXRoIGQ9Ik0xMC44LDEyLjhMNy4xLDlsMy44LTMuOGwwLDcuNkgxMC44eiIvPgogIDwvZz4KPC9zdmc+Cg==);
 --jp-icon-caret-right: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxNiIgdmlld0JveD0iMCAwIDE4IDE4Ij4KICA8ZyBjbGFzcz0ianAtaWNvbjMiIGZpbGw9IiM2MTYxNjEiIHNoYXBlLXJlbmRlcmluZz0iZ2VvbWV0cmljUHJlY2lzaW9uIj4KICAgIDxwYXRoIGQ9Ik03LjIsNS4yTDEwLjksOWwtMy44LDMuOFY1LjJINy4yeiIvPgogIDwvZz4KPC9zdmc+Cg==);
 --jp-icon-caret-up-empty-thin: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxNiIgdmlld0JveD0iMCAwIDIwIDIwIj4KCTxnIGNsYXNzPSJqcC1pY29uMyIgZmlsbD0iIzYxNjE2MSIgc2hhcGUtcmVuZGVyaW5nPSJnZW9tZXRyaWNQcmVjaXNpb24iPgoJCTxwb2x5Z29uIGNsYXNzPSJzdDEiIHBvaW50cz0iMTUuNCwxMy4zIDkuOSw3LjcgNC40LDEzLjIgMy42LDEyLjUgOS45LDYuMyAxNi4xLDEyLjYgIi8+Cgk8L2c+Cjwvc3ZnPgo=);
 --jp-icon-caret-up: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxNiIgdmlld0JveD0iMCAwIDE4IDE4Ij4KCTxnIGNsYXNzPSJqcC1pY29uMyIgZmlsbD0iIzYxNjE2MSIgc2hhcGUtcmVuZGVyaW5nPSJnZW9tZXRyaWNQcmVjaXNpb24iPgoJCTxwYXRoIGQ9Ik01LjIsMTAuNUw5LDYuOGwzLjgsMy44SDUuMnoiLz4KICA8L2c+Cjwvc3ZnPgo=);
 --jp-icon-case-sensitive: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxNiIgdmlld0JveD0iMCAwIDIwIDIwIj4KICA8ZyBjbGFzcz0ianAtaWNvbjIiIGZpbGw9IiM0MTQxNDEiPgogICAgPHJlY3QgeD0iMiIgeT0iMiIgd2lkdGg9IjE2IiBoZWlnaHQ9IjE2Ii8+CiAgPC9nPgogIDxnIGNsYXNzPSJqcC1pY29uLWFjY2VudDIiIGZpbGw9IiNGRkYiPgogICAgPHBhdGggZD0iTTcuNiw4aDAuOWwzLjUsOGgtMS4xTDEwLDE0SDZsLTAuOSwySDRMNy42LDh6IE04LDkuMUw2LjQsMTNoMy4yTDgsOS4xeiIvPgogICAgPHBhdGggZD0iTTE2LjYsOS44Yy0wLjIsMC4xLTAuNCwwLjEtMC43LDAuMWMtMC4yLDAtMC40LTAuMS0wLjYtMC4yYy0wLjEtMC4xLTAuMi0wLjQtMC4yLTAuNyBjLTAuMywwLjMtMC42LDAuNS0wLjksMC43Yy0wLjMsMC4xLTAuNywwLjItMS4xLDAuMmMtMC4zLDAtMC41LDAtMC43LTAuMWMtMC4yLTAuMS0wLjQtMC4yLTAuNi0wLjNjLTAuMi0wLjEtMC4zLTAuMy0wLjQtMC41IGMtMC4xLTAuMi0wLjEtMC40LTAuMS0wLjdjMC0wLjMsMC4xLTAuNiwwLjItMC44YzAuMS0wLjIsMC4zLTAuNCwwLjQtMC41QzEyLDcsMTIuMiw2LjksMTIuNSw2LjhjMC4yLTAuMSwwLjUtMC4xLDAuNy0wLjIgYzAuMy0wLjEsMC41LTAuMSwwLjctMC4xYzAuMiwwLDAuNC0wLjEsMC42LTAuMWMwLjIsMCwwLjMtMC4xLDAuNC0wLjJjMC4xLTAuMSwwLjItMC4yLDAuMi0wLjRjMC0xLTEuMS0xLTEuMy0xIGMtMC40LDAtMS40LDAtMS40LDEuMmgtMC45YzAtMC40LDAuMS0wLjcsMC4yLTFjMC4xLTAuMiwwLjMtMC40LDAuNS0wLjZjMC4yLTAuMiwwLjUtMC4zLDAuOC0wLjNDMTMuMyw0LDEzLjYsNCwxMy45LDQgYzAuMywwLDAuNSwwLDAuOCwwLjFjMC4zLDAsMC41LDAuMSwwLjcsMC4yYzAuMiwwLjEsMC40LDAuMywwLjUsMC41QzE2LDUsMTYsNS4yLDE2LDUuNnYyLjljMCwwLjIsMCwwLjQsMCwwLjUgYzAsMC4xLDAuMSwwLjIsMC4zLDAuMmMwLjEsMCwwLjIsMCwwLjMsMFY5Ljh6IE0xNS4yLDYuOWMtMS4yLDAuNi0zLjEsMC4yLTMuMSwxLjRjMCwxLjQsMy4xLDEsMy4xLTAuNVY2Ljl6Ii8+CiAgPC9nPgo8L3N2Zz4K);
 --jp-icon-check: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxNiIgdmlld0JveD0iMCAwIDI0IDI0Ij4KICA8ZyBjbGFzcz0ianAtaWNvbjMganAtaWNvbi1zZWxlY3RhYmxlIiBmaWxsPSIjNjE2MTYxIj4KICAgIDxwYXRoIGQ9Ik05IDE2LjE3TDQuODMgMTJsLTEuNDIgMS40MUw5IDE5IDIxIDdsLTEuNDEtMS40MXoiLz4KICA8L2c+Cjwvc3ZnPgo=);
 --jp-icon-circle-empty: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxNiIgdmlld0JveD0iMCAwIDI0IDI0Ij4KICA8ZyBjbGFzcz0ianAtaWNvbjMiIGZpbGw9IiM2MTYxNjEiPgogICAgPHBhdGggZD0iTTEyIDJDNi40NyAyIDIgNi40NyAyIDEyczQuNDcgMTAgMTAgMTAgMTAtNC40NyAxMC0xMFMxNy41MyAyIDEyIDJ6bTAgMThjLTQuNDEgMC04LTMuNTktOC04czMuNTktOCA4LTggOCAzLjU5IDggOC0zLjU5IDgtOCA4eiIvPgogIDwvZz4KPC9zdmc+Cg==);
 --jp-icon-circle: url(data:image/svg+xml;base64,PHN2ZyB2aWV3Qm94PSIwIDAgMTggMTgiIHdpZHRoPSIxNiIgeG1sbnM9Imh0dHA6Ly93d3cudzMub3JnLzIwMDAvc3ZnIj4KICA8ZyBjbGFzcz0ianAtaWNvbjMiIGZpbGw9IiM2MTYxNjEiPgogICAgPGNpcmNsZSBjeD0iOSIgY3k9IjkiIHI9IjgiLz4KICA8L2c+Cjwvc3ZnPgo=);
 --jp-icon-clear: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxNiIgdmlld0JveD0iMCAwIDI0IDI0Ij4KICA8bWFzayBpZD0iZG9udXRIb2xlIj4KICAgIDxyZWN0IHdpZHRoPSIyNCIgaGVpZ2h0PSIyNCIgZmlsbD0id2hpdGUiIC8+CiAgICA8Y2lyY2xlIGN4PSIxMiIgY3k9IjEyIiByPSI4IiBmaWxsPSJibGFjayIvPgogIDwvbWFzaz4KCiAgPGcgY2xhc3M9ImpwLWljb24zIiBmaWxsPSIjNjE2MTYxIj4KICAgIDxyZWN0IGhlaWdodD0iMTgiIHdpZHRoPSIyIiB4PSIxMSIgeT0iMyIgdHJhbnNmb3JtPSJyb3RhdGUoMzE1LCAxMiwgMTIpIi8+CiAgICA8Y2lyY2xlIGN4PSIxMiIgY3k9IjEyIiByPSIxMCIgbWFzaz0idXJsKCNkb251dEhvbGUpIi8+CiAgPC9nPgo8L3N2Zz4K);
 --jp-icon-close: url(data:image/svg+xml;base64,PHN2ZyB2aWV3Qm94PSIwIDAgMjQgMjQiIHdpZHRoPSIxNiIgeG1sbnM9Imh0dHA6Ly93d3cudzMub3JnLzIwMDAvc3ZnIj4KICA8ZyBjbGFzcz0ianAtaWNvbi1ub25lIGpwLWljb24tc2VsZWN0YWJsZS1pbnZlcnNlIGpwLWljb24zLWhvdmVyIiBmaWxsPSJub25lIj4KICAgIDxjaXJjbGUgY3g9IjEyIiBjeT0iMTIiIHI9IjExIi8+CiAgPC9nPgoKICA8ZyBjbGFzcz0ianAtaWNvbjMganAtaWNvbi1zZWxlY3RhYmxlIGpwLWljb24tYWNjZW50Mi1ob3ZlciIgZmlsbD0iIzYxNjE2MSI+CiAgICA8cGF0aCBkPSJNMTkgNi40MUwxNy41OSA1IDEyIDEwLjU5IDYuNDEgNSA1IDYuNDEgMTAuNTkgMTIgNSAxNy41OSA2LjQxIDE5IDEyIDEzLjQxIDE3LjU5IDE5IDE5IDE3LjU5IDEzLjQxIDEyeiIvPgogIDwvZz4KCiAgPGcgY2xhc3M9ImpwLWljb24tbm9uZSBqcC1pY29uLWJ1c3kiIGZpbGw9Im5vbmUiPgogICAgPGNpcmNsZSBjeD0iMTIiIGN5PSIxMiIgcj0iNyIvPgogIDwvZz4KPC9zdmc+Cg==);
 --jp-icon-code: url(data:image/svg+xml;base64,PHN2ZyB3aWR0aD0iMjIiIGhlaWdodD0iMjIiIHZpZXdCb3g9IjAgMCAyOCAyOCIgeG1sbnM9Imh0dHA6Ly93d3cudzMub3JnLzIwMDAvc3ZnIj4KCTxnIGNsYXNzPSJqcC1pY29uMyIgZmlsbD0iIzYxNjE2MSI+CgkJPHBhdGggZD0iTTExLjQgMTguNkw2LjggMTRMMTEuNCA5LjRMMTAgOEw0IDE0TDEwIDIwTDExLjQgMTguNlpNMTYuNiAxOC42TDIxLjIgMTRMMTYuNiA5LjRMMTggOEwyNCAxNEwxOCAyMEwxNi42IDE4LjZWMTguNloiLz4KCTwvZz4KPC9zdmc+Cg==);
 --jp-icon-console: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxNiIgdmlld0JveD0iMCAwIDIwMCAyMDAiPgogIDxnIGNsYXNzPSJqcC1pY29uLWJyYW5kMSBqcC1pY29uLXNlbGVjdGFibGUiIGZpbGw9IiMwMjg4RDEiPgogICAgPHBhdGggZD0iTTIwIDE5LjhoMTYwdjE1OS45SDIweiIvPgogIDwvZz4KICA8ZyBjbGFzcz0ianAtaWNvbi1zZWxlY3RhYmxlLWludmVyc2UiIGZpbGw9IiNmZmYiPgogICAgPHBhdGggZD0iTTEwNSAxMjcuM2g0MHYxMi44aC00MHpNNTEuMSA3N0w3NCA5OS45bC0yMy4zIDIzLjMgMTAuNSAxMC41IDIzLjMtMjMuM0w5NSA5OS45IDg0LjUgODkuNCA2MS42IDY2LjV6Ii8+CiAgPC9nPgo8L3N2Zz4K);
 --jp-icon-copy: url(data:image/svg+xml;base64,PHN2ZyB2aWV3Qm94PSIwIDAgMTggMTgiIHdpZHRoPSIxNiIgeG1sbnM9Imh0dHA6Ly93d3cudzMub3JnLzIwMDAvc3ZnIj4KICA8ZyBjbGFzcz0ianAtaWNvbjMiIGZpbGw9IiM2MTYxNjEiPgogICAgPHBhdGggZD0iTTExLjksMUgzLjJDMi40LDEsMS43LDEuNywxLjcsMi41djEwLjJoMS41VjIuNWg4LjdWMXogTTE0LjEsMy45aC04Yy0wLjgsMC0xLjUsMC43LTEuNSwxLjV2MTAuMmMwLDAuOCwwLjcsMS41LDEuNSwxLjVoOCBjMC44LDAsMS41LTAuNywxLjUtMS41VjUuNEMxNS41LDQuNiwxNC45LDMuOSwxNC4xLDMuOXogTTE0LjEsMTUuNWgtOFY1LjRoOFYxNS41eiIvPgogIDwvZz4KPC9zdmc+Cg==);
 --jp-icon-copyright: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIGVuYWJsZS1iYWNrZ3JvdW5kPSJuZXcgMCAwIDI0IDI0IiBoZWlnaHQ9IjI0IiB2aWV3Qm94PSIwIDAgMjQgMjQiIHdpZHRoPSIyNCI+CiAgPGcgY2xhc3M9ImpwLWljb24zIiBmaWxsPSIjNjE2MTYxIj4KICAgIDxwYXRoIGQ9Ik0xMS44OCw5LjE0YzEuMjgsMC4wNiwxLjYxLDEuMTUsMS42MywxLjY2aDEuNzljLTAuMDgtMS45OC0xLjQ5LTMuMTktMy40NS0zLjE5QzkuNjQsNy42MSw4LDksOCwxMi4xNCBjMCwxLjk0LDAuOTMsNC4yNCwzLjg0LDQuMjRjMi4yMiwwLDMuNDEtMS42NSwzLjQ0LTIuOTVoLTEuNzljLTAuMDMsMC41OS0wLjQ1LDEuMzgtMS42MywxLjQ0QzEwLjU1LDE0LjgzLDEwLDEzLjgxLDEwLDEyLjE0IEMxMCw5LjI1LDExLjI4LDkuMTYsMTEuODgsOS4xNHogTTEyLDJDNi40OCwyLDIsNi40OCwyLDEyczQuNDgsMTAsMTAsMTBzMTAtNC40OCwxMC0xMFMxNy41MiwyLDEyLDJ6IE0xMiwyMGMtNC40MSwwLTgtMy41OS04LTggczMuNTktOCw4LThzOCwzLjU5LDgsOFMxNi40MSwyMCwxMiwyMHoiLz4KICA8L2c+Cjwvc3ZnPgo=);
 --jp-icon-cut: url(data:image/svg+xml;base64,PHN2ZyB2aWV3Qm94PSIwIDAgMjQgMjQiIHdpZHRoPSIxNiIgeG1sbnM9Imh0dHA6Ly93d3cudzMub3JnLzIwMDAvc3ZnIj4KICA8ZyBjbGFzcz0ianAtaWNvbjMiIGZpbGw9IiM2MTYxNjEiPgogICAgPHBhdGggZD0iTTkuNjQgNy42NGMuMjMtLjUuMzYtMS4wNS4zNi0xLjY0IDAtMi4yMS0xLjc5LTQtNC00UzIgMy43OSAyIDZzMS43OSA0IDQgNGMuNTkgMCAxLjE0LS4xMyAxLjY0LS4zNkwxMCAxMmwtMi4zNiAyLjM2QzcuMTQgMTQuMTMgNi41OSAxNCA2IDE0Yy0yLjIxIDAtNCAxLjc5LTQgNHMxLjc5IDQgNCA0IDQtMS43OSA0LTRjMC0uNTktLjEzLTEuMTQtLjM2LTEuNjRMMTIgMTRsNyA3aDN2LTFMOS42NCA3LjY0ek02IDhjLTEuMSAwLTItLjg5LTItMnMuOS0yIDItMiAyIC44OSAyIDItLjkgMi0yIDJ6bTAgMTJjLTEuMSAwLTItLjg5LTItMnMuOS0yIDItMiAyIC44OSAyIDItLjkgMi0yIDJ6bTYtNy41Yy0uMjggMC0uNS0uMjItLjUtLjVzLjIyLS41LjUtLjUuNS4yMi41LjUtLjIyLjUtLjUuNXpNMTkgM2wtNiA2IDIgMiA3LTdWM3oiLz4KICA8L2c+Cjwvc3ZnPgo=);
 --jp-icon-download: url(data:image/svg+xml;base64,PHN2ZyB2aWV3Qm94PSIwIDAgMjQgMjQiIHdpZHRoPSIxNiIgeG1sbnM9Imh0dHA6Ly93d3cudzMub3JnLzIwMDAvc3ZnIj4KICA8ZyBjbGFzcz0ianAtaWNvbjMiIGZpbGw9IiM2MTYxNjEiPgogICAgPHBhdGggZD0iTTE5IDloLTRWM0g5djZINWw3IDcgNy03ek01IDE4djJoMTR2LTJINXoiLz4KICA8L2c+Cjwvc3ZnPgo=);
 --jp-icon-edit: url(data:image/svg+xml;base64,PHN2ZyB2aWV3Qm94PSIwIDAgMjQgMjQiIHdpZHRoPSIxNiIgeG1sbnM9Imh0dHA6Ly93d3cudzMub3JnLzIwMDAvc3ZnIj4KICA8ZyBjbGFzcz0ianAtaWNvbjMiIGZpbGw9IiM2MTYxNjEiPgogICAgPHBhdGggZD0iTTMgMTcuMjVWMjFoMy43NUwxNy44MSA5Ljk0bC0zLjc1LTMuNzVMMyAxNy4yNXpNMjAuNzEgNy4wNGMuMzktLjM5LjM5LTEuMDIgMC0xLjQxbC0yLjM0LTIuMzRjLS4zOS0uMzktMS4wMi0uMzktMS40MSAwbC0xLjgzIDEuODMgMy43NSAzLjc1IDEuODMtMS44M3oiLz4KICA8L2c+Cjwvc3ZnPgo=);
 --jp-icon-ellipses: url(data:image/svg+xml;base64,PHN2ZyB2aWV3Qm94PSIwIDAgMjQgMjQiIHdpZHRoPSIxNiIgeG1sbnM9Imh0dHA6Ly93d3cudzMub3JnLzIwMDAvc3ZnIj4KICA8ZyBjbGFzcz0ianAtaWNvbjMiIGZpbGw9IiM2MTYxNjEiPgogICAgPGNpcmNsZSBjeD0iNSIgY3k9IjEyIiByPSIyIi8+CiAgICA8Y2lyY2xlIGN4PSIxMiIgY3k9IjEyIiByPSIyIi8+CiAgICA8Y2lyY2xlIGN4PSIxOSIgY3k9IjEyIiByPSIyIi8+CiAgPC9nPgo8L3N2Zz4K);
 --jp-icon-extension: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxNiIgdmlld0JveD0iMCAwIDI0IDI0Ij4KICA8ZyBjbGFzcz0ianAtaWNvbjMiIGZpbGw9IiM2MTYxNjEiPgogICAgPHBhdGggZD0iTTIwLjUgMTFIMTlWN2MwLTEuMS0uOS0yLTItMmgtNFYzLjVDMTMgMi4xMiAxMS44OCAxIDEwLjUgMVM4IDIuMTIgOCAzLjVWNUg0Yy0xLjEgMC0xLjk5LjktMS45OSAydjMuOEgzLjVjMS40OSAwIDIuNyAxLjIxIDIuNyAyLjdzLTEuMjEgMi43LTIuNyAyLjdIMlYyMGMwIDEuMS45IDIgMiAyaDMuOHYtMS41YzAtMS40OSAxLjIxLTIuNyAyLjctMi43IDEuNDkgMCAyLjcgMS4yMSAyLjcgMi43VjIySDE3YzEuMSAwIDItLjkgMi0ydi00aDEuNWMxLjM4IDAgMi41LTEuMTIgMi41LTIuNVMyMS44OCAxMSAyMC41IDExeiIvPgogIDwvZz4KPC9zdmc+Cg==);
 --jp-icon-fast-forward: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIyNCIgaGVpZ2h0PSIyNCIgdmlld0JveD0iMCAwIDI0IDI0Ij4KICAgIDxnIGNsYXNzPSJqcC1pY29uMyIgZmlsbD0iIzYxNjE2MSI+CiAgICAgICAgPHBhdGggZD0iTTQgMThsOC41LTZMNCA2djEyem05LTEydjEybDguNS02TDEzIDZ6Ii8+CiAgICA8L2c+Cjwvc3ZnPgo=);
 --jp-icon-file-upload: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxNiIgdmlld0JveD0iMCAwIDI0IDI0Ij4KICA8ZyBjbGFzcz0ianAtaWNvbjMiIGZpbGw9IiM2MTYxNjEiPgogICAgPHBhdGggZD0iTTkgMTZoNnYtNmg0bC03LTctNyA3aDR6bS00IDJoMTR2Mkg1eiIvPgogIDwvZz4KPC9zdmc+Cg==);
 --jp-icon-file: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxNiIgdmlld0JveD0iMCAwIDIyIDIyIj4KICA8cGF0aCBjbGFzcz0ianAtaWNvbjMganAtaWNvbi1zZWxlY3RhYmxlIiBmaWxsPSIjNjE2MTYxIiBkPSJNMTkuMyA4LjJsLTUuNS01LjVjLS4zLS4zLS43LS41LTEuMi0uNUgzLjljLS44LjEtMS42LjktMS42IDEuOHYxNC4xYzAgLjkuNyAxLjYgMS42IDEuNmgxNC4yYy45IDAgMS42LS43IDEuNi0xLjZWOS40Yy4xLS41LS4xLS45LS40LTEuMnptLTUuOC0zLjNsMy40IDMuNmgtMy40VjQuOXptMy45IDEyLjdINC43Yy0uMSAwLS4yIDAtLjItLjJWNC43YzAtLjIuMS0uMy4yLS4zaDcuMnY0LjRzMCAuOC4zIDEuMWMuMy4zIDEuMS4zIDEuMS4zaDQuM3Y3LjJzLS4xLjItLjIuMnoiLz4KPC9zdmc+Cg==);
 --jp-icon-filter-list: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxNiIgdmlld0JveD0iMCAwIDI0IDI0Ij4KICA8ZyBjbGFzcz0ianAtaWNvbjMiIGZpbGw9IiM2MTYxNjEiPgogICAgPHBhdGggZD0iTTEwIDE4aDR2LTJoLTR2MnpNMyA2djJoMThWNkgzem0zIDdoMTJ2LTJINnYyeiIvPgogIDwvZz4KPC9zdmc+Cg==);
 --jp-icon-folder: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxNiIgdmlld0JveD0iMCAwIDI0IDI0Ij4KICA8cGF0aCBjbGFzcz0ianAtaWNvbjMganAtaWNvbi1zZWxlY3RhYmxlIiBmaWxsPSIjNjE2MTYxIiBkPSJNMTAgNEg0Yy0xLjEgMC0xLjk5LjktMS45OSAyTDIgMThjMCAxLjEuOSAyIDIgMmgxNmMxLjEgMCAyLS45IDItMlY4YzAtMS4xLS45LTItMi0yaC04bC0yLTJ6Ii8+Cjwvc3ZnPgo=);
 --jp-icon-html5: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxNiIgdmlld0JveD0iMCAwIDUxMiA1MTIiPgogIDxwYXRoIGNsYXNzPSJqcC1pY29uMCBqcC1pY29uLXNlbGVjdGFibGUiIGZpbGw9IiMwMDAiIGQ9Ik0xMDguNCAwaDIzdjIyLjhoMjEuMlYwaDIzdjY5aC0yM1Y0NmgtMjF2MjNoLTIzLjJNMjA2IDIzaC0yMC4zVjBoNjMuN3YyM0gyMjl2NDZoLTIzbTUzLjUtNjloMjQuMWwxNC44IDI0LjNMMzEzLjIgMGgyNC4xdjY5aC0yM1YzNC44bC0xNi4xIDI0LjgtMTYuMS0yNC44VjY5aC0yMi42bTg5LjItNjloMjN2NDYuMmgzMi42VjY5aC01NS42Ii8+CiAgPHBhdGggY2xhc3M9ImpwLWljb24tc2VsZWN0YWJsZSIgZmlsbD0iI2U0NGQyNiIgZD0iTTEwNy42IDQ3MWwtMzMtMzcwLjRoMzYyLjhsLTMzIDM3MC4yTDI1NS43IDUxMiIvPgogIDxwYXRoIGNsYXNzPSJqcC1pY29uLXNlbGVjdGFibGUiIGZpbGw9IiNmMTY1MjkiIGQ9Ik0yNTYgNDgwLjVWMTMxaDE0OC4zTDM3NiA0NDciLz4KICA8cGF0aCBjbGFzcz0ianAtaWNvbi1zZWxlY3RhYmxlLWludmVyc2UiIGZpbGw9IiNlYmViZWIiIGQ9Ik0xNDIgMTc2LjNoMTE0djQ1LjRoLTY0LjJsNC4yIDQ2LjVoNjB2NDUuM0gxNTQuNG0yIDIyLjhIMjAybDMuMiAzNi4zIDUwLjggMTMuNnY0Ny40bC05My4yLTI2Ii8+CiAgPHBhdGggY2xhc3M9ImpwLWljb24tc2VsZWN0YWJsZS1pbnZlcnNlIiBmaWxsPSIjZmZmIiBkPSJNMzY5LjYgMTc2LjNIMjU1Ljh2NDUuNGgxMDkuNm0tNC4xIDQ2LjVIMjU1Ljh2NDUuNGg1NmwtNS4zIDU5LTUwLjcgMTMuNnY0Ny4ybDkzLTI1LjgiLz4KPC9zdmc+Cg==);
 --jp-icon-image: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxNiIgdmlld0JveD0iMCAwIDIyIDIyIj4KICA8cGF0aCBjbGFzcz0ianAtaWNvbi1icmFuZDQganAtaWNvbi1zZWxlY3RhYmxlLWludmVyc2UiIGZpbGw9IiNGRkYiIGQ9Ik0yLjIgMi4yaDE3LjV2MTcuNUgyLjJ6Ii8+CiAgPHBhdGggY2xhc3M9ImpwLWljb24tYnJhbmQwIGpwLWljb24tc2VsZWN0YWJsZSIgZmlsbD0iIzNGNTFCNSIgZD0iTTIuMiAyLjJ2MTcuNWgxNy41bC4xLTE3LjVIMi4yem0xMi4xIDIuMmMxLjIgMCAyLjIgMSAyLjIgMi4ycy0xIDIuMi0yLjIgMi4yLTIuMi0xLTIuMi0yLjIgMS0yLjIgMi4yLTIuMnpNNC40IDE3LjZsMy4zLTguOCAzLjMgNi42IDIuMi0zLjIgNC40IDUuNEg0LjR6Ii8+Cjwvc3ZnPgo=);
 --jp-icon-inspector: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxNiIgdmlld0JveD0iMCAwIDI0IDI0Ij4KICA8cGF0aCBjbGFzcz0ianAtaWNvbjMganAtaWNvbi1zZWxlY3RhYmxlIiBmaWxsPSIjNjE2MTYxIiBkPSJNMjAgNEg0Yy0xLjEgMC0xLjk5LjktMS45OSAyTDIgMThjMCAxLjEuOSAyIDIgMmgxNmMxLjEgMCAyLS45IDItMlY2YzAtMS4xLS45LTItMi0yem0tNSAxNEg0di00aDExdjR6bTAtNUg0VjloMTF2NHptNSA1aC00VjloNHY5eiIvPgo8L3N2Zz4K);
 --jp-icon-json: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxNiIgdmlld0JveD0iMCAwIDIyIDIyIj4KICA8ZyBjbGFzcz0ianAtaWNvbi13YXJuMSBqcC1pY29uLXNlbGVjdGFibGUiIGZpbGw9IiNGOUE4MjUiPgogICAgPHBhdGggZD0iTTIwLjIgMTEuOGMtMS42IDAtMS43LjUtMS43IDEgMCAuNC4xLjkuMSAxLjMuMS41LjEuOS4xIDEuMyAwIDEuNy0xLjQgMi4zLTMuNSAyLjNoLS45di0xLjloLjVjMS4xIDAgMS40IDAgMS40LS44IDAtLjMgMC0uNi0uMS0xIDAtLjQtLjEtLjgtLjEtMS4yIDAtMS4zIDAtMS44IDEuMy0yLTEuMy0uMi0xLjMtLjctMS4zLTIgMC0uNC4xLS44LjEtMS4yLjEtLjQuMS0uNy4xLTEgMC0uOC0uNC0uNy0xLjQtLjhoLS41VjQuMWguOWMyLjIgMCAzLjUuNyAzLjUgMi4zIDAgLjQtLjEuOS0uMSAxLjMtLjEuNS0uMS45LS4xIDEuMyAwIC41LjIgMSAxLjcgMXYxLjh6TTEuOCAxMC4xYzEuNiAwIDEuNy0uNSAxLjctMSAwLS40LS4xLS45LS4xLTEuMy0uMS0uNS0uMS0uOS0uMS0xLjMgMC0xLjYgMS40LTIuMyAzLjUtMi4zaC45djEuOWgtLjVjLTEgMC0xLjQgMC0xLjQuOCAwIC4zIDAgLjYuMSAxIDAgLjIuMS42LjEgMSAwIDEuMyAwIDEuOC0xLjMgMkM2IDExLjIgNiAxMS43IDYgMTNjMCAuNC0uMS44LS4xIDEuMi0uMS4zLS4xLjctLjEgMSAwIC44LjMuOCAxLjQuOGguNXYxLjloLS45Yy0yLjEgMC0zLjUtLjYtMy41LTIuMyAwLS40LjEtLjkuMS0xLjMuMS0uNS4xLS45LjEtMS4zIDAtLjUtLjItMS0xLjctMXYtMS45eiIvPgogICAgPGNpcmNsZSBjeD0iMTEiIGN5PSIxMy44IiByPSIyLjEiLz4KICAgIDxjaXJjbGUgY3g9IjExIiBjeT0iOC4yIiByPSIyLjEiLz4KICA8L2c+Cjwvc3ZnPgo=);
 --jp-icon-julia: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxNiIgdmlld0JveD0iMCAwIDMyNSAzMDAiPgogIDxnIGNsYXNzPSJqcC1icmFuZDAganAtaWNvbi1zZWxlY3RhYmxlIiBmaWxsPSIjY2IzYzMzIj4KICAgIDxwYXRoIGQ9Ik0gMTUwLjg5ODQzOCAyMjUgQyAxNTAuODk4NDM4IDI2Ni40MjE4NzUgMTE3LjMyMDMxMiAzMDAgNzUuODk4NDM4IDMwMCBDIDM0LjQ3NjU2MiAzMDAgMC44OTg0MzggMjY2LjQyMTg3NSAwLjg5ODQzOCAyMjUgQyAwLjg5ODQzOCAxODMuNTc4MTI1IDM0LjQ3NjU2MiAxNTAgNzUuODk4NDM4IDE1MCBDIDExNy4zMjAzMTIgMTUwIDE1MC44OTg0MzggMTgzLjU3ODEyNSAxNTAuODk4NDM4IDIyNSIvPgogIDwvZz4KICA8ZyBjbGFzcz0ianAtYnJhbmQwIGpwLWljb24tc2VsZWN0YWJsZSIgZmlsbD0iIzM4OTgyNiI+CiAgICA8cGF0aCBkPSJNIDIzNy41IDc1IEMgMjM3LjUgMTE2LjQyMTg3NSAyMDMuOTIxODc1IDE1MCAxNjIuNSAxNTAgQyAxMjEuMDc4MTI1IDE1MCA4Ny41IDExNi40MjE4NzUgODcuNSA3NSBDIDg3LjUgMzMuNTc4MTI1IDEyMS4wNzgxMjUgMCAxNjIuNSAwIEMgMjAzLjkyMTg3NSAwIDIzNy41IDMzLjU3ODEyNSAyMzcuNSA3NSIvPgogIDwvZz4KICA8ZyBjbGFzcz0ianAtYnJhbmQwIGpwLWljb24tc2VsZWN0YWJsZSIgZmlsbD0iIzk1NThiMiI+CiAgICA8cGF0aCBkPSJNIDMyNC4xMDE1NjIgMjI1IEMgMzI0LjEwMTU2MiAyNjYuNDIxODc1IDI5MC41MjM0MzggMzAwIDI0OS4xMDE1NjIgMzAwIEMgMjA3LjY3OTY4OCAzMDAgMTc0LjEwMTU2MiAyNjYuNDIxODc1IDE3NC4xMDE1NjIgMjI1IEMgMTc0LjEwMTU2MiAxODMuNTc4MTI1IDIwNy42Nzk2ODggMTUwIDI0OS4xMDE1NjIgMTUwIEMgMjkwLjUyMzQzOCAxNTAgMzI0LjEwMTU2MiAxODMuNTc4MTI1IDMyNC4xMDE1NjIgMjI1Ii8+CiAgPC9nPgo8L3N2Zz4K);
 --jp-icon-jupyter-favicon: url(data:image/svg+xml;base64,PHN2ZyB3aWR0aD0iMTUyIiBoZWlnaHQ9IjE2NSIgdmlld0JveD0iMCAwIDE1MiAxNjUiIHZlcnNpb249IjEuMSIgeG1sbnM9Imh0dHA6Ly93d3cudzMub3JnLzIwMDAvc3ZnIj4KICA8ZyBjbGFzcz0ianAtaWNvbi13YXJuMCIgZmlsbD0iI0YzNzcyNiI+CiAgICA8cGF0aCB0cmFuc2Zvcm09InRyYW5zbGF0ZSgwLjA3ODk0NywgMTEwLjU4MjkyNykiIGQ9Ik03NS45NDIyODQyLDI5LjU4MDQ1NjEgQzQzLjMwMjM5NDcsMjkuNTgwNDU2MSAxNC43OTY3ODMyLDE3LjY1MzQ2MzQgMCwwIEM1LjUxMDgzMjExLDE1Ljg0MDY4MjkgMTUuNzgxNTM4OSwyOS41NjY3NzMyIDI5LjM5MDQ5NDcsMzkuMjc4NDE3MSBDNDIuOTk5Nyw0OC45ODk4NTM3IDU5LjI3MzcsNTQuMjA2NzgwNSA3NS45NjA1Nzg5LDU0LjIwNjc4MDUgQzkyLjY0NzQ1NzksNTQuMjA2NzgwNSAxMDguOTIxNDU4LDQ4Ljk4OTg1MzcgMTIyLjUzMDY2MywzOS4yNzg0MTcxIEMxMzYuMTM5NDUzLDI5LjU2Njc3MzIgMTQ2LjQxMDI4NCwxNS44NDA2ODI5IDE1MS45MjExNTgsMCBDMTM3LjA4Nzg2OCwxNy42NTM0NjM0IDEwOC41ODI1ODksMjkuNTgwNDU2MSA3NS45NDIyODQyLDI5LjU4MDQ1NjEgTDc1Ljk0MjI4NDIsMjkuNTgwNDU2MSBaIiAvPgogICAgPHBhdGggdHJhbnNmb3JtPSJ0cmFuc2xhdGUoMC4wMzczNjgsIDAuNzA0ODc4KSIgZD0iTTc1Ljk3ODQ1NzksMjQuNjI2NDA3MyBDMTA4LjYxODc2MywyNC42MjY0MDczIDEzNy4xMjQ0NTgsMzYuNTUzNDQxNSAxNTEuOTIxMTU4LDU0LjIwNjc4MDUgQzE0Ni40MTAyODQsMzguMzY2MjIyIDEzNi4xMzk0NTMsMjQuNjQwMTMxNyAxMjIuNTMwNjYzLDE0LjkyODQ4NzggQzEwOC45MjE0NTgsNS4yMTY4NDM5IDkyLjY0NzQ1NzksMCA3NS45NjA1Nzg5LDAgQzU5LjI3MzcsMCA0Mi45OTk3LDUuMjE2ODQzOSAyOS4zOTA0OTQ3LDE0LjkyODQ4NzggQzE1Ljc4MTUzODksMjQuNjQwMTMxNyA1LjUxMDgzMjExLDM4LjM2NjIyMiAwLDU0LjIwNjc4MDUgQzE0LjgzMzA4MTYsMzYuNTg5OTI5MyA0My4zMzg1Njg0LDI0LjYyNjQwNzMgNzUuOTc4NDU3OSwyNC42MjY0MDczIEw3NS45Nzg0NTc5LDI0LjYyNjQwNzMgWiIgLz4KICA8L2c+Cjwvc3ZnPgo=);
 --jp-icon-jupyter: url(data:image/svg+xml;base64,PHN2ZyB3aWR0aD0iMzkiIGhlaWdodD0iNTEiIHZpZXdCb3g9IjAgMCAzOSA1MSIgeG1sbnM9Imh0dHA6Ly93d3cudzMub3JnLzIwMDAvc3ZnIj4KICA8ZyB0cmFuc2Zvcm09InRyYW5zbGF0ZSgtMTYzOCAtMjI4MSkiPgogICAgPGcgY2xhc3M9ImpwLWljb24td2FybjAiIGZpbGw9IiNGMzc3MjYiPgogICAgICA8cGF0aCB0cmFuc2Zvcm09InRyYW5zbGF0ZSgxNjM5Ljc0IDIzMTEuOTgpIiBkPSJNIDE4LjI2NDYgNy4xMzQxMUMgMTAuNDE0NSA3LjEzNDExIDMuNTU4NzIgNC4yNTc2IDAgMEMgMS4zMjUzOSAzLjgyMDQgMy43OTU1NiA3LjEzMDgxIDcuMDY4NiA5LjQ3MzAzQyAxMC4zNDE3IDExLjgxNTIgMTQuMjU1NyAxMy4wNzM0IDE4LjI2OSAxMy4wNzM0QyAyMi4yODIzIDEzLjA3MzQgMjYuMTk2MyAxMS44MTUyIDI5LjQ2OTQgOS40NzMwM0MgMzIuNzQyNCA3LjEzMDgxIDM1LjIxMjYgMy44MjA0IDM2LjUzOCAwQyAzMi45NzA1IDQuMjU3NiAyNi4xMTQ4IDcuMTM0MTEgMTguMjY0NiA3LjEzNDExWiIvPgogICAgICA8cGF0aCB0cmFuc2Zvcm09InRyYW5zbGF0ZSgxNjM5LjczIDIyODUuNDgpIiBkPSJNIDE4LjI3MzMgNS45MzkzMUMgMjYuMTIzNSA1LjkzOTMxIDMyLjk3OTMgOC44MTU4MyAzNi41MzggMTMuMDczNEMgMzUuMjEyNiA5LjI1MzAzIDMyLjc0MjQgNS45NDI2MiAyOS40Njk0IDMuNjAwNEMgMjYuMTk2MyAxLjI1ODE4IDIyLjI4MjMgMCAxOC4yNjkgMEMgMTQuMjU1NyAwIDEwLjM0MTcgMS4yNTgxOCA3LjA2ODYgMy42MDA0QyAzLjc5NTU2IDUuOTQyNjIgMS4zMjUzOSA5LjI1MzAzIDAgMTMuMDczNEMgMy41Njc0NSA4LjgyNDYzIDEwLjQyMzIgNS45MzkzMSAxOC4yNzMzIDUuOTM5MzFaIi8+CiAgICA8L2c+CiAgICA8ZyBjbGFzcz0ianAtaWNvbjMiIGZpbGw9IiM2MTYxNjEiPgogICAgICA8cGF0aCB0cmFuc2Zvcm09InRyYW5zbGF0ZSgxNjY5LjMgMjI4MS4zMSkiIGQ9Ik0gNS44OTM1MyAyLjg0NEMgNS45MTg4OSAzLjQzMTY1IDUuNzcwODUgNC4wMTM2NyA1LjQ2ODE1IDQuNTE2NDVDIDUuMTY1NDUgNS4wMTkyMiA0LjcyMTY4IDUuNDIwMTUgNC4xOTI5OSA1LjY2ODUxQyAzLjY2NDMgNS45MTY4OCAzLjA3NDQ0IDYuMDAxNTEgMi40OTgwNSA1LjkxMTcxQyAxLjkyMTY2IDUuODIxOSAxLjM4NDYzIDUuNTYxNyAwLjk1NDg5OCA1LjE2NDAxQyAwLjUyNTE3IDQuNzY2MzMgMC4yMjIwNTYgNC4yNDkwMyAwLjA4MzkwMzcgMy42Nzc1N0MgLTAuMDU0MjQ4MyAzLjEwNjExIC0wLjAyMTIzIDIuNTA2MTcgMC4xNzg3ODEgMS45NTM2NEMgMC4zNzg3OTMgMS40MDExIDAuNzM2ODA5IDAuOTIwODE3IDEuMjA3NTQgMC41NzM1MzhDIDEuNjc4MjYgMC4yMjYyNTkgMi4yNDA1NSAwLjAyNzU5MTkgMi44MjMyNiAwLjAwMjY3MjI5QyAzLjYwMzg5IC0wLjAzMDcxMTUgNC4zNjU3MyAwLjI0OTc4OSA0Ljk0MTQyIDAuNzgyNTUxQyA1LjUxNzExIDEuMzE1MzEgNS44NTk1NiAyLjA1Njc2IDUuODkzNTMgMi44NDRaIi8+CiAgICAgIDxwYXRoIHRyYW5zZm9ybT0idHJhbnNsYXRlKDE2MzkuOCAyMzIzLjgxKSIgZD0iTSA3LjQyNzg5IDMuNTgzMzhDIDcuNDYwMDggNC4zMjQzIDcuMjczNTUgNS4wNTgxOSA2Ljg5MTkzIDUuNjkyMTNDIDYuNTEwMzEgNi4zMjYwNyA1Ljk1MDc1IDYuODMxNTYgNS4yODQxMSA3LjE0NDZDIDQuNjE3NDcgNy40NTc2MyAzLjg3MzcxIDcuNTY0MTQgMy4xNDcwMiA3LjQ1MDYzQyAyLjQyMDMyIDcuMzM3MTIgMS43NDMzNiA3LjAwODcgMS4yMDE4NCA2LjUwNjk1QyAwLjY2MDMyOCA2LjAwNTIgMC4yNzg2MSA1LjM1MjY4IDAuMTA1MDE3IDQuNjMyMDJDIC0wLjA2ODU3NTcgMy45MTEzNSAtMC4wMjYyMzYxIDMuMTU0OTQgMC4yMjY2NzUgMi40NTg1NkMgMC40Nzk1ODcgMS43NjIxNyAwLjkzMTY5NyAxLjE1NzEzIDEuNTI1NzYgMC43MjAwMzNDIDIuMTE5ODMgMC4yODI5MzUgMi44MjkxNCAwLjAzMzQzOTUgMy41NjM4OSAwLjAwMzEzMzQ0QyA0LjU0NjY3IC0wLjAzNzQwMzMgNS41MDUyOSAwLjMxNjcwNiA2LjIyOTYxIDAuOTg3ODM1QyA2Ljk1MzkzIDEuNjU4OTYgNy4zODQ4NCAyLjU5MjM1IDcuNDI3ODkgMy41ODMzOEwgNy40Mjc4OSAzLjU4MzM4WiIvPgogICAgICA8cGF0aCB0cmFuc2Zvcm09InRyYW5zbGF0ZSgxNjM4LjM2IDIyODYuMDYpIiBkPSJNIDIuMjc0NzEgNC4zOTYyOUMgMS44NDM2MyA0LjQxNTA4IDEuNDE2NzEgNC4zMDQ0NSAxLjA0Nzk5IDQuMDc4NDNDIDAuNjc5MjY4IDMuODUyNCAwLjM4NTMyOCAzLjUyMTE0IDAuMjAzMzcxIDMuMTI2NTZDIDAuMDIxNDEzNiAyLjczMTk4IC0wLjA0MDM3OTggMi4yOTE4MyAwLjAyNTgxMTYgMS44NjE4MUMgMC4wOTIwMDMxIDEuNDMxOCAwLjI4MzIwNCAxLjAzMTI2IDAuNTc1MjEzIDAuNzEwODgzQyAwLjg2NzIyMiAwLjM5MDUxIDEuMjQ2OTEgMC4xNjQ3MDggMS42NjYyMiAwLjA2MjA1OTJDIDIuMDg1NTMgLTAuMDQwNTg5NyAyLjUyNTYxIC0wLjAxNTQ3MTQgMi45MzA3NiAwLjEzNDIzNUMgMy4zMzU5MSAwLjI4Mzk0MSAzLjY4NzkyIDAuNTUxNTA1IDMuOTQyMjIgMC45MDMwNkMgNC4xOTY1MiAxLjI1NDYyIDQuMzQxNjkgMS42NzQzNiA0LjM1OTM1IDIuMTA5MTZDIDQuMzgyOTkgMi42OTEwNyA0LjE3Njc4IDMuMjU4NjkgMy43ODU5NyAzLjY4NzQ2QyAzLjM5NTE2IDQuMTE2MjQgMi44NTE2NiA0LjM3MTE2IDIuMjc0NzEgNC4zOTYyOUwgMi4yNzQ3MSA0LjM5NjI5WiIvPgogICAgPC9nPgogIDwvZz4+Cjwvc3ZnPgo=);
 --jp-icon-jupyterlab-wordmark: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIyMDAiIHZpZXdCb3g9IjAgMCAxODYwLjggNDc1Ij4KICA8ZyBjbGFzcz0ianAtaWNvbjIiIGZpbGw9IiM0RTRFNEUiIHRyYW5zZm9ybT0idHJhbnNsYXRlKDQ4MC4xMzY0MDEsIDY0LjI3MTQ5MykiPgogICAgPGcgdHJhbnNmb3JtPSJ0cmFuc2xhdGUoMC4wMDAwMDAsIDU4Ljg3NTU2NikiPgogICAgICA8ZyB0cmFuc2Zvcm09InRyYW5zbGF0ZSgwLjA4NzYwMywgMC4xNDAyOTQpIj4KICAgICAgICA8cGF0aCBkPSJNLTQyNi45LDE2OS44YzAsNDguNy0zLjcsNjQuNy0xMy42LDc2LjRjLTEwLjgsMTAtMjUsMTUuNS0zOS43LDE1LjVsMy43LDI5IGMyMi44LDAuMyw0NC44LTcuOSw2MS45LTIzLjFjMTcuOC0xOC41LDI0LTQ0LjEsMjQtODMuM1YwSC00Mjd2MTcwLjFMLTQyNi45LDE2OS44TC00MjYuOSwxNjkuOHoiLz4KICAgICAgPC9nPgogICAgPC9nPgogICAgPGcgdHJhbnNmb3JtPSJ0cmFuc2xhdGUoMTU1LjA0NTI5NiwgNTYuODM3MTA0KSI+CiAgICAgIDxnIHRyYW5zZm9ybT0idHJhbnNsYXRlKDEuNTYyNDUzLCAxLjc5OTg0MikiPgogICAgICAgIDxwYXRoIGQ9Ik0tMzEyLDE0OGMwLDIxLDAsMzkuNSwxLjcsNTUuNGgtMzEuOGwtMi4xLTMzLjNoLTAuOGMtNi43LDExLjYtMTYuNCwyMS4zLTI4LDI3LjkgYy0xMS42LDYuNi0yNC44LDEwLTM4LjIsOS44Yy0zMS40LDAtNjktMTcuNy02OS04OVYwaDM2LjR2MTEyLjdjMCwzOC43LDExLjYsNjQuNyw0NC42LDY0LjdjMTAuMy0wLjIsMjAuNC0zLjUsMjguOS05LjQgYzguNS01LjksMTUuMS0xNC4zLDE4LjktMjMuOWMyLjItNi4xLDMuMy0xMi41LDMuMy0xOC45VjAuMmgzNi40VjE0OEgtMzEyTC0zMTIsMTQ4eiIvPgogICAgICA8L2c+CiAgICA8L2c+CiAgICA8ZyB0cmFuc2Zvcm09InRyYW5zbGF0ZSgzOTAuMDEzMzIyLCA1My40Nzk2MzgpIj4KICAgICAgPGcgdHJhbnNmb3JtPSJ0cmFuc2xhdGUoMS43MDY0NTgsIDAuMjMxNDI1KSI+CiAgICAgICAgPHBhdGggZD0iTS00NzguNiw3MS40YzAtMjYtMC44LTQ3LTEuNy02Ni43aDMyLjdsMS43LDM0LjhoMC44YzcuMS0xMi41LDE3LjUtMjIuOCwzMC4xLTI5LjcgYzEyLjUtNywyNi43LTEwLjMsNDEtOS44YzQ4LjMsMCw4NC43LDQxLjcsODQuNywxMDMuM2MwLDczLjEtNDMuNywxMDkuMi05MSwxMDkuMmMtMTIuMSwwLjUtMjQuMi0yLjItMzUtNy44IGMtMTAuOC01LjYtMTkuOS0xMy45LTI2LjYtMjQuMmgtMC44VjI5MWgtMzZ2LTIyMEwtNDc4LjYsNzEuNEwtNDc4LjYsNzEuNHogTS00NDIuNiwxMjUuNmMwLjEsNS4xLDAuNiwxMC4xLDEuNywxNS4xIGMzLDEyLjMsOS45LDIzLjMsMTkuOCwzMS4xYzkuOSw3LjgsMjIuMSwxMi4xLDM0LjcsMTIuMWMzOC41LDAsNjAuNy0zMS45LDYwLjctNzguNWMwLTQwLjctMjEuMS03NS42LTU5LjUtNzUuNiBjLTEyLjksMC40LTI1LjMsNS4xLTM1LjMsMTMuNGMtOS45LDguMy0xNi45LDE5LjctMTkuNiwzMi40Yy0xLjUsNC45LTIuMywxMC0yLjUsMTUuMVYxMjUuNkwtNDQyLjYsMTI1LjZMLTQ0Mi42LDEyNS42eiIvPgogICAgICA8L2c+CiAgICA8L2c+CiAgICA8ZyB0cmFuc2Zvcm09InRyYW5zbGF0ZSg2MDYuNzQwNzI2LCA1Ni44MzcxMDQpIj4KICAgICAgPGcgdHJhbnNmb3JtPSJ0cmFuc2xhdGUoMC43NTEyMjYsIDEuOTg5Mjk5KSI+CiAgICAgICAgPHBhdGggZD0iTS00NDAuOCwwbDQzLjcsMTIwLjFjNC41LDEzLjQsOS41LDI5LjQsMTIuOCw0MS43aDAuOGMzLjctMTIuMiw3LjktMjcuNywxMi44LTQyLjQgbDM5LjctMTE5LjJoMzguNUwtMzQ2LjksMTQ1Yy0yNiw2OS43LTQzLjcsMTA1LjQtNjguNiwxMjcuMmMtMTIuNSwxMS43LTI3LjksMjAtNDQuNiwyMy45bC05LjEtMzEuMSBjMTEuNy0zLjksMjIuNS0xMC4xLDMxLjgtMTguMWMxMy4yLTExLjEsMjMuNy0yNS4yLDMwLjYtNDEuMmMxLjUtMi44LDIuNS01LjcsMi45LTguOGMtMC4zLTMuMy0xLjItNi42LTIuNS05LjdMLTQ4MC4yLDAuMSBoMzkuN0wtNDQwLjgsMEwtNDQwLjgsMHoiLz4KICAgICAgPC9nPgogICAgPC9nPgogICAgPGcgdHJhbnNmb3JtPSJ0cmFuc2xhdGUoODIyLjc0ODEwNCwgMC4wMDAwMDApIj4KICAgICAgPGcgdHJhbnNmb3JtPSJ0cmFuc2xhdGUoMS40NjQwNTAsIDAuMzc4OTE0KSI+CiAgICAgICAgPHBhdGggZD0iTS00MTMuNywwdjU4LjNoNTJ2MjguMmgtNTJWMTk2YzAsMjUsNywzOS41LDI3LjMsMzkuNWM3LjEsMC4xLDE0LjItMC43LDIxLjEtMi41IGwxLjcsMjcuN2MtMTAuMywzLjctMjEuMyw1LjQtMzIuMiw1Yy03LjMsMC40LTE0LjYtMC43LTIxLjMtMy40Yy02LjgtMi43LTEyLjktNi44LTE3LjktMTIuMWMtMTAuMy0xMC45LTE0LjEtMjktMTQuMS01Mi45IFY4Ni41aC0zMVY1OC4zaDMxVjkuNkwtNDEzLjcsMEwtNDEzLjcsMHoiLz4KICAgICAgPC9nPgogICAgPC9nPgogICAgPGcgdHJhbnNmb3JtPSJ0cmFuc2xhdGUoOTc0LjQzMzI4NiwgNTMuNDc5NjM4KSI+CiAgICAgIDxnIHRyYW5zZm9ybT0idHJhbnNsYXRlKDAuOTkwMDM0LCAwLjYxMDMzOSkiPgogICAgICAgIDxwYXRoIGQ9Ik0tNDQ1LjgsMTEzYzAuOCw1MCwzMi4yLDcwLjYsNjguNiw3MC42YzE5LDAuNiwzNy45LTMsNTUuMy0xMC41bDYuMiwyNi40IGMtMjAuOSw4LjktNDMuNSwxMy4xLTY2LjIsMTIuNmMtNjEuNSwwLTk4LjMtNDEuMi05OC4zLTEwMi41Qy00ODAuMiw0OC4yLTQ0NC43LDAtMzg2LjUsMGM2NS4yLDAsODIuNyw1OC4zLDgyLjcsOTUuNyBjLTAuMSw1LjgtMC41LDExLjUtMS4yLDE3LjJoLTE0MC42SC00NDUuOEwtNDQ1LjgsMTEzeiBNLTMzOS4yLDg2LjZjMC40LTIzLjUtOS41LTYwLjEtNTAuNC02MC4xIGMtMzYuOCwwLTUyLjgsMzQuNC01NS43LDYwLjFILTMzOS4yTC0zMzkuMiw4Ni42TC0zMzkuMiw4Ni42eiIvPgogICAgICA8L2c+CiAgICA8L2c+CiAgICA8ZyB0cmFuc2Zvcm09InRyYW5zbGF0ZSgxMjAxLjk2MTA1OCwgNTMuNDc5NjM4KSI+CiAgICAgIDxnIHRyYW5zZm9ybT0idHJhbnNsYXRlKDEuMTc5NjQwLCAwLjcwNTA2OCkiPgogICAgICAgIDxwYXRoIGQ9Ik0tNDc4LjYsNjhjMC0yMy45LTAuNC00NC41LTEuNy02My40aDMxLjhsMS4yLDM5LjloMS43YzkuMS0yNy4zLDMxLTQ0LjUsNTUuMy00NC41IGMzLjUtMC4xLDcsMC40LDEwLjMsMS4ydjM0LjhjLTQuMS0wLjktOC4yLTEuMy0xMi40LTEuMmMtMjUuNiwwLTQzLjcsMTkuNy00OC43LDQ3LjRjLTEsNS43LTEuNiwxMS41LTEuNywxNy4ydjEwOC4zaC0zNlY2OCBMLTQ3OC42LDY4eiIvPgogICAgICA8L2c+CiAgICA8L2c+CiAgPC9nPgoKICA8ZyBjbGFzcz0ianAtaWNvbi13YXJuMCIgZmlsbD0iI0YzNzcyNiI+CiAgICA8cGF0aCBkPSJNMTM1Mi4zLDMyNi4yaDM3VjI4aC0zN1YzMjYuMnogTTE2MDQuOCwzMjYuMmMtMi41LTEzLjktMy40LTMxLjEtMy40LTQ4Ljd2LTc2IGMwLTQwLjctMTUuMS04My4xLTc3LjMtODMuMWMtMjUuNiwwLTUwLDcuMS02Ni44LDE4LjFsOC40LDI0LjRjMTQuMy05LjIsMzQtMTUuMSw1My0xNS4xYzQxLjYsMCw0Ni4yLDMwLjIsNDYuMiw0N3Y0LjIgYy03OC42LTAuNC0xMjIuMywyNi41LTEyMi4zLDc1LjZjMCwyOS40LDIxLDU4LjQsNjIuMiw1OC40YzI5LDAsNTAuOS0xNC4zLDYyLjItMzAuMmgxLjNsMi45LDI1LjZIMTYwNC44eiBNMTU2NS43LDI1Ny43IGMwLDMuOC0wLjgsOC0yLjEsMTEuOGMtNS45LDE3LjItMjIuNywzNC00OS4yLDM0Yy0xOC45LDAtMzQuOS0xMS4zLTM0LjktMzUuM2MwLTM5LjUsNDUuOC00Ni42LDg2LjItNDUuOFYyNTcuN3ogTTE2OTguNSwzMjYuMiBsMS43LTMzLjZoMS4zYzE1LjEsMjYuOSwzOC43LDM4LjIsNjguMSwzOC4yYzQ1LjQsMCw5MS4yLTM2LjEsOTEuMi0xMDguOGMwLjQtNjEuNy0zNS4zLTEwMy43LTg1LjctMTAzLjcgYy0zMi44LDAtNTYuMywxNC43LTY5LjMsMzcuNGgtMC44VjI4aC0zNi42djI0NS43YzAsMTguMS0wLjgsMzguNi0xLjcsNTIuNUgxNjk4LjV6IE0xNzA0LjgsMjA4LjJjMC01LjksMS4zLTEwLjksMi4xLTE1LjEgYzcuNi0yOC4xLDMxLjEtNDUuNCw1Ni4zLTQ1LjRjMzkuNSwwLDYwLjUsMzQuOSw2MC41LDc1LjZjMCw0Ni42LTIzLjEsNzguMS02MS44LDc4LjFjLTI2LjksMC00OC4zLTE3LjYtNTUuNS00My4zIGMtMC44LTQuMi0xLjctOC44LTEuNy0xMy40VjIwOC4yeiIvPgogIDwvZz4KPC9zdmc+Cg==);
 --jp-icon-kernel: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxNiIgdmlld0JveD0iMCAwIDI0IDI0Ij4KICAgIDxwYXRoIGNsYXNzPSJqcC1pY29uMiIgZmlsbD0iIzYxNjE2MSIgZD0iTTE1IDlIOXY2aDZWOXptLTIgNGgtMnYtMmgydjJ6bTgtMlY5aC0yVjdjMC0xLjEtLjktMi0yLTJoLTJWM2gtMnYyaC0yVjNIOXYySDdjLTEuMSAwLTIgLjktMiAydjJIM3YyaDJ2MkgzdjJoMnYyYzAgMS4xLjkgMiAyIDJoMnYyaDJ2LTJoMnYyaDJ2LTJoMmMxLjEgMCAyLS45IDItMnYtMmgydi0yaC0ydi0yaDJ6bS00IDZIN1Y3aDEwdjEweiIvPgo8L3N2Zz4K);
 --jp-icon-keyboard: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxNiIgdmlld0JveD0iMCAwIDI0IDI0Ij4KICA8cGF0aCBjbGFzcz0ianAtaWNvbjMganAtaWNvbi1zZWxlY3RhYmxlIiBmaWxsPSIjNjE2MTYxIiBkPSJNMjAgNUg0Yy0xLjEgMC0xLjk5LjktMS45OSAyTDIgMTdjMCAxLjEuOSAyIDIgMmgxNmMxLjEgMCAyLS45IDItMlY3YzAtMS4xLS45LTItMi0yem0tOSAzaDJ2MmgtMlY4em0wIDNoMnYyaC0ydi0yek04IDhoMnYySDhWOHptMCAzaDJ2Mkg4di0yem0tMSAySDV2LTJoMnYyem0wLTNINVY4aDJ2MnptOSA3SDh2LTJoOHYyem0wLTRoLTJ2LTJoMnYyem0wLTNoLTJWOGgydjJ6bTMgM2gtMnYtMmgydjJ6bTAtM2gtMlY4aDJ2MnoiLz4KPC9zdmc+Cg==);
 --jp-icon-launcher: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxNiIgdmlld0JveD0iMCAwIDI0IDI0Ij4KICA8cGF0aCBjbGFzcz0ianAtaWNvbjMganAtaWNvbi1zZWxlY3RhYmxlIiBmaWxsPSIjNjE2MTYxIiBkPSJNMTkgMTlINVY1aDdWM0g1YTIgMiAwIDAwLTIgMnYxNGEyIDIgMCAwMDIgMmgxNGMxLjEgMCAyLS45IDItMnYtN2gtMnY3ek0xNCAzdjJoMy41OWwtOS44MyA5LjgzIDEuNDEgMS40MUwxOSA2LjQxVjEwaDJWM2gtN3oiLz4KPC9zdmc+Cg==);
 --jp-icon-line-form: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxNiIgdmlld0JveD0iMCAwIDI0IDI0Ij4KICAgIDxwYXRoIGZpbGw9IndoaXRlIiBkPSJNNS44OCA0LjEyTDEzLjc2IDEybC03Ljg4IDcuODhMOCAyMmwxMC0xMEw4IDJ6Ii8+Cjwvc3ZnPgo=);
 --jp-icon-link: url(data:image/svg+xml;base64,PHN2ZyB2aWV3Qm94PSIwIDAgMjQgMjQiIHdpZHRoPSIxNiIgeG1sbnM9Imh0dHA6Ly93d3cudzMub3JnLzIwMDAvc3ZnIj4KICA8ZyBjbGFzcz0ianAtaWNvbjMiIGZpbGw9IiM2MTYxNjEiPgogICAgPHBhdGggZD0iTTMuOSAxMmMwLTEuNzEgMS4zOS0zLjEgMy4xLTMuMWg0VjdIN2MtMi43NiAwLTUgMi4yNC01IDVzMi4yNCA1IDUgNWg0di0xLjlIN2MtMS43MSAwLTMuMS0xLjM5LTMuMS0zLjF6TTggMTNoOHYtMkg4djJ6bTktNmgtNHYxLjloNGMxLjcxIDAgMy4xIDEuMzkgMy4xIDMuMXMtMS4zOSAzLjEtMy4xIDMuMWgtNFYxN2g0YzIuNzYgMCA1LTIuMjQgNS01cy0yLjI0LTUtNS01eiIvPgogIDwvZz4KPC9zdmc+Cg==);
 --jp-icon-list: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxNiIgdmlld0JveD0iMCAwIDI0IDI0Ij4KICAgIDxwYXRoIGNsYXNzPSJqcC1pY29uMiBqcC1pY29uLXNlbGVjdGFibGUiIGZpbGw9IiM2MTYxNjEiIGQ9Ik0xOSA1djE0SDVWNWgxNG0xLjEtMkgzLjljLS41IDAtLjkuNC0uOS45djE2LjJjMCAuNC40LjkuOS45aDE2LjJjLjQgMCAuOS0uNS45LS45VjMuOWMwLS41LS41LS45LS45LS45ek0xMSA3aDZ2MmgtNlY3em0wIDRoNnYyaC02di0yem0wIDRoNnYyaC02ek03IDdoMnYySDd6bTAgNGgydjJIN3ptMCA0aDJ2Mkg3eiIvPgo8L3N2Zz4=);
 --jp-icon-listings-info: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHZpZXdCb3g9IjAgMCA1MC45NzggNTAuOTc4IiBzdHlsZT0iZW5hYmxlLWJhY2tncm91bmQ6bmV3IDAgMCA1MC45NzggNTAuOTc4OyIgeG1sOnNwYWNlPSJwcmVzZXJ2ZSI+Cgk8Zz4KCQk8cGF0aCBzdHlsZT0iZmlsbDojMDEwMDAyOyIgZD0iTTQzLjUyLDcuNDU4QzM4LjcxMSwyLjY0OCwzMi4zMDcsMCwyNS40ODksMEMxOC42NywwLDEyLjI2NiwyLjY0OCw3LjQ1OCw3LjQ1OAoJCQljLTkuOTQzLDkuOTQxLTkuOTQzLDI2LjExOSwwLDM2LjA2MmM0LjgwOSw0LjgwOSwxMS4yMTIsNy40NTYsMTguMDMxLDcuNDU4YzAsMCwwLjAwMSwwLDAuMDAyLDAKCQkJYzYuODE2LDAsMTMuMjIxLTIuNjQ4LDE4LjAyOS03LjQ1OGM0LjgwOS00LjgwOSw3LjQ1Ny0xMS4yMTIsNy40NTctMTguMDNDNTAuOTc3LDE4LjY3LDQ4LjMyOCwxMi4yNjYsNDMuNTIsNy40NTh6CgkJCSBNNDIuMTA2LDQyLjEwNWMtNC40MzIsNC40MzEtMTAuMzMyLDYuODcyLTE2LjYxNSw2Ljg3MmgtMC4wMDJjLTYuMjg1LTAuMDAxLTEyLjE4Ny0yLjQ0MS0xNi42MTctNi44NzIKCQkJYy05LjE2Mi05LjE2My05LjE2Mi0yNC4wNzEsMC0zMy4yMzNDMTMuMzAzLDQuNDQsMTkuMjA0LDIsMjUuNDg5LDJjNi4yODQsMCwxMi4xODYsMi40NCwxNi42MTcsNi44NzIKCQkJYzQuNDMxLDQuNDMxLDYuODcxLDEwLjMzMiw2Ljg3MSwxNi42MTdDNDguOTc3LDMxLjc3Miw0Ni41MzYsMzcuNjc1LDQyLjEwNiw0Mi4xMDV6Ii8+CgkJPHBhdGggc3R5bGU9ImZpbGw6IzAxMDAwMjsiIGQ9Ik0yMy41NzgsMzIuMjE4Yy0wLjAyMy0xLjczNCwwLjE0My0zLjA1OSwwLjQ5Ni0zLjk3MmMwLjM1My0wLjkxMywxLjExLTEuOTk3LDIuMjcyLTMuMjUzCgkJCWMwLjQ2OC0wLjUzNiwwLjkyMy0xLjA2MiwxLjM2Ny0xLjU3NWMwLjYyNi0wLjc1MywxLjEwNC0xLjQ3OCwxLjQzNi0yLjE3NWMwLjMzMS0wLjcwNywwLjQ5NS0xLjU0MSwwLjQ5NS0yLjUKCQkJYzAtMS4wOTYtMC4yNi0yLjA4OC0wLjc3OS0yLjk3OWMtMC41NjUtMC44NzktMS41MDEtMS4zMzYtMi44MDYtMS4zNjljLTEuODAyLDAuMDU3LTIuOTg1LDAuNjY3LTMuNTUsMS44MzIKCQkJYy0wLjMwMSwwLjUzNS0wLjUwMywxLjE0MS0wLjYwNywxLjgxNGMtMC4xMzksMC43MDctMC4yMDcsMS40MzItMC4yMDcsMi4xNzRoLTIuOTM3Yy0wLjA5MS0yLjIwOCwwLjQwNy00LjExNCwxLjQ5My01LjcxOQoJCQljMS4wNjItMS42NCwyLjg1NS0yLjQ4MSw1LjM3OC0yLjUyN2MyLjE2LDAuMDIzLDMuODc0LDAuNjA4LDUuMTQxLDEuNzU4YzEuMjc4LDEuMTYsMS45MjksMi43NjQsMS45NSw0LjgxMQoJCQljMCwxLjE0Mi0wLjEzNywyLjExMS0wLjQxLDIuOTExYy0wLjMwOSwwLjg0NS0wLjczMSwxLjU5My0xLjI2OCwyLjI0M2MtMC40OTIsMC42NS0xLjA2OCwxLjMxOC0xLjczLDIuMDAyCgkJCWMtMC42NSwwLjY5Ny0xLjMxMywxLjQ3OS0xLjk4NywyLjM0NmMtMC4yMzksMC4zNzctMC40MjksMC43NzctMC41NjUsMS4xOTljLTAuMTYsMC45NTktMC4yMTcsMS45NTEtMC4xNzEsMi45NzkKCQkJQzI2LjU4OSwzMi4yMTgsMjMuNTc4LDMyLjIxOCwyMy41NzgsMzIuMjE4eiBNMjMuNTc4LDM4LjIydi0zLjQ4NGgzLjA3NnYzLjQ4NEgyMy41Nzh6Ii8+Cgk8L2c+Cjwvc3ZnPgo=);
 --jp-icon-markdown: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxNiIgdmlld0JveD0iMCAwIDIyIDIyIj4KICA8cGF0aCBjbGFzcz0ianAtaWNvbi1jb250cmFzdDAganAtaWNvbi1zZWxlY3RhYmxlIiBmaWxsPSIjN0IxRkEyIiBkPSJNNSAxNC45aDEybC02LjEgNnptOS40LTYuOGMwLTEuMy0uMS0yLjktLjEtNC41LS40IDEuNC0uOSAyLjktMS4zIDQuM2wtMS4zIDQuM2gtMkw4LjUgNy45Yy0uNC0xLjMtLjctMi45LTEtNC4zLS4xIDEuNi0uMSAzLjItLjIgNC42TDcgMTIuNEg0LjhsLjctMTFoMy4zTDEwIDVjLjQgMS4yLjcgMi43IDEgMy45LjMtMS4yLjctMi42IDEtMy45bDEuMi0zLjdoMy4zbC42IDExaC0yLjRsLS4zLTQuMnoiLz4KPC9zdmc+Cg==);
 --jp-icon-new-folder: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxNiIgdmlld0JveD0iMCAwIDI0IDI0Ij4KICA8ZyBjbGFzcz0ianAtaWNvbjMiIGZpbGw9IiM2MTYxNjEiPgogICAgPHBhdGggZD0iTTIwIDZoLThsLTItMkg0Yy0xLjExIDAtMS45OS44OS0xLjk5IDJMMiAxOGMwIDEuMTEuODkgMiAyIDJoMTZjMS4xMSAwIDItLjg5IDItMlY4YzAtMS4xMS0uODktMi0yLTJ6bS0xIDhoLTN2M2gtMnYtM2gtM3YtMmgzVjloMnYzaDN2MnoiLz4KICA8L2c+Cjwvc3ZnPgo=);
 --jp-icon-not-trusted: url(data:image/svg+xml;base64,PHN2ZyBmaWxsPSJub25lIiB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxNiIgdmlld0JveD0iMCAwIDI1IDI1Ij4KICAgIDxwYXRoIGNsYXNzPSJqcC1pY29uMiIgc3Ryb2tlPSIjMzMzMzMzIiBzdHJva2Utd2lkdGg9IjIiIHRyYW5zZm9ybT0idHJhbnNsYXRlKDMgMykiIGQ9Ik0xLjg2MDk0IDExLjQ0MDlDMC44MjY0NDggOC43NzAyNyAwLjg2Mzc3OSA2LjA1NzY0IDEuMjQ5MDcgNC4xOTkzMkMyLjQ4MjA2IDMuOTMzNDcgNC4wODA2OCAzLjQwMzQ3IDUuNjAxMDIgMi44NDQ5QzcuMjM1NDkgMi4yNDQ0IDguODU2NjYgMS41ODE1IDkuOTg3NiAxLjA5NTM5QzExLjA1OTcgMS41ODM0MSAxMi42MDk0IDIuMjQ0NCAxNC4yMTggMi44NDMzOUMxNS43NTAzIDMuNDEzOTQgMTcuMzk5NSAzLjk1MjU4IDE4Ljc1MzkgNC4yMTM4NUMxOS4xMzY0IDYuMDcxNzcgMTkuMTcwOSA4Ljc3NzIyIDE4LjEzOSAxMS40NDA5QzE3LjAzMDMgMTQuMzAzMiAxNC42NjY4IDE3LjE4NDQgOS45OTk5OSAxOC45MzU0QzUuMzMzMTkgMTcuMTg0NCAyLjk2OTY4IDE0LjMwMzIgMS44NjA5NCAxMS40NDA5WiIvPgogICAgPHBhdGggY2xhc3M9ImpwLWljb24yIiBzdHJva2U9IiMzMzMzMzMiIHN0cm9rZS13aWR0aD0iMiIgdHJhbnNmb3JtPSJ0cmFuc2xhdGUoOS4zMTU5MiA5LjMyMDMxKSIgZD0iTTcuMzY4NDIgMEwwIDcuMzY0NzkiLz4KICAgIDxwYXRoIGNsYXNzPSJqcC1pY29uMiIgc3Ryb2tlPSIjMzMzMzMzIiBzdHJva2Utd2lkdGg9IjIiIHRyYW5zZm9ybT0idHJhbnNsYXRlKDkuMzE1OTIgMTYuNjgzNikgc2NhbGUoMSAtMSkiIGQ9Ik03LjM2ODQyIDBMMCA3LjM2NDc5Ii8+Cjwvc3ZnPgo=);
 --jp-icon-notebook: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxNiIgdmlld0JveD0iMCAwIDIyIDIyIj4KICA8ZyBjbGFzcz0ianAtaWNvbi13YXJuMCBqcC1pY29uLXNlbGVjdGFibGUiIGZpbGw9IiNFRjZDMDAiPgogICAgPHBhdGggZD0iTTE4LjcgMy4zdjE1LjRIMy4zVjMuM2gxNS40bTEuNS0xLjVIMS44djE4LjNoMTguM2wuMS0xOC4zeiIvPgogICAgPHBhdGggZD0iTTE2LjUgMTYuNWwtNS40LTQuMy01LjYgNC4zdi0xMWgxMXoiLz4KICA8L2c+Cjwvc3ZnPgo=);
 --jp-icon-numbering: url(data:image/svg+xml;base64,PHN2ZyB3aWR0aD0iMjIiIGhlaWdodD0iMjIiIHZpZXdCb3g9IjAgMCAyOCAyOCIgeG1sbnM9Imh0dHA6Ly93d3cudzMub3JnLzIwMDAvc3ZnIj4KCTxnIGNsYXNzPSJqcC1pY29uMyIgZmlsbD0iIzYxNjE2MSI+CgkJPHBhdGggZD0iTTQgMTlINlYxOS41SDVWMjAuNUg2VjIxSDRWMjJIN1YxOEg0VjE5Wk01IDEwSDZWNkg0VjdINVYxMFpNNCAxM0g1LjhMNCAxNS4xVjE2SDdWMTVINS4yTDcgMTIuOVYxMkg0VjEzWk05IDdWOUgyM1Y3SDlaTTkgMjFIMjNWMTlIOVYyMVpNOSAxNUgyM1YxM0g5VjE1WiIvPgoJPC9nPgo8L3N2Zz4K);
 --jp-icon-offline-bolt: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHZpZXdCb3g9IjAgMCAyNCAyNCIgd2lkdGg9IjE2Ij4KICA8ZyBjbGFzcz0ianAtaWNvbjMiIGZpbGw9IiM2MTYxNjEiPgogICAgPHBhdGggZD0iTTEyIDIuMDJjLTUuNTEgMC05Ljk4IDQuNDctOS45OCA5Ljk4czQuNDcgOS45OCA5Ljk4IDkuOTggOS45OC00LjQ3IDkuOTgtOS45OFMxNy41MSAyLjAyIDEyIDIuMDJ6TTExLjQ4IDIwdi02LjI2SDhMMTMgNHY2LjI2aDMuMzVMMTEuNDggMjB6Ii8+CiAgPC9nPgo8L3N2Zz4K);
 --jp-icon-palette: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxNiIgdmlld0JveD0iMCAwIDI0IDI0Ij4KICA8ZyBjbGFzcz0ianAtaWNvbjMiIGZpbGw9IiM2MTYxNjEiPgogICAgPHBhdGggZD0iTTE4IDEzVjIwSDRWNkg5LjAyQzkuMDcgNS4yOSA5LjI0IDQuNjIgOS41IDRINEMyLjkgNCAyIDQuOSAyIDZWMjBDMiAyMS4xIDIuOSAyMiA0IDIySDE4QzE5LjEgMjIgMjAgMjEuMSAyMCAyMFYxNUwxOCAxM1pNMTkuMyA4Ljg5QzE5Ljc0IDguMTkgMjAgNy4zOCAyMCA2LjVDMjAgNC4wMSAxNy45OSAyIDE1LjUgMkMxMy4wMSAyIDExIDQuMDEgMTEgNi41QzExIDguOTkgMTMuMDEgMTEgMTUuNDkgMTFDMTYuMzcgMTEgMTcuMTkgMTAuNzQgMTcuODggMTAuM0wyMSAxMy40MkwyMi40MiAxMkwxOS4zIDguODlaTTE1LjUgOUMxNC4xMiA5IDEzIDcuODggMTMgNi41QzEzIDUuMTIgMTQuMTIgNCAxNS41IDRDMTYuODggNCAxOCA1LjEyIDE4IDYuNUMxOCA3Ljg4IDE2Ljg4IDkgMTUuNSA5WiIvPgogICAgPHBhdGggZmlsbC1ydWxlPSJldmVub2RkIiBjbGlwLXJ1bGU9ImV2ZW5vZGQiIGQ9Ik00IDZIOS4wMTg5NEM5LjAwNjM5IDYuMTY1MDIgOSA2LjMzMTc2IDkgNi41QzkgOC44MTU3NyAxMC4yMTEgMTAuODQ4NyAxMi4wMzQzIDEySDlWMTRIMTZWMTIuOTgxMUMxNi41NzAzIDEyLjkzNzcgMTcuMTIgMTIuODIwNyAxNy42Mzk2IDEyLjYzOTZMMTggMTNWMjBINFY2Wk04IDhINlYxMEg4VjhaTTYgMTJIOFYxNEg2VjEyWk04IDE2SDZWMThIOFYxNlpNOSAxNkgxNlYxOEg5VjE2WiIvPgogIDwvZz4KPC9zdmc+Cg==);
 --jp-icon-paste: url(data:image/svg+xml;base64,PHN2ZyBoZWlnaHQ9IjI0IiB2aWV3Qm94PSIwIDAgMjQgMjQiIHdpZHRoPSIyNCIgeG1sbnM9Imh0dHA6Ly93d3cudzMub3JnLzIwMDAvc3ZnIj4KICAgIDxnIGNsYXNzPSJqcC1pY29uMyIgZmlsbD0iIzYxNjE2MSI+CiAgICAgICAgPHBhdGggZD0iTTE5IDJoLTQuMThDMTQuNC44NCAxMy4zIDAgMTIgMGMtMS4zIDAtMi40Ljg0LTIuODIgMkg1Yy0xLjEgMC0yIC45LTIgMnYxNmMwIDEuMS45IDIgMiAyaDE0YzEuMSAwIDItLjkgMi0yVjRjMC0xLjEtLjktMi0yLTJ6bS03IDBjLjU1IDAgMSAuNDUgMSAxcy0uNDUgMS0xIDEtMS0uNDUtMS0xIC40NS0xIDEtMXptNyAxOEg1VjRoMnYzaDEwVjRoMnYxNnoiLz4KICAgIDwvZz4KPC9zdmc+Cg==);
 --jp-icon-pdf: url(data:image/svg+xml;base64,PHN2ZwogICB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHZpZXdCb3g9IjAgMCAyMiAyMiIgd2lkdGg9IjE2Ij4KICAgIDxwYXRoIHRyYW5zZm9ybT0icm90YXRlKDQ1KSIgY2xhc3M9ImpwLWljb24tc2VsZWN0YWJsZSIgZmlsbD0iI0ZGMkEyQSIKICAgICAgIGQ9Im0gMjIuMzQ0MzY5LC0zLjAxNjM2NDIgaCA1LjYzODYwNCB2IDEuNTc5MjQzMyBoIC0zLjU0OTIyNyB2IDEuNTA4NjkyOTkgaCAzLjMzNzU3NiBWIDEuNjUwODE1NCBoIC0zLjMzNzU3NiB2IDMuNDM1MjYxMyBoIC0yLjA4OTM3NyB6IG0gLTcuMTM2NDQ0LDEuNTc5MjQzMyB2IDQuOTQzOTU0MyBoIDAuNzQ4OTIgcSAxLjI4MDc2MSwwIDEuOTUzNzAzLC0wLjYzNDk1MzUgMC42NzgzNjksLTAuNjM0OTUzNSAwLjY3ODM2OSwtMS44NDUxNjQxIDAsLTEuMjA0NzgzNTUgLTAuNjcyOTQyLC0xLjgzNDMxMDExIC0wLjY3Mjk0MiwtMC42Mjk1MjY1OSAtMS45NTkxMywtMC42Mjk1MjY1OSB6IG0gLTIuMDg5Mzc3LC0xLjU3OTI0MzMgaCAyLjIwMzM0MyBxIDEuODQ1MTY0LDAgMi43NDYwMzksMC4yNjU5MjA3IDAuOTA2MzAxLDAuMjYwNDkzNyAxLjU1MjEwOCwwLjg5MDAyMDMgMC41Njk4MywwLjU0ODEyMjMgMC44NDY2MDUsMS4yNjQ0ODAwNiAwLjI3Njc3NCwwLjcxNjM1NzgxIDAuMjc2Nzc0LDEuNjIyNjU4OTQgMCwwLjkxNzE1NTEgLTAuMjc2Nzc0LDEuNjM4OTM5OSAtMC4yNzY3NzUsMC43MTYzNTc4IC0wLjg0NjYwNSwxLjI2NDQ4IC0wLjY1MTIzNCwwLjYyOTUyNjYgLTEuNTYyOTYyLDAuODk1NDQ3MyAtMC45MTE3MjgsMC4yNjA0OTM3IC0yLjczNTE4NSwwLjI2MDQ5MzcgaCAtMi4yMDMzNDMgeiBtIC04LjE0NTg1NjUsMCBoIDMuNDY3ODIzIHEgMS41NDY2ODE2LDAgMi4zNzE1Nzg1LDAuNjg5MjIzIDAuODMwMzI0LDAuNjgzNzk2MSAwLjgzMDMyNCwxLjk1MzcwMzE0IDAsMS4yNzUzMzM5NyAtMC44MzAzMjQsMS45NjQ1NTcwNiBRIDkuOTg3MTk2MSwyLjI3NDkxNSA4LjQ0MDUxNDUsMi4yNzQ5MTUgSCA3LjA2MjA2ODQgViA1LjA4NjA3NjcgSCA0Ljk3MjY5MTUgWiBtIDIuMDg5Mzc2OSwxLjUxNDExOTkgdiAyLjI2MzAzOTQzIGggMS4xNTU5NDEgcSAwLjYwNzgxODgsMCAwLjkzODg2MjksLTAuMjkzMDU1NDcgMC4zMzEwNDQxLC0wLjI5ODQ4MjQxIDAuMzMxMDQ0MSwtMC44NDExNzc3MiAwLC0wLjU0MjY5NTMxIC0wLjMzMTA0NDEsLTAuODM1NzUwNzQgLTAuMzMxMDQ0MSwtMC4yOTMwNTU1IC0wLjkzODg2MjksLTAuMjkzMDU1NSB6IgovPgo8L3N2Zz4K);
 --jp-icon-python: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxNiIgdmlld0JveD0iMCAwIDIyIDIyIj4KICA8ZyBjbGFzcz0ianAtaWNvbi1icmFuZDAganAtaWNvbi1zZWxlY3RhYmxlIiBmaWxsPSIjMEQ0N0ExIj4KICAgIDxwYXRoIGQ9Ik0xMS4xIDYuOVY1LjhINi45YzAtLjUgMC0xLjMuMi0xLjYuNC0uNy44LTEuMSAxLjctMS40IDEuNy0uMyAyLjUtLjMgMy45LS4xIDEgLjEgMS45LjkgMS45IDEuOXY0LjJjMCAuNS0uOSAxLjYtMiAxLjZIOC44Yy0xLjUgMC0yLjQgMS40LTIuNCAyLjh2Mi4ySDQuN0MzLjUgMTUuMSAzIDE0IDMgMTMuMVY5Yy0uMS0xIC42LTIgMS44LTIgMS41LS4xIDYuMy0uMSA2LjMtLjF6Ii8+CiAgICA8cGF0aCBkPSJNMTAuOSAxNS4xdjEuMWg0LjJjMCAuNSAwIDEuMy0uMiAxLjYtLjQuNy0uOCAxLjEtMS43IDEuNC0xLjcuMy0yLjUuMy0zLjkuMS0xLS4xLTEuOS0uOS0xLjktMS45di00LjJjMC0uNS45LTEuNiAyLTEuNmgzLjhjMS41IDAgMi40LTEuNCAyLjQtMi44VjYuNmgxLjdDMTguNSA2LjkgMTkgOCAxOSA4LjlWMTNjMCAxLS43IDIuMS0xLjkgMi4xaC02LjJ6Ii8+CiAgPC9nPgo8L3N2Zz4K);
 --jp-icon-r-kernel: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxNiIgdmlld0JveD0iMCAwIDIyIDIyIj4KICA8cGF0aCBjbGFzcz0ianAtaWNvbi1jb250cmFzdDMganAtaWNvbi1zZWxlY3RhYmxlIiBmaWxsPSIjMjE5NkYzIiBkPSJNNC40IDIuNWMxLjItLjEgMi45LS4zIDQuOS0uMyAyLjUgMCA0LjEuNCA1LjIgMS4zIDEgLjcgMS41IDEuOSAxLjUgMy41IDAgMi0xLjQgMy41LTIuOSA0LjEgMS4yLjQgMS43IDEuNiAyLjIgMyAuNiAxLjkgMSAzLjkgMS4zIDQuNmgtMy44Yy0uMy0uNC0uOC0xLjctMS4yLTMuN3MtMS4yLTIuNi0yLjYtMi42aC0uOXY2LjRINC40VjIuNXptMy43IDYuOWgxLjRjMS45IDAgMi45LS45IDIuOS0yLjNzLTEtMi4zLTIuOC0yLjNjLS43IDAtMS4zIDAtMS42LjJ2NC41aC4xdi0uMXoiLz4KPC9zdmc+Cg==);
 --jp-icon-react: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxNiIgdmlld0JveD0iMTUwIDE1MCA1NDEuOSAyOTUuMyI+CiAgPGcgY2xhc3M9ImpwLWljb24tYnJhbmQyIGpwLWljb24tc2VsZWN0YWJsZSIgZmlsbD0iIzYxREFGQiI+CiAgICA8cGF0aCBkPSJNNjY2LjMgMjk2LjVjMC0zMi41LTQwLjctNjMuMy0xMDMuMS04Mi40IDE0LjQtNjMuNiA4LTExNC4yLTIwLjItMTMwLjQtNi41LTMuOC0xNC4xLTUuNi0yMi40LTUuNnYyMi4zYzQuNiAwIDguMy45IDExLjQgMi42IDEzLjYgNy44IDE5LjUgMzcuNSAxNC45IDc1LjctMS4xIDkuNC0yLjkgMTkuMy01LjEgMjkuNC0xOS42LTQuOC00MS04LjUtNjMuNS0xMC45LTEzLjUtMTguNS0yNy41LTM1LjMtNDEuNi01MCAzMi42LTMwLjMgNjMuMi00Ni45IDg0LTQ2LjlWNzhjLTI3LjUgMC02My41IDE5LjYtOTkuOSA1My42LTM2LjQtMzMuOC03Mi40LTUzLjItOTkuOS01My4ydjIyLjNjMjAuNyAwIDUxLjQgMTYuNSA4NCA0Ni42LTE0IDE0LjctMjggMzEuNC00MS4zIDQ5LjktMjIuNiAyLjQtNDQgNi4xLTYzLjYgMTEtMi4zLTEwLTQtMTkuNy01LjItMjktNC43LTM4LjIgMS4xLTY3LjkgMTQuNi03NS44IDMtMS44IDYuOS0yLjYgMTEuNS0yLjZWNzguNWMtOC40IDAtMTYgMS44LTIyLjYgNS42LTI4LjEgMTYuMi0zNC40IDY2LjctMTkuOSAxMzAuMS02Mi4yIDE5LjItMTAyLjcgNDkuOS0xMDIuNyA4Mi4zIDAgMzIuNSA0MC43IDYzLjMgMTAzLjEgODIuNC0xNC40IDYzLjYtOCAxMTQuMiAyMC4yIDEzMC40IDYuNSAzLjggMTQuMSA1LjYgMjIuNSA1LjYgMjcuNSAwIDYzLjUtMTkuNiA5OS45LTUzLjYgMzYuNCAzMy44IDcyLjQgNTMuMiA5OS45IDUzLjIgOC40IDAgMTYtMS44IDIyLjYtNS42IDI4LjEtMTYuMiAzNC40LTY2LjcgMTkuOS0xMzAuMSA2Mi0xOS4xIDEwMi41LTQ5LjkgMTAyLjUtODIuM3ptLTEzMC4yLTY2LjdjLTMuNyAxMi45LTguMyAyNi4yLTEzLjUgMzkuNS00LjEtOC04LjQtMTYtMTMuMS0yNC00LjYtOC05LjUtMTUuOC0xNC40LTIzLjQgMTQuMiAyLjEgMjcuOSA0LjcgNDEgNy45em0tNDUuOCAxMDYuNWMtNy44IDEzLjUtMTUuOCAyNi4zLTI0LjEgMzguMi0xNC45IDEuMy0zMCAyLTQ1LjIgMi0xNS4xIDAtMzAuMi0uNy00NS0xLjktOC4zLTExLjktMTYuNC0yNC42LTI0LjItMzgtNy42LTEzLjEtMTQuNS0yNi40LTIwLjgtMzkuOCA2LjItMTMuNCAxMy4yLTI2LjggMjAuNy0zOS45IDcuOC0xMy41IDE1LjgtMjYuMyAyNC4xLTM4LjIgMTQuOS0xLjMgMzAtMiA0NS4yLTIgMTUuMSAwIDMwLjIuNyA0NSAxLjkgOC4zIDExLjkgMTYuNCAyNC42IDI0LjIgMzggNy42IDEzLjEgMTQuNSAyNi40IDIwLjggMzkuOC02LjMgMTMuNC0xMy4yIDI2LjgtMjAuNyAzOS45em0zMi4zLTEzYzUuNCAxMy40IDEwIDI2LjggMTMuOCAzOS44LTEzLjEgMy4yLTI2LjkgNS45LTQxLjIgOCA0LjktNy43IDkuOC0xNS42IDE0LjQtMjMuNyA0LjYtOCA4LjktMTYuMSAxMy0yNC4xek00MjEuMiA0MzBjLTkuMy05LjYtMTguNi0yMC4zLTI3LjgtMzIgOSAuNCAxOC4yLjcgMjcuNS43IDkuNCAwIDE4LjctLjIgMjcuOC0uNy05IDExLjctMTguMyAyMi40LTI3LjUgMzJ6bS03NC40LTU4LjljLTE0LjItMi4xLTI3LjktNC43LTQxLTcuOSAzLjctMTIuOSA4LjMtMjYuMiAxMy41LTM5LjUgNC4xIDggOC40IDE2IDEzLjEgMjQgNC43IDggOS41IDE1LjggMTQuNCAyMy40ek00MjAuNyAxNjNjOS4zIDkuNiAxOC42IDIwLjMgMjcuOCAzMi05LS40LTE4LjItLjctMjcuNS0uNy05LjQgMC0xOC43LjItMjcuOC43IDktMTEuNyAxOC4zLTIyLjQgMjcuNS0zMnptLTc0IDU4LjljLTQuOSA3LjctOS44IDE1LjYtMTQuNCAyMy43LTQuNiA4LTguOSAxNi0xMyAyNC01LjQtMTMuNC0xMC0yNi44LTEzLjgtMzkuOCAxMy4xLTMuMSAyNi45LTUuOCA0MS4yLTcuOXptLTkwLjUgMTI1LjJjLTM1LjQtMTUuMS01OC4zLTM0LjktNTguMy01MC42IDAtMTUuNyAyMi45LTM1LjYgNTguMy01MC42IDguNi0zLjcgMTgtNyAyNy43LTEwLjEgNS43IDE5LjYgMTMuMiA0MCAyMi41IDYwLjktOS4yIDIwLjgtMTYuNiA0MS4xLTIyLjIgNjAuNi05LjktMy4xLTE5LjMtNi41LTI4LTEwLjJ6TTMxMCA0OTBjLTEzLjYtNy44LTE5LjUtMzcuNS0xNC45LTc1LjcgMS4xLTkuNCAyLjktMTkuMyA1LjEtMjkuNCAxOS42IDQuOCA0MSA4LjUgNjMuNSAxMC45IDEzLjUgMTguNSAyNy41IDM1LjMgNDEuNiA1MC0zMi42IDMwLjMtNjMuMiA0Ni45LTg0IDQ2LjktNC41LS4xLTguMy0xLTExLjMtMi43em0yMzcuMi03Ni4yYzQuNyAzOC4yLTEuMSA2Ny45LTE0LjYgNzUuOC0zIDEuOC02LjkgMi42LTExLjUgMi42LTIwLjcgMC01MS40LTE2LjUtODQtNDYuNiAxNC0xNC43IDI4LTMxLjQgNDEuMy00OS45IDIyLjYtMi40IDQ0LTYuMSA2My42LTExIDIuMyAxMC4xIDQuMSAxOS44IDUuMiAyOS4xem0zOC41LTY2LjdjLTguNiAzLjctMTggNy0yNy43IDEwLjEtNS43LTE5LjYtMTMuMi00MC0yMi41LTYwLjkgOS4yLTIwLjggMTYuNi00MS4xIDIyLjItNjAuNiA5LjkgMy4xIDE5LjMgNi41IDI4LjEgMTAuMiAzNS40IDE1LjEgNTguMyAzNC45IDU4LjMgNTAuNi0uMSAxNS43LTIzIDM1LjYtNTguNCA1MC42ek0zMjAuOCA3OC40eiIvPgogICAgPGNpcmNsZSBjeD0iNDIwLjkiIGN5PSIyOTYuNSIgcj0iNDUuNyIvPgogIDwvZz4KPC9zdmc+Cg==);
 --jp-icon-redo: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIGhlaWdodD0iMjQiIHZpZXdCb3g9IjAgMCAyNCAyNCIgd2lkdGg9IjE2Ij4KICA8ZyBjbGFzcz0ianAtaWNvbjMiIGZpbGw9IiM2MTYxNjEiPgogICAgICA8cGF0aCBkPSJNMCAwaDI0djI0SDB6IiBmaWxsPSJub25lIi8+PHBhdGggZD0iTTE4LjQgMTAuNkMxNi41NSA4Ljk5IDE0LjE1IDggMTEuNSA4Yy00LjY1IDAtOC41OCAzLjAzLTkuOTYgNy4yMkwzLjkgMTZjMS4wNS0zLjE5IDQuMDUtNS41IDcuNi01LjUgMS45NSAwIDMuNzMuNzIgNS4xMiAxLjg4TDEzIDE2aDlWN2wtMy42IDMuNnoiLz4KICA8L2c+Cjwvc3ZnPgo=);
 --jp-icon-refresh: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxNiIgdmlld0JveD0iMCAwIDE4IDE4Ij4KICAgIDxnIGNsYXNzPSJqcC1pY29uMyIgZmlsbD0iIzYxNjE2MSI+CiAgICAgICAgPHBhdGggZD0iTTkgMTMuNWMtMi40OSAwLTQuNS0yLjAxLTQuNS00LjVTNi41MSA0LjUgOSA0LjVjMS4yNCAwIDIuMzYuNTIgMy4xNyAxLjMzTDEwIDhoNVYzbC0xLjc2IDEuNzZDMTIuMTUgMy42OCAxMC42NiAzIDkgMyA1LjY5IDMgMy4wMSA1LjY5IDMuMDEgOVM1LjY5IDE1IDkgMTVjMi45NyAwIDUuNDMtMi4xNiA1LjktNWgtMS41MmMtLjQ2IDItMi4yNCAzLjUtNC4zOCAzLjV6Ii8+CiAgICA8L2c+Cjwvc3ZnPgo=);
 --jp-icon-regex: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxNiIgdmlld0JveD0iMCAwIDIwIDIwIj4KICA8ZyBjbGFzcz0ianAtaWNvbjIiIGZpbGw9IiM0MTQxNDEiPgogICAgPHJlY3QgeD0iMiIgeT0iMiIgd2lkdGg9IjE2IiBoZWlnaHQ9IjE2Ii8+CiAgPC9nPgoKICA8ZyBjbGFzcz0ianAtaWNvbi1hY2NlbnQyIiBmaWxsPSIjRkZGIj4KICAgIDxjaXJjbGUgY2xhc3M9InN0MiIgY3g9IjUuNSIgY3k9IjE0LjUiIHI9IjEuNSIvPgogICAgPHJlY3QgeD0iMTIiIHk9IjQiIGNsYXNzPSJzdDIiIHdpZHRoPSIxIiBoZWlnaHQ9IjgiLz4KICAgIDxyZWN0IHg9IjguNSIgeT0iNy41IiB0cmFuc2Zvcm09Im1hdHJpeCgwLjg2NiAtMC41IDAuNSAwLjg2NiAtMi4zMjU1IDcuMzIxOSkiIGNsYXNzPSJzdDIiIHdpZHRoPSI4IiBoZWlnaHQ9IjEiLz4KICAgIDxyZWN0IHg9IjEyIiB5PSI0IiB0cmFuc2Zvcm09Im1hdHJpeCgwLjUgLTAuODY2IDAuODY2IDAuNSAtMC42Nzc5IDE0LjgyNTIpIiBjbGFzcz0ic3QyIiB3aWR0aD0iMSIgaGVpZ2h0PSI4Ii8+CiAgPC9nPgo8L3N2Zz4K);
 --jp-icon-run: url(data:image/svg+xml;base64,PHN2ZyBoZWlnaHQ9IjI0IiB2aWV3Qm94PSIwIDAgMjQgMjQiIHdpZHRoPSIyNCIgeG1sbnM9Imh0dHA6Ly93d3cudzMub3JnLzIwMDAvc3ZnIj4KICAgIDxnIGNsYXNzPSJqcC1pY29uMyIgZmlsbD0iIzYxNjE2MSI+CiAgICAgICAgPHBhdGggZD0iTTggNXYxNGwxMS03eiIvPgogICAgPC9nPgo8L3N2Zz4K);
 --jp-icon-running: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxNiIgdmlld0JveD0iMCAwIDUxMiA1MTIiPgogIDxnIGNsYXNzPSJqcC1pY29uMyIgZmlsbD0iIzYxNjE2MSI+CiAgICA8cGF0aCBkPSJNMjU2IDhDMTE5IDggOCAxMTkgOCAyNTZzMTExIDI0OCAyNDggMjQ4IDI0OC0xMTEgMjQ4LTI0OFMzOTMgOCAyNTYgOHptOTYgMzI4YzAgOC44LTcuMiAxNi0xNiAxNkgxNzZjLTguOCAwLTE2LTcuMi0xNi0xNlYxNzZjMC04LjggNy4yLTE2IDE2LTE2aDE2MGM4LjggMCAxNiA3LjIgMTYgMTZ2MTYweiIvPgogIDwvZz4KPC9zdmc+Cg==);
 --jp-icon-save: url(data:image/svg+xml;base64,PHN2ZyBoZWlnaHQ9IjI0IiB2aWV3Qm94PSIwIDAgMjQgMjQiIHdpZHRoPSIyNCIgeG1sbnM9Imh0dHA6Ly93d3cudzMub3JnLzIwMDAvc3ZnIj4KICAgIDxnIGNsYXNzPSJqcC1pY29uMyIgZmlsbD0iIzYxNjE2MSI+CiAgICAgICAgPHBhdGggZD0iTTE3IDNINWMtMS4xMSAwLTIgLjktMiAydjE0YzAgMS4xLjg5IDIgMiAyaDE0YzEuMSAwIDItLjkgMi0yVjdsLTQtNHptLTUgMTZjLTEuNjYgMC0zLTEuMzQtMy0zczEuMzQtMyAzLTMgMyAxLjM0IDMgMy0xLjM0IDMtMyAzem0zLTEwSDVWNWgxMHY0eiIvPgogICAgPC9nPgo8L3N2Zz4K);
 --jp-icon-search: url(data:image/svg+xml;base64,PHN2ZyB2aWV3Qm94PSIwIDAgMTggMTgiIHdpZHRoPSIxNiIgeG1sbnM9Imh0dHA6Ly93d3cudzMub3JnLzIwMDAvc3ZnIj4KICA8ZyBjbGFzcz0ianAtaWNvbjMiIGZpbGw9IiM2MTYxNjEiPgogICAgPHBhdGggZD0iTTEyLjEsMTAuOWgtMC43bC0wLjItMC4yYzAuOC0wLjksMS4zLTIuMiwxLjMtMy41YzAtMy0yLjQtNS40LTUuNC01LjRTMS44LDQuMiwxLjgsNy4xczIuNCw1LjQsNS40LDUuNCBjMS4zLDAsMi41LTAuNSwzLjUtMS4zbDAuMiwwLjJ2MC43bDQuMSw0LjFsMS4yLTEuMkwxMi4xLDEwLjl6IE03LjEsMTAuOWMtMi4xLDAtMy43LTEuNy0zLjctMy43czEuNy0zLjcsMy43LTMuN3MzLjcsMS43LDMuNywzLjcgUzkuMiwxMC45LDcuMSwxMC45eiIvPgogIDwvZz4KPC9zdmc+Cg==);
 --jp-icon-settings: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxNiIgdmlld0JveD0iMCAwIDI0IDI0Ij4KICA8cGF0aCBjbGFzcz0ianAtaWNvbjMganAtaWNvbi1zZWxlY3RhYmxlIiBmaWxsPSIjNjE2MTYxIiBkPSJNMTkuNDMgMTIuOThjLjA0LS4zMi4wNy0uNjQuMDctLjk4cy0uMDMtLjY2LS4wNy0uOThsMi4xMS0xLjY1Yy4xOS0uMTUuMjQtLjQyLjEyLS42NGwtMi0zLjQ2Yy0uMTItLjIyLS4zOS0uMy0uNjEtLjIybC0yLjQ5IDFjLS41Mi0uNC0xLjA4LS43My0xLjY5LS45OGwtLjM4LTIuNjVBLjQ4OC40ODggMCAwMDE0IDJoLTRjLS4yNSAwLS40Ni4xOC0uNDkuNDJsLS4zOCAyLjY1Yy0uNjEuMjUtMS4xNy41OS0xLjY5Ljk4bC0yLjQ5LTFjLS4yMy0uMDktLjQ5IDAtLjYxLjIybC0yIDMuNDZjLS4xMy4yMi0uMDcuNDkuMTIuNjRsMi4xMSAxLjY1Yy0uMDQuMzItLjA3LjY1LS4wNy45OHMuMDMuNjYuMDcuOThsLTIuMTEgMS42NWMtLjE5LjE1LS4yNC40Mi0uMTIuNjRsMiAzLjQ2Yy4xMi4yMi4zOS4zLjYxLjIybDIuNDktMWMuNTIuNCAxLjA4LjczIDEuNjkuOThsLjM4IDIuNjVjLjAzLjI0LjI0LjQyLjQ5LjQyaDRjLjI1IDAgLjQ2LS4xOC40OS0uNDJsLjM4LTIuNjVjLjYxLS4yNSAxLjE3LS41OSAxLjY5LS45OGwyLjQ5IDFjLjIzLjA5LjQ5IDAgLjYxLS4yMmwyLTMuNDZjLjEyLS4yMi4wNy0uNDktLjEyLS42NGwtMi4xMS0xLjY1ek0xMiAxNS41Yy0xLjkzIDAtMy41LTEuNTctMy41LTMuNXMxLjU3LTMuNSAzLjUtMy41IDMuNSAxLjU3IDMuNSAzLjUtMS41NyAzLjUtMy41IDMuNXoiLz4KPC9zdmc+Cg==);
 --jp-icon-spreadsheet: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxNiIgdmlld0JveD0iMCAwIDIyIDIyIj4KICA8cGF0aCBjbGFzcz0ianAtaWNvbi1jb250cmFzdDEganAtaWNvbi1zZWxlY3RhYmxlIiBmaWxsPSIjNENBRjUwIiBkPSJNMi4yIDIuMnYxNy42aDE3LjZWMi4ySDIuMnptMTUuNCA3LjdoLTUuNVY0LjRoNS41djUuNXpNOS45IDQuNHY1LjVINC40VjQuNGg1LjV6bS01LjUgNy43aDUuNXY1LjVINC40di01LjV6bTcuNyA1LjV2LTUuNWg1LjV2NS41aC01LjV6Ii8+Cjwvc3ZnPgo=);
 --jp-icon-stop: url(data:image/svg+xml;base64,PHN2ZyBoZWlnaHQ9IjI0IiB2aWV3Qm94PSIwIDAgMjQgMjQiIHdpZHRoPSIyNCIgeG1sbnM9Imh0dHA6Ly93d3cudzMub3JnLzIwMDAvc3ZnIj4KICAgIDxnIGNsYXNzPSJqcC1pY29uMyIgZmlsbD0iIzYxNjE2MSI+CiAgICAgICAgPHBhdGggZD0iTTAgMGgyNHYyNEgweiIgZmlsbD0ibm9uZSIvPgogICAgICAgIDxwYXRoIGQ9Ik02IDZoMTJ2MTJINnoiLz4KICAgIDwvZz4KPC9zdmc+Cg==);
 --jp-icon-tab: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxNiIgdmlld0JveD0iMCAwIDI0IDI0Ij4KICA8ZyBjbGFzcz0ianAtaWNvbjMiIGZpbGw9IiM2MTYxNjEiPgogICAgPHBhdGggZD0iTTIxIDNIM2MtMS4xIDAtMiAuOS0yIDJ2MTRjMCAxLjEuOSAyIDIgMmgxOGMxLjEgMCAyLS45IDItMlY1YzAtMS4xLS45LTItMi0yem0wIDE2SDNWNWgxMHY0aDh2MTB6Ii8+CiAgPC9nPgo8L3N2Zz4K);
 --jp-icon-table-rows: url(data:image/svg+xml;base64,PHN2ZyBoZWlnaHQ9IjI0IiB2aWV3Qm94PSIwIDAgMjQgMjQiIHdpZHRoPSIyNCIgeG1sbnM9Imh0dHA6Ly93d3cudzMub3JnLzIwMDAvc3ZnIj4KICAgIDxnIGNsYXNzPSJqcC1pY29uMyIgZmlsbD0iIzYxNjE2MSI+CiAgICAgICAgPHBhdGggZD0iTTAgMGgyNHYyNEgweiIgZmlsbD0ibm9uZSIvPgogICAgICAgIDxwYXRoIGQ9Ik0yMSw4SDNWNGgxOFY4eiBNMjEsMTBIM3Y0aDE4VjEweiBNMjEsMTZIM3Y0aDE4VjE2eiIvPgogICAgPC9nPgo8L3N2Zz4=);
 --jp-icon-tag: url(data:image/svg+xml;base64,PHN2ZyB3aWR0aD0iMjgiIGhlaWdodD0iMjgiIHZpZXdCb3g9IjAgMCA0MyAyOCIgeG1sbnM9Imh0dHA6Ly93d3cudzMub3JnLzIwMDAvc3ZnIj4KCTxnIGNsYXNzPSJqcC1pY29uMyIgZmlsbD0iIzYxNjE2MSI+CgkJPHBhdGggZD0iTTI4LjgzMzIgMTIuMzM0TDMyLjk5OTggMTYuNTAwN0wzNy4xNjY1IDEyLjMzNEgyOC44MzMyWiIvPgoJCTxwYXRoIGQ9Ik0xNi4yMDk1IDIxLjYxMDRDMTUuNjg3MyAyMi4xMjk5IDE0Ljg0NDMgMjIuMTI5OSAxNC4zMjQ4IDIxLjYxMDRMNi45ODI5IDE0LjcyNDVDNi41NzI0IDE0LjMzOTQgNi4wODMxMyAxMy42MDk4IDYuMDQ3ODYgMTMuMDQ4MkM1Ljk1MzQ3IDExLjUyODggNi4wMjAwMiA4LjYxOTQ0IDYuMDY2MjEgNy4wNzY5NUM2LjA4MjgxIDYuNTE0NzcgNi41NTU0OCA2LjA0MzQ3IDcuMTE4MDQgNi4wMzA1NUM5LjA4ODYzIDUuOTg0NzMgMTMuMjYzOCA1LjkzNTc5IDEzLjY1MTggNi4zMjQyNUwyMS43MzY5IDEzLjYzOUMyMi4yNTYgMTQuMTU4NSAyMS43ODUxIDE1LjQ3MjQgMjEuMjYyIDE1Ljk5NDZMMTYuMjA5NSAyMS42MTA0Wk05Ljc3NTg1IDguMjY1QzkuMzM1NTEgNy44MjU2NiA4LjYyMzUxIDcuODI1NjYgOC4xODI4IDguMjY1QzcuNzQzNDYgOC43MDU3MSA3Ljc0MzQ2IDkuNDE3MzMgOC4xODI4IDkuODU2NjdDOC42MjM4MiAxMC4yOTY0IDkuMzM1ODIgMTAuMjk2NCA5Ljc3NTg1IDkuODU2NjdDMTAuMjE1NiA5LjQxNzMzIDEwLjIxNTYgOC43MDUzMyA5Ljc3NTg1IDguMjY1WiIvPgoJPC9nPgo8L3N2Zz4K);
 --jp-icon-terminal: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxNiIgdmlld0JveD0iMCAwIDI0IDI0IiA+CiAgICA8cmVjdCBjbGFzcz0ianAtaWNvbjIganAtaWNvbi1zZWxlY3RhYmxlIiB3aWR0aD0iMjAiIGhlaWdodD0iMjAiIHRyYW5zZm9ybT0idHJhbnNsYXRlKDIgMikiIGZpbGw9IiMzMzMzMzMiLz4KICAgIDxwYXRoIGNsYXNzPSJqcC1pY29uLWFjY2VudDIganAtaWNvbi1zZWxlY3RhYmxlLWludmVyc2UiIGQ9Ik01LjA1NjY0IDguNzYxNzJDNS4wNTY2NCA4LjU5NzY2IDUuMDMxMjUgOC40NTMxMiA0Ljk4MDQ3IDguMzI4MTJDNC45MzM1OSA4LjE5OTIyIDQuODU1NDcgOC4wODIwMyA0Ljc0NjA5IDcuOTc2NTZDNC42NDA2MiA3Ljg3MTA5IDQuNSA3Ljc3NTM5IDQuMzI0MjIgNy42ODk0NUM0LjE1MjM0IDcuNTk5NjEgMy45NDMzNiA3LjUxMTcyIDMuNjk3MjcgNy40MjU3OEMzLjMwMjczIDcuMjg1MTYgMi45NDMzNiA3LjEzNjcyIDIuNjE5MTQgNi45ODA0N0MyLjI5NDkyIDYuODI0MjIgMi4wMTc1OCA2LjY0MjU4IDEuNzg3MTEgNi40MzU1NUMxLjU2MDU1IDYuMjI4NTIgMS4zODQ3NyA1Ljk4ODI4IDEuMjU5NzcgNS43MTQ4NEMxLjEzNDc3IDUuNDM3NSAxLjA3MjI3IDUuMTA5MzggMS4wNzIyNyA0LjczMDQ3QzEuMDcyMjcgNC4zOTg0NCAxLjEyODkxIDQuMDk1NyAxLjI0MjE5IDMuODIyMjdDMS4zNTU0NyAzLjU0NDkyIDEuNTE1NjIgMy4zMDQ2OSAxLjcyMjY2IDMuMTAxNTZDMS45Mjk2OSAyLjg5ODQ0IDIuMTc5NjkgMi43MzQzNyAyLjQ3MjY2IDIuNjA5MzhDMi43NjU2MiAyLjQ4NDM4IDMuMDkxOCAyLjQwNDMgMy40NTExNyAyLjM2OTE0VjEuMTA5MzhINC4zODg2N1YyLjM4MDg2QzQuNzQwMjMgMi40Mjc3MyA1LjA1NjY0IDIuNTIzNDQgNS4zMzc4OSAyLjY2Nzk3QzUuNjE5MTQgMi44MTI1IDUuODU3NDIgMy4wMDE5NSA2LjA1MjczIDMuMjM2MzNDNi4yNTE5NSAzLjQ2NjggNi40MDQzIDMuNzQwMjMgNi41MDk3NyA0LjA1NjY0QzYuNjE5MTQgNC4zNjkxNCA2LjY3MzgzIDQuNzIwNyA2LjY3MzgzIDUuMTExMzNINS4wNDQ5MkM1LjA0NDkyIDQuNjM4NjcgNC45Mzc1IDQuMjgxMjUgNC43MjI2NiA0LjAzOTA2QzQuNTA3ODEgMy43OTI5NyA0LjIxNjggMy42Njk5MiAzLjg0OTYxIDMuNjY5OTJDMy42NTAzOSAzLjY2OTkyIDMuNDc2NTYgMy42OTcyNyAzLjMyODEyIDMuNzUxOTVDMy4xODM1OSAzLjgwMjczIDMuMDY0NDUgMy44NzY5NSAyLjk3MDcgMy45NzQ2MUMyLjg3Njk1IDQuMDY4MzYgMi44MDY2NCA0LjE3OTY5IDIuNzU5NzcgNC4zMDg1OUMyLjcxNjggNC40Mzc1IDIuNjk1MzEgNC41NzgxMiAyLjY5NTMxIDQuNzMwNDdDMi42OTUzMSA0Ljg4MjgxIDIuNzE2OCA1LjAxOTUzIDIuNzU5NzcgNS4xNDA2MkMyLjgwNjY0IDUuMjU3ODEgMi44ODI4MSA1LjM2NzE5IDIuOTg4MjggNS40Njg3NUMzLjA5NzY2IDUuNTcwMzEgMy4yNDAyMyA1LjY2Nzk3IDMuNDE2MDIgNS43NjE3MkMzLjU5MTggNS44NTE1NiAzLjgxMDU1IDUuOTQzMzYgNC4wNzIyNyA2LjAzNzExQzQuNDY2OCA2LjE4NTU1IDQuODI0MjIgNi4zMzk4NCA1LjE0NDUzIDYuNUM1LjQ2NDg0IDYuNjU2MjUgNS43MzgyOCA2LjgzOTg0IDUuOTY0ODQgNy4wNTA3OEM2LjE5NTMxIDcuMjU3ODEgNi4zNzEwOSA3LjUgNi40OTIxOSA3Ljc3NzM0QzYuNjE3MTkgOC4wNTA3OCA2LjY3OTY5IDguMzc1IDYuNjc5NjkgOC43NUM2LjY3OTY5IDkuMDkzNzUgNi42MjMwNSA5LjQwNDMgNi41MDk3NyA5LjY4MTY0QzYuMzk2NDggOS45NTUwOCA2LjIzNDM4IDEwLjE5MTQgNi4wMjM0NCAxMC4zOTA2QzUuODEyNSAxMC41ODk4IDUuNTU4NTkgMTAuNzUgNS4yNjE3MiAxMC44NzExQzQuOTY0ODQgMTAuOTg4MyA0LjYzMjgxIDExLjA2NDUgNC4yNjU2MiAxMS4wOTk2VjEyLjI0OEgzLjMzMzk4VjExLjA5OTZDMy4wMDE5NSAxMS4wNjg0IDIuNjc5NjkgMTAuOTk2MSAyLjM2NzE5IDEwLjg4MjhDMi4wNTQ2OSAxMC43NjU2IDEuNzc3MzQgMTAuNTk3NyAxLjUzNTE2IDEwLjM3ODlDMS4yOTY4OCAxMC4xNjAyIDEuMTA1NDcgOS44ODQ3NyAwLjk2MDkzOCA5LjU1MjczQzAuODE2NDA2IDkuMjE2OCAwLjc0NDE0MSA4LjgxNDQ1IDAuNzQ0MTQxIDguMzQ1N0gyLjM3ODkxQzIuMzc4OTEgOC42MjY5NSAyLjQxOTkyIDguODYzMjggMi41MDE5NSA5LjA1NDY5QzIuNTgzOTggOS4yNDIxOSAyLjY4OTQ1IDkuMzkyNTggMi44MTgzNiA5LjUwNTg2QzIuOTUxMTcgOS42MTUyMyAzLjEwMTU2IDkuNjkzMzYgMy4yNjk1MyA5Ljc0MDIzQzMuNDM3NSA5Ljc4NzExIDMuNjA5MzggOS44MTA1NSAzLjc4NTE2IDkuODEwNTVDNC4yMDMxMiA5LjgxMDU1IDQuNTE5NTMgOS43MTI4OSA0LjczNDM4IDkuNTE3NThDNC45NDkyMiA5LjMyMjI3IDUuMDU2NjQgOS4wNzAzMSA1LjA1NjY0IDguNzYxNzJaTTEzLjQxOCAxMi4yNzE1SDguMDc0MjJWMTFIMTMuNDE4VjEyLjI3MTVaIiB0cmFuc2Zvcm09InRyYW5zbGF0ZSgzLjk1MjY0IDYpIiBmaWxsPSJ3aGl0ZSIvPgo8L3N2Zz4K);
 --jp-icon-text-editor: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxNiIgdmlld0JveD0iMCAwIDI0IDI0Ij4KICA8cGF0aCBjbGFzcz0ianAtaWNvbjMganAtaWNvbi1zZWxlY3RhYmxlIiBmaWxsPSIjNjE2MTYxIiBkPSJNMTUgMTVIM3YyaDEydi0yem0wLThIM3YyaDEyVjd6TTMgMTNoMTh2LTJIM3Yyem0wIDhoMTh2LTJIM3Yyek0zIDN2MmgxOFYzSDN6Ii8+Cjwvc3ZnPgo=);
 --jp-icon-toc: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIyNCIgaGVpZ2h0PSIyNCIgdmlld0JveD0iMCAwIDI0IDI0Ij4KICA8ZyBjbGFzcz0ianAtaWNvbjMganAtaWNvbi1zZWxlY3RhYmxlIiBmaWxsPSIjNjE2MTYxIj4KICAgIDxwYXRoIGQ9Ik03LDVIMjFWN0g3VjVNNywxM1YxMUgyMVYxM0g3TTQsNC41QTEuNSwxLjUgMCAwLDEgNS41LDZBMS41LDEuNSAwIDAsMSA0LDcuNUExLjUsMS41IDAgMCwxIDIuNSw2QTEuNSwxLjUgMCAwLDEgNCw0LjVNNCwxMC41QTEuNSwxLjUgMCAwLDEgNS41LDEyQTEuNSwxLjUgMCAwLDEgNCwxMy41QTEuNSwxLjUgMCAwLDEgMi41LDEyQTEuNSwxLjUgMCAwLDEgNCwxMC41TTcsMTlWMTdIMjFWMTlIN000LDE2LjVBMS41LDEuNSAwIDAsMSA1LjUsMThBMS41LDEuNSAwIDAsMSA0LDE5LjVBMS41LDEuNSAwIDAsMSAyLjUsMThBMS41LDEuNSAwIDAsMSA0LDE2LjVaIiAvPgogIDwvZz4KPC9zdmc+Cg==);
 --jp-icon-tree-view: url(data:image/svg+xml;base64,PHN2ZyBoZWlnaHQ9IjI0IiB2aWV3Qm94PSIwIDAgMjQgMjQiIHdpZHRoPSIyNCIgeG1sbnM9Imh0dHA6Ly93d3cudzMub3JnLzIwMDAvc3ZnIj4KICAgIDxnIGNsYXNzPSJqcC1pY29uMyIgZmlsbD0iIzYxNjE2MSI+CiAgICAgICAgPHBhdGggZD0iTTAgMGgyNHYyNEgweiIgZmlsbD0ibm9uZSIvPgogICAgICAgIDxwYXRoIGQ9Ik0yMiAxMVYzaC03djNIOVYzSDJ2OGg3VjhoMnYxMGg0djNoN3YtOGgtN3YzaC0yVjhoMnYzeiIvPgogICAgPC9nPgo8L3N2Zz4=);
 --jp-icon-trusted: url(data:image/svg+xml;base64,PHN2ZyBmaWxsPSJub25lIiB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxNiIgdmlld0JveD0iMCAwIDI0IDI1Ij4KICAgIDxwYXRoIGNsYXNzPSJqcC1pY29uMiIgc3Ryb2tlPSIjMzMzMzMzIiBzdHJva2Utd2lkdGg9IjIiIHRyYW5zZm9ybT0idHJhbnNsYXRlKDIgMykiIGQ9Ik0xLjg2MDk0IDExLjQ0MDlDMC44MjY0NDggOC43NzAyNyAwLjg2Mzc3OSA2LjA1NzY0IDEuMjQ5MDcgNC4xOTkzMkMyLjQ4MjA2IDMuOTMzNDcgNC4wODA2OCAzLjQwMzQ3IDUuNjAxMDIgMi44NDQ5QzcuMjM1NDkgMi4yNDQ0IDguODU2NjYgMS41ODE1IDkuOTg3NiAxLjA5NTM5QzExLjA1OTcgMS41ODM0MSAxMi42MDk0IDIuMjQ0NCAxNC4yMTggMi44NDMzOUMxNS43NTAzIDMuNDEzOTQgMTcuMzk5NSAzLjk1MjU4IDE4Ljc1MzkgNC4yMTM4NUMxOS4xMzY0IDYuMDcxNzcgMTkuMTcwOSA4Ljc3NzIyIDE4LjEzOSAxMS40NDA5QzE3LjAzMDMgMTQuMzAzMiAxNC42NjY4IDE3LjE4NDQgOS45OTk5OSAxOC45MzU0QzUuMzMzMiAxNy4xODQ0IDIuOTY5NjggMTQuMzAzMiAxLjg2MDk0IDExLjQ0MDlaIi8+CiAgICA8cGF0aCBjbGFzcz0ianAtaWNvbjIiIGZpbGw9IiMzMzMzMzMiIHN0cm9rZT0iIzMzMzMzMyIgdHJhbnNmb3JtPSJ0cmFuc2xhdGUoOCA5Ljg2NzE5KSIgZD0iTTIuODYwMTUgNC44NjUzNUwwLjcyNjU0OSAyLjk5OTU5TDAgMy42MzA0NUwyLjg2MDE1IDYuMTMxNTdMOCAwLjYzMDg3Mkw3LjI3ODU3IDBMMi44NjAxNSA0Ljg2NTM1WiIvPgo8L3N2Zz4K);
 --jp-icon-undo: url(data:image/svg+xml;base64,PHN2ZyB2aWV3Qm94PSIwIDAgMjQgMjQiIHdpZHRoPSIxNiIgeG1sbnM9Imh0dHA6Ly93d3cudzMub3JnLzIwMDAvc3ZnIj4KICA8ZyBjbGFzcz0ianAtaWNvbjMiIGZpbGw9IiM2MTYxNjEiPgogICAgPHBhdGggZD0iTTEyLjUgOGMtMi42NSAwLTUuMDUuOTktNi45IDIuNkwyIDd2OWg5bC0zLjYyLTMuNjJjMS4zOS0xLjE2IDMuMTYtMS44OCA1LjEyLTEuODggMy41NCAwIDYuNTUgMi4zMSA3LjYgNS41bDIuMzctLjc4QzIxLjA4IDExLjAzIDE3LjE1IDggMTIuNSA4eiIvPgogIDwvZz4KPC9zdmc+Cg==);
 --jp-icon-vega: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxNiIgdmlld0JveD0iMCAwIDIyIDIyIj4KICA8ZyBjbGFzcz0ianAtaWNvbjEganAtaWNvbi1zZWxlY3RhYmxlIiBmaWxsPSIjMjEyMTIxIj4KICAgIDxwYXRoIGQ9Ik0xMC42IDUuNGwyLjItMy4ySDIuMnY3LjNsNC02LjZ6Ii8+CiAgICA8cGF0aCBkPSJNMTUuOCAyLjJsLTQuNCA2LjZMNyA2LjNsLTQuOCA4djUuNWgxNy42VjIuMmgtNHptLTcgMTUuNEg1LjV2LTQuNGgzLjN2NC40em00LjQgMEg5LjhWOS44aDMuNHY3Ljh6bTQuNCAwaC0zLjRWNi41aDMuNHYxMS4xeiIvPgogIDwvZz4KPC9zdmc+Cg==);
 --jp-icon-yaml: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxNiIgdmlld0JveD0iMCAwIDIyIDIyIj4KICA8ZyBjbGFzcz0ianAtaWNvbi1jb250cmFzdDIganAtaWNvbi1zZWxlY3RhYmxlIiBmaWxsPSIjRDgxQjYwIj4KICAgIDxwYXRoIGQ9Ik03LjIgMTguNnYtNS40TDMgNS42aDMuM2wxLjQgMy4xYy4zLjkuNiAxLjYgMSAyLjUuMy0uOC42LTEuNiAxLTIuNWwxLjQtMy4xaDMuNGwtNC40IDcuNnY1LjVsLTIuOS0uMXoiLz4KICAgIDxjaXJjbGUgY2xhc3M9InN0MCIgY3g9IjE3LjYiIGN5PSIxNi41IiByPSIyLjEiLz4KICAgIDxjaXJjbGUgY2xhc3M9InN0MCIgY3g9IjE3LjYiIGN5PSIxMSIgcj0iMi4xIi8+CiAgPC9nPgo8L3N2Zz4K);
}

/\* Icon CSS class declarations \*/

.jp-AddIcon {
 background-image: var(--jp-icon-add);
}
.jp-BugIcon {
 background-image: var(--jp-icon-bug);
}
.jp-BuildIcon {
 background-image: var(--jp-icon-build);
}
.jp-CaretDownEmptyIcon {
 background-image: var(--jp-icon-caret-down-empty);
}
.jp-CaretDownEmptyThinIcon {
 background-image: var(--jp-icon-caret-down-empty-thin);
}
.jp-CaretDownIcon {
 background-image: var(--jp-icon-caret-down);
}
.jp-CaretLeftIcon {
 background-image: var(--jp-icon-caret-left);
}
.jp-CaretRightIcon {
 background-image: var(--jp-icon-caret-right);
}
.jp-CaretUpEmptyThinIcon {
 background-image: var(--jp-icon-caret-up-empty-thin);
}
.jp-CaretUpIcon {
 background-image: var(--jp-icon-caret-up);
}
.jp-CaseSensitiveIcon {
 background-image: var(--jp-icon-case-sensitive);
}
.jp-CheckIcon {
 background-image: var(--jp-icon-check);
}
.jp-CircleEmptyIcon {
 background-image: var(--jp-icon-circle-empty);
}
.jp-CircleIcon {
 background-image: var(--jp-icon-circle);
}
.jp-ClearIcon {
 background-image: var(--jp-icon-clear);
}
.jp-CloseIcon {
 background-image: var(--jp-icon-close);
}
.jp-CodeIcon {
 background-image: var(--jp-icon-code);
}
.jp-ConsoleIcon {
 background-image: var(--jp-icon-console);
}
.jp-CopyIcon {
 background-image: var(--jp-icon-copy);
}
.jp-CopyrightIcon {
 background-image: var(--jp-icon-copyright);
}
.jp-CutIcon {
 background-image: var(--jp-icon-cut);
}
.jp-DownloadIcon {
 background-image: var(--jp-icon-download);
}
.jp-EditIcon {
 background-image: var(--jp-icon-edit);
}
.jp-EllipsesIcon {
 background-image: var(--jp-icon-ellipses);
}
.jp-ExtensionIcon {
 background-image: var(--jp-icon-extension);
}
.jp-FastForwardIcon {
 background-image: var(--jp-icon-fast-forward);
}
.jp-FileIcon {
 background-image: var(--jp-icon-file);
}
.jp-FileUploadIcon {
 background-image: var(--jp-icon-file-upload);
}
.jp-FilterListIcon {
 background-image: var(--jp-icon-filter-list);
}
.jp-FolderIcon {
 background-image: var(--jp-icon-folder);
}
.jp-Html5Icon {
 background-image: var(--jp-icon-html5);
}
.jp-ImageIcon {
 background-image: var(--jp-icon-image);
}
.jp-InspectorIcon {
 background-image: var(--jp-icon-inspector);
}
.jp-JsonIcon {
 background-image: var(--jp-icon-json);
}
.jp-JuliaIcon {
 background-image: var(--jp-icon-julia);
}
.jp-JupyterFaviconIcon {
 background-image: var(--jp-icon-jupyter-favicon);
}
.jp-JupyterIcon {
 background-image: var(--jp-icon-jupyter);
}
.jp-JupyterlabWordmarkIcon {
 background-image: var(--jp-icon-jupyterlab-wordmark);
}
.jp-KernelIcon {
 background-image: var(--jp-icon-kernel);
}
.jp-KeyboardIcon {
 background-image: var(--jp-icon-keyboard);
}
.jp-LauncherIcon {
 background-image: var(--jp-icon-launcher);
}
.jp-LineFormIcon {
 background-image: var(--jp-icon-line-form);
}
.jp-LinkIcon {
 background-image: var(--jp-icon-link);
}
.jp-ListIcon {
 background-image: var(--jp-icon-list);
}
.jp-ListingsInfoIcon {
 background-image: var(--jp-icon-listings-info);
}
.jp-MarkdownIcon {
 background-image: var(--jp-icon-markdown);
}
.jp-NewFolderIcon {
 background-image: var(--jp-icon-new-folder);
}
.jp-NotTrustedIcon {
 background-image: var(--jp-icon-not-trusted);
}
.jp-NotebookIcon {
 background-image: var(--jp-icon-notebook);
}
.jp-NumberingIcon {
 background-image: var(--jp-icon-numbering);
}
.jp-OfflineBoltIcon {
 background-image: var(--jp-icon-offline-bolt);
}
.jp-PaletteIcon {
 background-image: var(--jp-icon-palette);
}
.jp-PasteIcon {
 background-image: var(--jp-icon-paste);
}
.jp-PdfIcon {
 background-image: var(--jp-icon-pdf);
}
.jp-PythonIcon {
 background-image: var(--jp-icon-python);
}
.jp-RKernelIcon {
 background-image: var(--jp-icon-r-kernel);
}
.jp-ReactIcon {
 background-image: var(--jp-icon-react);
}
.jp-RedoIcon {
 background-image: var(--jp-icon-redo);
}
.jp-RefreshIcon {
 background-image: var(--jp-icon-refresh);
}
.jp-RegexIcon {
 background-image: var(--jp-icon-regex);
}
.jp-RunIcon {
 background-image: var(--jp-icon-run);
}
.jp-RunningIcon {
 background-image: var(--jp-icon-running);
}
.jp-SaveIcon {
 background-image: var(--jp-icon-save);
}
.jp-SearchIcon {
 background-image: var(--jp-icon-search);
}
.jp-SettingsIcon {
 background-image: var(--jp-icon-settings);
}
.jp-SpreadsheetIcon {
 background-image: var(--jp-icon-spreadsheet);
}
.jp-StopIcon {
 background-image: var(--jp-icon-stop);
}
.jp-TabIcon {
 background-image: var(--jp-icon-tab);
}
.jp-TableRowsIcon {
 background-image: var(--jp-icon-table-rows);
}
.jp-TagIcon {
 background-image: var(--jp-icon-tag);
}
.jp-TerminalIcon {
 background-image: var(--jp-icon-terminal);
}
.jp-TextEditorIcon {
 background-image: var(--jp-icon-text-editor);
}
.jp-TocIcon {
 background-image: var(--jp-icon-toc);
}
.jp-TreeViewIcon {
 background-image: var(--jp-icon-tree-view);
}
.jp-TrustedIcon {
 background-image: var(--jp-icon-trusted);
}
.jp-UndoIcon {
 background-image: var(--jp-icon-undo);
}
.jp-VegaIcon {
 background-image: var(--jp-icon-vega);
}
.jp-YamlIcon {
 background-image: var(--jp-icon-yaml);
}

/\*-----------------------------------------------------------------------------
| Copyright (c) Jupyter Development Team.
| Distributed under the terms of the Modified BSD License.
|----------------------------------------------------------------------------\*/

/\*\*
 \* (DEPRECATED) Support for consuming icons as CSS background images
 \*/

.jp-Icon,
.jp-MaterialIcon {
 background-position: center;
 background-repeat: no-repeat;
 background-size: 16px;
 min-width: 16px;
 min-height: 16px;
}

.jp-Icon-cover {
 background-position: center;
 background-repeat: no-repeat;
 background-size: cover;
}

/\*\*
 \* (DEPRECATED) Support for specific CSS icon sizes
 \*/

.jp-Icon-16 {
 background-size: 16px;
 min-width: 16px;
 min-height: 16px;
}

.jp-Icon-18 {
 background-size: 18px;
 min-width: 18px;
 min-height: 18px;
}

.jp-Icon-20 {
 background-size: 20px;
 min-width: 20px;
 min-height: 20px;
}

/\*-----------------------------------------------------------------------------
| Copyright (c) Jupyter Development Team.
| Distributed under the terms of the Modified BSD License.
|----------------------------------------------------------------------------\*/

/\*\*
 \* Support for icons as inline SVG HTMLElements
 \*/

/\* recolor the primary elements of an icon \*/
.jp-icon0[fill] {
 fill: var(--jp-inverse-layout-color0);
}
.jp-icon1[fill] {
 fill: var(--jp-inverse-layout-color1);
}
.jp-icon2[fill] {
 fill: var(--jp-inverse-layout-color2);
}
.jp-icon3[fill] {
 fill: var(--jp-inverse-layout-color3);
}
.jp-icon4[fill] {
 fill: var(--jp-inverse-layout-color4);
}

.jp-icon0[stroke] {
 stroke: var(--jp-inverse-layout-color0);
}
.jp-icon1[stroke] {
 stroke: var(--jp-inverse-layout-color1);
}
.jp-icon2[stroke] {
 stroke: var(--jp-inverse-layout-color2);
}
.jp-icon3[stroke] {
 stroke: var(--jp-inverse-layout-color3);
}
.jp-icon4[stroke] {
 stroke: var(--jp-inverse-layout-color4);
}
/\* recolor the accent elements of an icon \*/
.jp-icon-accent0[fill] {
 fill: var(--jp-layout-color0);
}
.jp-icon-accent1[fill] {
 fill: var(--jp-layout-color1);
}
.jp-icon-accent2[fill] {
 fill: var(--jp-layout-color2);
}
.jp-icon-accent3[fill] {
 fill: var(--jp-layout-color3);
}
.jp-icon-accent4[fill] {
 fill: var(--jp-layout-color4);
}

.jp-icon-accent0[stroke] {
 stroke: var(--jp-layout-color0);
}
.jp-icon-accent1[stroke] {
 stroke: var(--jp-layout-color1);
}
.jp-icon-accent2[stroke] {
 stroke: var(--jp-layout-color2);
}
.jp-icon-accent3[stroke] {
 stroke: var(--jp-layout-color3);
}
.jp-icon-accent4[stroke] {
 stroke: var(--jp-layout-color4);
}
/\* set the color of an icon to transparent \*/
.jp-icon-none[fill] {
 fill: none;
}

.jp-icon-none[stroke] {
 stroke: none;
}
/\* brand icon colors. Same for light and dark \*/
.jp-icon-brand0[fill] {
 fill: var(--jp-brand-color0);
}
.jp-icon-brand1[fill] {
 fill: var(--jp-brand-color1);
}
.jp-icon-brand2[fill] {
 fill: var(--jp-brand-color2);
}
.jp-icon-brand3[fill] {
 fill: var(--jp-brand-color3);
}
.jp-icon-brand4[fill] {
 fill: var(--jp-brand-color4);
}

.jp-icon-brand0[stroke] {
 stroke: var(--jp-brand-color0);
}
.jp-icon-brand1[stroke] {
 stroke: var(--jp-brand-color1);
}
.jp-icon-brand2[stroke] {
 stroke: var(--jp-brand-color2);
}
.jp-icon-brand3[stroke] {
 stroke: var(--jp-brand-color3);
}
.jp-icon-brand4[stroke] {
 stroke: var(--jp-brand-color4);
}
/\* warn icon colors. Same for light and dark \*/
.jp-icon-warn0[fill] {
 fill: var(--jp-warn-color0);
}
.jp-icon-warn1[fill] {
 fill: var(--jp-warn-color1);
}
.jp-icon-warn2[fill] {
 fill: var(--jp-warn-color2);
}
.jp-icon-warn3[fill] {
 fill: var(--jp-warn-color3);
}

.jp-icon-warn0[stroke] {
 stroke: var(--jp-warn-color0);
}
.jp-icon-warn1[stroke] {
 stroke: var(--jp-warn-color1);
}
.jp-icon-warn2[stroke] {
 stroke: var(--jp-warn-color2);
}
.jp-icon-warn3[stroke] {
 stroke: var(--jp-warn-color3);
}
/\* icon colors that contrast well with each other and most backgrounds \*/
.jp-icon-contrast0[fill] {
 fill: var(--jp-icon-contrast-color0);
}
.jp-icon-contrast1[fill] {
 fill: var(--jp-icon-contrast-color1);
}
.jp-icon-contrast2[fill] {
 fill: var(--jp-icon-contrast-color2);
}
.jp-icon-contrast3[fill] {
 fill: var(--jp-icon-contrast-color3);
}

.jp-icon-contrast0[stroke] {
 stroke: var(--jp-icon-contrast-color0);
}
.jp-icon-contrast1[stroke] {
 stroke: var(--jp-icon-contrast-color1);
}
.jp-icon-contrast2[stroke] {
 stroke: var(--jp-icon-contrast-color2);
}
.jp-icon-contrast3[stroke] {
 stroke: var(--jp-icon-contrast-color3);
}

/\* CSS for icons in selected items in the settings editor \*/
#setting-editor .jp-PluginList .jp-mod-selected .jp-icon-selectable[fill] {
 fill: #fff;
}
#setting-editor
 .jp-PluginList
 .jp-mod-selected
 .jp-icon-selectable-inverse[fill] {
 fill: var(--jp-brand-color1);
}

/\* CSS for icons in selected filebrowser listing items \*/
.jp-DirListing-item.jp-mod-selected .jp-icon-selectable[fill] {
 fill: #fff;
}
.jp-DirListing-item.jp-mod-selected .jp-icon-selectable-inverse[fill] {
 fill: var(--jp-brand-color1);
}

/\* CSS for icons in selected tabs in the sidebar tab manager \*/
#tab-manager .lm-TabBar-tab.jp-mod-active .jp-icon-selectable[fill] {
 fill: #fff;
}

#tab-manager .lm-TabBar-tab.jp-mod-active .jp-icon-selectable-inverse[fill] {
 fill: var(--jp-brand-color1);
}
#tab-manager
 .lm-TabBar-tab.jp-mod-active
 .jp-icon-hover
 :hover
 .jp-icon-selectable[fill] {
 fill: var(--jp-brand-color1);
}

#tab-manager
 .lm-TabBar-tab.jp-mod-active
 .jp-icon-hover
 :hover
 .jp-icon-selectable-inverse[fill] {
 fill: #fff;
}

/\*\*
 \* TODO: come up with non css-hack solution for showing the busy icon on top
 \* of the close icon
 \* CSS for complex behavior of close icon of tabs in the sidebar tab manager
 \*/
#tab-manager
 .lm-TabBar-tab.jp-mod-dirty
 > .lm-TabBar-tabCloseIcon
 > :not(:hover)
 > .jp-icon3[fill] {
 fill: none;
}
#tab-manager
 .lm-TabBar-tab.jp-mod-dirty
 > .lm-TabBar-tabCloseIcon
 > :not(:hover)
 > .jp-icon-busy[fill] {
 fill: var(--jp-inverse-layout-color3);
}

#tab-manager
 .lm-TabBar-tab.jp-mod-dirty.jp-mod-active
 > .lm-TabBar-tabCloseIcon
 > :not(:hover)
 > .jp-icon-busy[fill] {
 fill: #fff;
}

/\*\*
\* TODO: come up with non css-hack solution for showing the busy icon on top
\* of the close icon
\* CSS for complex behavior of close icon of tabs in the main area tabbar
\*/
.lm-DockPanel-tabBar
 .lm-TabBar-tab.lm-mod-closable.jp-mod-dirty
 > .lm-TabBar-tabCloseIcon
 > :not(:hover)
 > .jp-icon3[fill] {
 fill: none;
}
.lm-DockPanel-tabBar
 .lm-TabBar-tab.lm-mod-closable.jp-mod-dirty
 > .lm-TabBar-tabCloseIcon
 > :not(:hover)
 > .jp-icon-busy[fill] {
 fill: var(--jp-inverse-layout-color3);
}

/\* CSS for icons in status bar \*/
#jp-main-statusbar .jp-mod-selected .jp-icon-selectable[fill] {
 fill: #fff;
}

#jp-main-statusbar .jp-mod-selected .jp-icon-selectable-inverse[fill] {
 fill: var(--jp-brand-color1);
}
/\* special handling for splash icon CSS. While the theme CSS reloads during
 splash, the splash icon can loose theming. To prevent that, we set a
 default for its color variable \*/
:root {
 --jp-warn-color0: var(--md-orange-700);
}

/\* not sure what to do with this one, used in filebrowser listing \*/
.jp-DragIcon {
 margin-right: 4px;
}

/\*-----------------------------------------------------------------------------
| Copyright (c) Jupyter Development Team.
| Distributed under the terms of the Modified BSD License.
|----------------------------------------------------------------------------\*/

/\*\*
 \* Support for alt colors for icons as inline SVG HTMLElements
 \*/

/\* alt recolor the primary elements of an icon \*/
.jp-icon-alt .jp-icon0[fill] {
 fill: var(--jp-layout-color0);
}
.jp-icon-alt .jp-icon1[fill] {
 fill: var(--jp-layout-color1);
}
.jp-icon-alt .jp-icon2[fill] {
 fill: var(--jp-layout-color2);
}
.jp-icon-alt .jp-icon3[fill] {
 fill: var(--jp-layout-color3);
}
.jp-icon-alt .jp-icon4[fill] {
 fill: var(--jp-layout-color4);
}

.jp-icon-alt .jp-icon0[stroke] {
 stroke: var(--jp-layout-color0);
}
.jp-icon-alt .jp-icon1[stroke] {
 stroke: var(--jp-layout-color1);
}
.jp-icon-alt .jp-icon2[stroke] {
 stroke: var(--jp-layout-color2);
}
.jp-icon-alt .jp-icon3[stroke] {
 stroke: var(--jp-layout-color3);
}
.jp-icon-alt .jp-icon4[stroke] {
 stroke: var(--jp-layout-color4);
}

/\* alt recolor the accent elements of an icon \*/
.jp-icon-alt .jp-icon-accent0[fill] {
 fill: var(--jp-inverse-layout-color0);
}
.jp-icon-alt .jp-icon-accent1[fill] {
 fill: var(--jp-inverse-layout-color1);
}
.jp-icon-alt .jp-icon-accent2[fill] {
 fill: var(--jp-inverse-layout-color2);
}
.jp-icon-alt .jp-icon-accent3[fill] {
 fill: var(--jp-inverse-layout-color3);
}
.jp-icon-alt .jp-icon-accent4[fill] {
 fill: var(--jp-inverse-layout-color4);
}

.jp-icon-alt .jp-icon-accent0[stroke] {
 stroke: var(--jp-inverse-layout-color0);
}
.jp-icon-alt .jp-icon-accent1[stroke] {
 stroke: var(--jp-inverse-layout-color1);
}
.jp-icon-alt .jp-icon-accent2[stroke] {
 stroke: var(--jp-inverse-layout-color2);
}
.jp-icon-alt .jp-icon-accent3[stroke] {
 stroke: var(--jp-inverse-layout-color3);
}
.jp-icon-alt .jp-icon-accent4[stroke] {
 stroke: var(--jp-inverse-layout-color4);
}

/\*-----------------------------------------------------------------------------
| Copyright (c) Jupyter Development Team.
| Distributed under the terms of the Modified BSD License.
|----------------------------------------------------------------------------\*/

.jp-icon-hoverShow:not(:hover) svg {
 display: none !important;
}

/\*\*
 \* Support for hover colors for icons as inline SVG HTMLElements
 \*/

/\*\*
 \* regular colors
 \*/

/\* recolor the primary elements of an icon \*/
.jp-icon-hover :hover .jp-icon0-hover[fill] {
 fill: var(--jp-inverse-layout-color0);
}
.jp-icon-hover :hover .jp-icon1-hover[fill] {
 fill: var(--jp-inverse-layout-color1);
}
.jp-icon-hover :hover .jp-icon2-hover[fill] {
 fill: var(--jp-inverse-layout-color2);
}
.jp-icon-hover :hover .jp-icon3-hover[fill] {
 fill: var(--jp-inverse-layout-color3);
}
.jp-icon-hover :hover .jp-icon4-hover[fill] {
 fill: var(--jp-inverse-layout-color4);
}

.jp-icon-hover :hover .jp-icon0-hover[stroke] {
 stroke: var(--jp-inverse-layout-color0);
}
.jp-icon-hover :hover .jp-icon1-hover[stroke] {
 stroke: var(--jp-inverse-layout-color1);
}
.jp-icon-hover :hover .jp-icon2-hover[stroke] {
 stroke: var(--jp-inverse-layout-color2);
}
.jp-icon-hover :hover .jp-icon3-hover[stroke] {
 stroke: var(--jp-inverse-layout-color3);
}
.jp-icon-hover :hover .jp-icon4-hover[stroke] {
 stroke: var(--jp-inverse-layout-color4);
}

/\* recolor the accent elements of an icon \*/
.jp-icon-hover :hover .jp-icon-accent0-hover[fill] {
 fill: var(--jp-layout-color0);
}
.jp-icon-hover :hover .jp-icon-accent1-hover[fill] {
 fill: var(--jp-layout-color1);
}
.jp-icon-hover :hover .jp-icon-accent2-hover[fill] {
 fill: var(--jp-layout-color2);
}
.jp-icon-hover :hover .jp-icon-accent3-hover[fill] {
 fill: var(--jp-layout-color3);
}
.jp-icon-hover :hover .jp-icon-accent4-hover[fill] {
 fill: var(--jp-layout-color4);
}

.jp-icon-hover :hover .jp-icon-accent0-hover[stroke] {
 stroke: var(--jp-layout-color0);
}
.jp-icon-hover :hover .jp-icon-accent1-hover[stroke] {
 stroke: var(--jp-layout-color1);
}
.jp-icon-hover :hover .jp-icon-accent2-hover[stroke] {
 stroke: var(--jp-layout-color2);
}
.jp-icon-hover :hover .jp-icon-accent3-hover[stroke] {
 stroke: var(--jp-layout-color3);
}
.jp-icon-hover :hover .jp-icon-accent4-hover[stroke] {
 stroke: var(--jp-layout-color4);
}

/\* set the color of an icon to transparent \*/
.jp-icon-hover :hover .jp-icon-none-hover[fill] {
 fill: none;
}

.jp-icon-hover :hover .jp-icon-none-hover[stroke] {
 stroke: none;
}

/\*\*
 \* inverse colors
 \*/

/\* inverse recolor the primary elements of an icon \*/
.jp-icon-hover.jp-icon-alt :hover .jp-icon0-hover[fill] {
 fill: var(--jp-layout-color0);
}
.jp-icon-hover.jp-icon-alt :hover .jp-icon1-hover[fill] {
 fill: var(--jp-layout-color1);
}
.jp-icon-hover.jp-icon-alt :hover .jp-icon2-hover[fill] {
 fill: var(--jp-layout-color2);
}
.jp-icon-hover.jp-icon-alt :hover .jp-icon3-hover[fill] {
 fill: var(--jp-layout-color3);
}
.jp-icon-hover.jp-icon-alt :hover .jp-icon4-hover[fill] {
 fill: var(--jp-layout-color4);
}

.jp-icon-hover.jp-icon-alt :hover .jp-icon0-hover[stroke] {
 stroke: var(--jp-layout-color0);
}
.jp-icon-hover.jp-icon-alt :hover .jp-icon1-hover[stroke] {
 stroke: var(--jp-layout-color1);
}
.jp-icon-hover.jp-icon-alt :hover .jp-icon2-hover[stroke] {
 stroke: var(--jp-layout-color2);
}
.jp-icon-hover.jp-icon-alt :hover .jp-icon3-hover[stroke] {
 stroke: var(--jp-layout-color3);
}
.jp-icon-hover.jp-icon-alt :hover .jp-icon4-hover[stroke] {
 stroke: var(--jp-layout-color4);
}

/\* inverse recolor the accent elements of an icon \*/
.jp-icon-hover.jp-icon-alt :hover .jp-icon-accent0-hover[fill] {
 fill: var(--jp-inverse-layout-color0);
}
.jp-icon-hover.jp-icon-alt :hover .jp-icon-accent1-hover[fill] {
 fill: var(--jp-inverse-layout-color1);
}
.jp-icon-hover.jp-icon-alt :hover .jp-icon-accent2-hover[fill] {
 fill: var(--jp-inverse-layout-color2);
}
.jp-icon-hover.jp-icon-alt :hover .jp-icon-accent3-hover[fill] {
 fill: var(--jp-inverse-layout-color3);
}
.jp-icon-hover.jp-icon-alt :hover .jp-icon-accent4-hover[fill] {
 fill: var(--jp-inverse-layout-color4);
}

.jp-icon-hover.jp-icon-alt :hover .jp-icon-accent0-hover[stroke] {
 stroke: var(--jp-inverse-layout-color0);
}
.jp-icon-hover.jp-icon-alt :hover .jp-icon-accent1-hover[stroke] {
 stroke: var(--jp-inverse-layout-color1);
}
.jp-icon-hover.jp-icon-alt :hover .jp-icon-accent2-hover[stroke] {
 stroke: var(--jp-inverse-layout-color2);
}
.jp-icon-hover.jp-icon-alt :hover .jp-icon-accent3-hover[stroke] {
 stroke: var(--jp-inverse-layout-color3);
}
.jp-icon-hover.jp-icon-alt :hover .jp-icon-accent4-hover[stroke] {
 stroke: var(--jp-inverse-layout-color4);
}

/\*-----------------------------------------------------------------------------
| Copyright (c) Jupyter Development Team.
| Distributed under the terms of the Modified BSD License.
|----------------------------------------------------------------------------\*/

.jp-switch {
 display: flex;
 align-items: center;
 padding-left: 4px;
 padding-right: 4px;
 font-size: var(--jp-ui-font-size1);
 background-color: transparent;
 color: var(--jp-ui-font-color1);
 border: none;
 height: 20px;
}

.jp-switch:hover {
 background-color: var(--jp-layout-color2);
}

.jp-switch-label {
 margin-right: 5px;
}

.jp-switch-track {
 cursor: pointer;
 background-color: var(--jp-border-color1);
 -webkit-transition: 0.4s;
 transition: 0.4s;
 border-radius: 34px;
 height: 16px;
 width: 35px;
 position: relative;
}

.jp-switch-track::before {
 content: '';
 position: absolute;
 height: 10px;
 width: 10px;
 margin: 3px;
 left: 0px;
 background-color: var(--jp-ui-inverse-font-color1);
 -webkit-transition: 0.4s;
 transition: 0.4s;
 border-radius: 50%;
}

.jp-switch[aria-checked='true'] .jp-switch-track {
 background-color: var(--jp-warn-color0);
}

.jp-switch[aria-checked='true'] .jp-switch-track::before {
 /\* track width (35) - margins (3 + 3) - thumb width (10) \*/
 left: 19px;
}

/\*-----------------------------------------------------------------------------
| Copyright (c) Jupyter Development Team.
| Distributed under the terms of the Modified BSD License.
|----------------------------------------------------------------------------\*/

/\* Sibling imports \*/

/\* Override Blueprint's \_reset.scss styles \*/
html {
 box-sizing: unset;
}

\*,
\*::before,
\*::after {
 box-sizing: unset;
}

body {
 color: unset;
 font-family: var(--jp-ui-font-family);
}

p {
 margin-top: unset;
 margin-bottom: unset;
}

small {
 font-size: unset;
}

strong {
 font-weight: unset;
}

/\* Override Blueprint's \_typography.scss styles \*/
a {
 text-decoration: unset;
 color: unset;
}
a:hover {
 text-decoration: unset;
 color: unset;
}

/\* Override Blueprint's \_accessibility.scss styles \*/
:focus {
 outline: unset;
 outline-offset: unset;
 -moz-outline-radius: unset;
}

/\* Styles for ui-components \*/
.jp-Button {
 border-radius: var(--jp-border-radius);
 padding: 0px 12px;
 font-size: var(--jp-ui-font-size1);
}

/\* Use our own theme for hover styles \*/
button.jp-Button.bp3-button.bp3-minimal:hover {
 background-color: var(--jp-layout-color2);
}
.jp-Button.minimal {
 color: unset !important;
}

.jp-Button.jp-ToolbarButtonComponent {
 text-transform: none;
}

.jp-InputGroup input {
 box-sizing: border-box;
 border-radius: 0;
 background-color: transparent;
 color: var(--jp-ui-font-color0);
 box-shadow: inset 0 0 0 var(--jp-border-width) var(--jp-input-border-color);
}

.jp-InputGroup input:focus {
 box-shadow: inset 0 0 0 var(--jp-border-width)
 var(--jp-input-active-box-shadow-color),
 inset 0 0 0 3px var(--jp-input-active-box-shadow-color);
}

.jp-InputGroup input::placeholder,
input::placeholder {
 color: var(--jp-ui-font-color3);
}

.jp-BPIcon {
 display: inline-block;
 vertical-align: middle;
 margin: auto;
}

/\* Stop blueprint futzing with our icon fills \*/
.bp3-icon.jp-BPIcon > svg:not([fill]) {
 fill: var(--jp-inverse-layout-color3);
}

.jp-InputGroupAction {
 padding: 6px;
}

.jp-HTMLSelect.jp-DefaultStyle select {
 background-color: initial;
 border: none;
 border-radius: 0;
 box-shadow: none;
 color: var(--jp-ui-font-color0);
 display: block;
 font-size: var(--jp-ui-font-size1);
 height: 24px;
 line-height: 14px;
 padding: 0 25px 0 10px;
 text-align: left;
 -moz-appearance: none;
 -webkit-appearance: none;
}

/\* Use our own theme for hover and option styles \*/
.jp-HTMLSelect.jp-DefaultStyle select:hover,
.jp-HTMLSelect.jp-DefaultStyle select > option {
 background-color: var(--jp-layout-color2);
 color: var(--jp-ui-font-color0);
}
select {
 box-sizing: border-box;
}

/\*-----------------------------------------------------------------------------
| Copyright (c) Jupyter Development Team.
| Distributed under the terms of the Modified BSD License.
|----------------------------------------------------------------------------\*/

.jp-Collapse {
 display: flex;
 flex-direction: column;
 align-items: stretch;
 border-top: 1px solid var(--jp-border-color2);
 border-bottom: 1px solid var(--jp-border-color2);
}

.jp-Collapse-header {
 padding: 1px 12px;
 color: var(--jp-ui-font-color1);
 background-color: var(--jp-layout-color1);
 font-size: var(--jp-ui-font-size2);
}

.jp-Collapse-header:hover {
 background-color: var(--jp-layout-color2);
}

.jp-Collapse-contents {
 padding: 0px 12px 0px 12px;
 background-color: var(--jp-layout-color1);
 color: var(--jp-ui-font-color1);
 overflow: auto;
}

/\*-----------------------------------------------------------------------------
| Copyright (c) Jupyter Development Team.
| Distributed under the terms of the Modified BSD License.
|----------------------------------------------------------------------------\*/

/\*-----------------------------------------------------------------------------
| Variables
|----------------------------------------------------------------------------\*/

:root {
 --jp-private-commandpalette-search-height: 28px;
}

/\*-----------------------------------------------------------------------------
| Overall styles
|----------------------------------------------------------------------------\*/

.lm-CommandPalette {
 padding-bottom: 0px;
 color: var(--jp-ui-font-color1);
 background: var(--jp-layout-color1);
 /\* This is needed so that all font sizing of children done in ems is
 \* relative to this base size \*/
 font-size: var(--jp-ui-font-size1);
}

/\*-----------------------------------------------------------------------------
| Modal variant
|----------------------------------------------------------------------------\*/

.jp-ModalCommandPalette {
 position: absolute;
 z-index: 10000;
 top: 38px;
 left: 30%;
 margin: 0;
 padding: 4px;
 width: 40%;
 box-shadow: var(--jp-elevation-z4);
 border-radius: 4px;
 background: var(--jp-layout-color0);
}

.jp-ModalCommandPalette .lm-CommandPalette {
 max-height: 40vh;
}

.jp-ModalCommandPalette .lm-CommandPalette .lm-close-icon::after {
 display: none;
}

.jp-ModalCommandPalette .lm-CommandPalette .lm-CommandPalette-header {
 display: none;
}

.jp-ModalCommandPalette .lm-CommandPalette .lm-CommandPalette-item {
 margin-left: 4px;
 margin-right: 4px;
}

.jp-ModalCommandPalette
 .lm-CommandPalette
 .lm-CommandPalette-item.lm-mod-disabled {
 display: none;
}

/\*-----------------------------------------------------------------------------
| Search
|----------------------------------------------------------------------------\*/

.lm-CommandPalette-search {
 padding: 4px;
 background-color: var(--jp-layout-color1);
 z-index: 2;
}

.lm-CommandPalette-wrapper {
 overflow: overlay;
 padding: 0px 9px;
 background-color: var(--jp-input-active-background);
 height: 30px;
 box-shadow: inset 0 0 0 var(--jp-border-width) var(--jp-input-border-color);
}

.lm-CommandPalette.lm-mod-focused .lm-CommandPalette-wrapper {
 box-shadow: inset 0 0 0 1px var(--jp-input-active-box-shadow-color),
 inset 0 0 0 3px var(--jp-input-active-box-shadow-color);
}

.jp-SearchIconGroup {
 color: white;
 background-color: var(--jp-brand-color1);
 position: absolute;
 top: 4px;
 right: 4px;
 padding: 5px 5px 1px 5px;
}

.jp-SearchIconGroup svg {
 height: 20px;
 width: 20px;
}

.jp-SearchIconGroup .jp-icon3[fill] {
 fill: var(--jp-layout-color0);
}

.lm-CommandPalette-input {
 background: transparent;
 width: calc(100% - 18px);
 float: left;
 border: none;
 outline: none;
 font-size: var(--jp-ui-font-size1);
 color: var(--jp-ui-font-color0);
 line-height: var(--jp-private-commandpalette-search-height);
}

.lm-CommandPalette-input::-webkit-input-placeholder,
.lm-CommandPalette-input::-moz-placeholder,
.lm-CommandPalette-input:-ms-input-placeholder {
 color: var(--jp-ui-font-color2);
 font-size: var(--jp-ui-font-size1);
}

/\*-----------------------------------------------------------------------------
| Results
|----------------------------------------------------------------------------\*/

.lm-CommandPalette-header:first-child {
 margin-top: 0px;
}

.lm-CommandPalette-header {
 border-bottom: solid var(--jp-border-width) var(--jp-border-color2);
 color: var(--jp-ui-font-color1);
 cursor: pointer;
 display: flex;
 font-size: var(--jp-ui-font-size0);
 font-weight: 600;
 letter-spacing: 1px;
 margin-top: 8px;
 padding: 8px 0 8px 12px;
 text-transform: uppercase;
}

.lm-CommandPalette-header.lm-mod-active {
 background: var(--jp-layout-color2);
}

.lm-CommandPalette-header > mark {
 background-color: transparent;
 font-weight: bold;
 color: var(--jp-ui-font-color1);
}

.lm-CommandPalette-item {
 padding: 4px 12px 4px 4px;
 color: var(--jp-ui-font-color1);
 font-size: var(--jp-ui-font-size1);
 font-weight: 400;
 display: flex;
}

.lm-CommandPalette-item.lm-mod-disabled {
 color: var(--jp-ui-font-color2);
}

.lm-CommandPalette-item.lm-mod-active {
 color: var(--jp-ui-inverse-font-color1);
 background: var(--jp-brand-color1);
}

.lm-CommandPalette-item.lm-mod-active .lm-CommandPalette-itemLabel > mark {
 color: var(--jp-ui-inverse-font-color0);
}

.lm-CommandPalette-item.lm-mod-active .jp-icon-selectable[fill] {
 fill: var(--jp-layout-color0);
}

.lm-CommandPalette-item.lm-mod-active .lm-CommandPalette-itemLabel > mark {
 color: var(--jp-ui-inverse-font-color0);
}

.lm-CommandPalette-item.lm-mod-active:hover:not(.lm-mod-disabled) {
 color: var(--jp-ui-inverse-font-color1);
 background: var(--jp-brand-color1);
}

.lm-CommandPalette-item:hover:not(.lm-mod-active):not(.lm-mod-disabled) {
 background: var(--jp-layout-color2);
}

.lm-CommandPalette-itemContent {
 overflow: hidden;
}

.lm-CommandPalette-itemLabel > mark {
 color: var(--jp-ui-font-color0);
 background-color: transparent;
 font-weight: bold;
}

.lm-CommandPalette-item.lm-mod-disabled mark {
 color: var(--jp-ui-font-color2);
}

.lm-CommandPalette-item .lm-CommandPalette-itemIcon {
 margin: 0 4px 0 0;
 position: relative;
 width: 16px;
 top: 2px;
 flex: 0 0 auto;
}

.lm-CommandPalette-item.lm-mod-disabled .lm-CommandPalette-itemIcon {
 opacity: 0.6;
}

.lm-CommandPalette-item .lm-CommandPalette-itemShortcut {
 flex: 0 0 auto;
}

.lm-CommandPalette-itemCaption {
 display: none;
}

.lm-CommandPalette-content {
 background-color: var(--jp-layout-color1);
}

.lm-CommandPalette-content:empty:after {
 content: 'No results';
 margin: auto;
 margin-top: 20px;
 width: 100px;
 display: block;
 font-size: var(--jp-ui-font-size2);
 font-family: var(--jp-ui-font-family);
 font-weight: lighter;
}

.lm-CommandPalette-emptyMessage {
 text-align: center;
 margin-top: 24px;
 line-height: 1.32;
 padding: 0px 8px;
 color: var(--jp-content-font-color3);
}

/\*-----------------------------------------------------------------------------
| Copyright (c) 2014-2017, Jupyter Development Team.
|
| Distributed under the terms of the Modified BSD License.
|----------------------------------------------------------------------------\*/

.jp-Dialog {
 position: absolute;
 z-index: 10000;
 display: flex;
 flex-direction: column;
 align-items: center;
 justify-content: center;
 top: 0px;
 left: 0px;
 margin: 0;
 padding: 0;
 width: 100%;
 height: 100%;
 background: var(--jp-dialog-background);
}

.jp-Dialog-content {
 display: flex;
 flex-direction: column;
 margin-left: auto;
 margin-right: auto;
 background: var(--jp-layout-color1);
 padding: 24px;
 padding-bottom: 12px;
 min-width: 300px;
 min-height: 150px;
 max-width: 1000px;
 max-height: 500px;
 box-sizing: border-box;
 box-shadow: var(--jp-elevation-z20);
 word-wrap: break-word;
 border-radius: var(--jp-border-radius);
 /\* This is needed so that all font sizing of children done in ems is
 \* relative to this base size \*/
 font-size: var(--jp-ui-font-size1);
 color: var(--jp-ui-font-color1);
 resize: both;
}

.jp-Dialog-button {
 overflow: visible;
}

button.jp-Dialog-button:focus {
 outline: 1px solid var(--jp-brand-color1);
 outline-offset: 4px;
 -moz-outline-radius: 0px;
}

button.jp-Dialog-button:focus::-moz-focus-inner {
 border: 0;
}

button.jp-Dialog-close-button {
 padding: 0;
 height: 100%;
 min-width: unset;
 min-height: unset;
}

.jp-Dialog-header {
 display: flex;
 justify-content: space-between;
 flex: 0 0 auto;
 padding-bottom: 12px;
 font-size: var(--jp-ui-font-size3);
 font-weight: 400;
 color: var(--jp-ui-font-color0);
}

.jp-Dialog-body {
 display: flex;
 flex-direction: column;
 flex: 1 1 auto;
 font-size: var(--jp-ui-font-size1);
 background: var(--jp-layout-color1);
 overflow: auto;
}

.jp-Dialog-footer {
 display: flex;
 flex-direction: row;
 justify-content: flex-end;
 flex: 0 0 auto;
 margin-left: -12px;
 margin-right: -12px;
 padding: 12px;
}

.jp-Dialog-title {
 overflow: hidden;
 white-space: nowrap;
 text-overflow: ellipsis;
}

.jp-Dialog-body > .jp-select-wrapper {
 width: 100%;
}

.jp-Dialog-body > button {
 padding: 0px 16px;
}

.jp-Dialog-body > label {
 line-height: 1.4;
 color: var(--jp-ui-font-color0);
}

.jp-Dialog-button.jp-mod-styled:not(:last-child) {
 margin-right: 12px;
}

/\*-----------------------------------------------------------------------------
| Copyright (c) 2014-2016, Jupyter Development Team.
|
| Distributed under the terms of the Modified BSD License.
|----------------------------------------------------------------------------\*/

.jp-HoverBox {
 position: fixed;
}

.jp-HoverBox.jp-mod-outofview {
 display: none;
}

/\*-----------------------------------------------------------------------------
| Copyright (c) Jupyter Development Team.
| Distributed under the terms of the Modified BSD License.
|----------------------------------------------------------------------------\*/

.jp-IFrame {
 width: 100%;
 height: 100%;
}

.jp-IFrame > iframe {
 border: none;
}

/\*
When drag events occur, `p-mod-override-cursor` is added to the body.
Because iframes steal all cursor events, the following two rules are necessary
to suppress pointer events while resize drags are occurring. There may be a
better solution to this problem.
\*/
body.lm-mod-override-cursor .jp-IFrame {
 position: relative;
}

body.lm-mod-override-cursor .jp-IFrame:before {
 content: '';
 position: absolute;
 top: 0;
 left: 0;
 right: 0;
 bottom: 0;
 background: transparent;
}

.jp-Input-Boolean-Dialog {
 flex-direction: row-reverse;
 align-items: end;
 width: 100%;
}

.jp-Input-Boolean-Dialog > label {
 flex: 1 1 auto;
}

/\*-----------------------------------------------------------------------------
| Copyright (c) 2014-2016, Jupyter Development Team.
|
| Distributed under the terms of the Modified BSD License.
|----------------------------------------------------------------------------\*/

.jp-MainAreaWidget > :focus {
 outline: none;
}

/\*\*
 \* google-material-color v1.2.6
 \* https://github.com/danlevan/google-material-color
 \*/
:root {
 --md-red-50: #ffebee;
 --md-red-100: #ffcdd2;
 --md-red-200: #ef9a9a;
 --md-red-300: #e57373;
 --md-red-400: #ef5350;
 --md-red-500: #f44336;
 --md-red-600: #e53935;
 --md-red-700: #d32f2f;
 --md-red-800: #c62828;
 --md-red-900: #b71c1c;
 --md-red-A100: #ff8a80;
 --md-red-A200: #ff5252;
 --md-red-A400: #ff1744;
 --md-red-A700: #d50000;

 --md-pink-50: #fce4ec;
 --md-pink-100: #f8bbd0;
 --md-pink-200: #f48fb1;
 --md-pink-300: #f06292;
 --md-pink-400: #ec407a;
 --md-pink-500: #e91e63;
 --md-pink-600: #d81b60;
 --md-pink-700: #c2185b;
 --md-pink-800: #ad1457;
 --md-pink-900: #880e4f;
 --md-pink-A100: #ff80ab;
 --md-pink-A200: #ff4081;
 --md-pink-A400: #f50057;
 --md-pink-A700: #c51162;

 --md-purple-50: #f3e5f5;
 --md-purple-100: #e1bee7;
 --md-purple-200: #ce93d8;
 --md-purple-300: #ba68c8;
 --md-purple-400: #ab47bc;
 --md-purple-500: #9c27b0;
 --md-purple-600: #8e24aa;
 --md-purple-700: #7b1fa2;
 --md-purple-800: #6a1b9a;
 --md-purple-900: #4a148c;
 --md-purple-A100: #ea80fc;
 --md-purple-A200: #e040fb;
 --md-purple-A400: #d500f9;
 --md-purple-A700: #aa00ff;

 --md-deep-purple-50: #ede7f6;
 --md-deep-purple-100: #d1c4e9;
 --md-deep-purple-200: #b39ddb;
 --md-deep-purple-300: #9575cd;
 --md-deep-purple-400: #7e57c2;
 --md-deep-purple-500: #673ab7;
 --md-deep-purple-600: #5e35b1;
 --md-deep-purple-700: #512da8;
 --md-deep-purple-800: #4527a0;
 --md-deep-purple-900: #311b92;
 --md-deep-purple-A100: #b388ff;
 --md-deep-purple-A200: #7c4dff;
 --md-deep-purple-A400: #651fff;
 --md-deep-purple-A700: #6200ea;

 --md-indigo-50: #e8eaf6;
 --md-indigo-100: #c5cae9;
 --md-indigo-200: #9fa8da;
 --md-indigo-300: #7986cb;
 --md-indigo-400: #5c6bc0;
 --md-indigo-500: #3f51b5;
 --md-indigo-600: #3949ab;
 --md-indigo-700: #303f9f;
 --md-indigo-800: #283593;
 --md-indigo-900: #1a237e;
 --md-indigo-A100: #8c9eff;
 --md-indigo-A200: #536dfe;
 --md-indigo-A400: #3d5afe;
 --md-indigo-A700: #304ffe;

 --md-blue-50: #e3f2fd;
 --md-blue-100: #bbdefb;
 --md-blue-200: #90caf9;
 --md-blue-300: #64b5f6;
 --md-blue-400: #42a5f5;
 --md-blue-500: #2196f3;
 --md-blue-600: #1e88e5;
 --md-blue-700: #1976d2;
 --md-blue-800: #1565c0;
 --md-blue-900: #0d47a1;
 --md-blue-A100: #82b1ff;
 --md-blue-A200: #448aff;
 --md-blue-A400: #2979ff;
 --md-blue-A700: #2962ff;

 --md-light-blue-50: #e1f5fe;
 --md-light-blue-100: #b3e5fc;
 --md-light-blue-200: #81d4fa;
 --md-light-blue-300: #4fc3f7;
 --md-light-blue-400: #29b6f6;
 --md-light-blue-500: #03a9f4;
 --md-light-blue-600: #039be5;
 --md-light-blue-700: #0288d1;
 --md-light-blue-800: #0277bd;
 --md-light-blue-900: #01579b;
 --md-light-blue-A100: #80d8ff;
 --md-light-blue-A200: #40c4ff;
 --md-light-blue-A400: #00b0ff;
 --md-light-blue-A700: #0091ea;

 --md-cyan-50: #e0f7fa;
 --md-cyan-100: #b2ebf2;
 --md-cyan-200: #80deea;
 --md-cyan-300: #4dd0e1;
 --md-cyan-400: #26c6da;
 --md-cyan-500: #00bcd4;
 --md-cyan-600: #00acc1;
 --md-cyan-700: #0097a7;
 --md-cyan-800: #00838f;
 --md-cyan-900: #006064;
 --md-cyan-A100: #84ffff;
 --md-cyan-A200: #18ffff;
 --md-cyan-A400: #00e5ff;
 --md-cyan-A700: #00b8d4;

 --md-teal-50: #e0f2f1;
 --md-teal-100: #b2dfdb;
 --md-teal-200: #80cbc4;
 --md-teal-300: #4db6ac;
 --md-teal-400: #26a69a;
 --md-teal-500: #009688;
 --md-teal-600: #00897b;
 --md-teal-700: #00796b;
 --md-teal-800: #00695c;
 --md-teal-900: #004d40;
 --md-teal-A100: #a7ffeb;
 --md-teal-A200: #64ffda;
 --md-teal-A400: #1de9b6;
 --md-teal-A700: #00bfa5;

 --md-green-50: #e8f5e9;
 --md-green-100: #c8e6c9;
 --md-green-200: #a5d6a7;
 --md-green-300: #81c784;
 --md-green-400: #66bb6a;
 --md-green-500: #4caf50;
 --md-green-600: #43a047;
 --md-green-700: #388e3c;
 --md-green-800: #2e7d32;
 --md-green-900: #1b5e20;
 --md-green-A100: #b9f6ca;
 --md-green-A200: #69f0ae;
 --md-green-A400: #00e676;
 --md-green-A700: #00c853;

 --md-light-green-50: #f1f8e9;
 --md-light-green-100: #dcedc8;
 --md-light-green-200: #c5e1a5;
 --md-light-green-300: #aed581;
 --md-light-green-400: #9ccc65;
 --md-light-green-500: #8bc34a;
 --md-light-green-600: #7cb342;
 --md-light-green-700: #689f38;
 --md-light-green-800: #558b2f;
 --md-light-green-900: #33691e;
 --md-light-green-A100: #ccff90;
 --md-light-green-A200: #b2ff59;
 --md-light-green-A400: #76ff03;
 --md-light-green-A700: #64dd17;

 --md-lime-50: #f9fbe7;
 --md-lime-100: #f0f4c3;
 --md-lime-200: #e6ee9c;
 --md-lime-300: #dce775;
 --md-lime-400: #d4e157;
 --md-lime-500: #cddc39;
 --md-lime-600: #c0ca33;
 --md-lime-700: #afb42b;
 --md-lime-800: #9e9d24;
 --md-lime-900: #827717;
 --md-lime-A100: #f4ff81;
 --md-lime-A200: #eeff41;
 --md-lime-A400: #c6ff00;
 --md-lime-A700: #aeea00;

 --md-yellow-50: #fffde7;
 --md-yellow-100: #fff9c4;
 --md-yellow-200: #fff59d;
 --md-yellow-300: #fff176;
 --md-yellow-400: #ffee58;
 --md-yellow-500: #ffeb3b;
 --md-yellow-600: #fdd835;
 --md-yellow-700: #fbc02d;
 --md-yellow-800: #f9a825;
 --md-yellow-900: #f57f17;
 --md-yellow-A100: #ffff8d;
 --md-yellow-A200: #ffff00;
 --md-yellow-A400: #ffea00;
 --md-yellow-A700: #ffd600;

 --md-amber-50: #fff8e1;
 --md-amber-100: #ffecb3;
 --md-amber-200: #ffe082;
 --md-amber-300: #ffd54f;
 --md-amber-400: #ffca28;
 --md-amber-500: #ffc107;
 --md-amber-600: #ffb300;
 --md-amber-700: #ffa000;
 --md-amber-800: #ff8f00;
 --md-amber-900: #ff6f00;
 --md-amber-A100: #ffe57f;
 --md-amber-A200: #ffd740;
 --md-amber-A400: #ffc400;
 --md-amber-A700: #ffab00;

 --md-orange-50: #fff3e0;
 --md-orange-100: #ffe0b2;
 --md-orange-200: #ffcc80;
 --md-orange-300: #ffb74d;
 --md-orange-400: #ffa726;
 --md-orange-500: #ff9800;
 --md-orange-600: #fb8c00;
 --md-orange-700: #f57c00;
 --md-orange-800: #ef6c00;
 --md-orange-900: #e65100;
 --md-orange-A100: #ffd180;
 --md-orange-A200: #ffab40;
 --md-orange-A400: #ff9100;
 --md-orange-A700: #ff6d00;

 --md-deep-orange-50: #fbe9e7;
 --md-deep-orange-100: #ffccbc;
 --md-deep-orange-200: #ffab91;
 --md-deep-orange-300: #ff8a65;
 --md-deep-orange-400: #ff7043;
 --md-deep-orange-500: #ff5722;
 --md-deep-orange-600: #f4511e;
 --md-deep-orange-700: #e64a19;
 --md-deep-orange-800: #d84315;
 --md-deep-orange-900: #bf360c;
 --md-deep-orange-A100: #ff9e80;
 --md-deep-orange-A200: #ff6e40;
 --md-deep-orange-A400: #ff3d00;
 --md-deep-orange-A700: #dd2c00;

 --md-brown-50: #efebe9;
 --md-brown-100: #d7ccc8;
 --md-brown-200: #bcaaa4;
 --md-brown-300: #a1887f;
 --md-brown-400: #8d6e63;
 --md-brown-500: #795548;
 --md-brown-600: #6d4c41;
 --md-brown-700: #5d4037;
 --md-brown-800: #4e342e;
 --md-brown-900: #3e2723;

 --md-grey-50: #fafafa;
 --md-grey-100: #f5f5f5;
 --md-grey-200: #eeeeee;
 --md-grey-300: #e0e0e0;
 --md-grey-400: #bdbdbd;
 --md-grey-500: #9e9e9e;
 --md-grey-600: #757575;
 --md-grey-700: #616161;
 --md-grey-800: #424242;
 --md-grey-900: #212121;

 --md-blue-grey-50: #eceff1;
 --md-blue-grey-100: #cfd8dc;
 --md-blue-grey-200: #b0bec5;
 --md-blue-grey-300: #90a4ae;
 --md-blue-grey-400: #78909c;
 --md-blue-grey-500: #607d8b;
 --md-blue-grey-600: #546e7a;
 --md-blue-grey-700: #455a64;
 --md-blue-grey-800: #37474f;
 --md-blue-grey-900: #263238;
}

/\*-----------------------------------------------------------------------------
| Copyright (c) 2017, Jupyter Development Team.
|
| Distributed under the terms of the Modified BSD License.
|----------------------------------------------------------------------------\*/

.jp-Spinner {
 position: absolute;
 display: flex;
 justify-content: center;
 align-items: center;
 z-index: 10;
 left: 0;
 top: 0;
 width: 100%;
 height: 100%;
 background: var(--jp-layout-color0);
 outline: none;
}

.jp-SpinnerContent {
 font-size: 10px;
 margin: 50px auto;
 text-indent: -9999em;
 width: 3em;
 height: 3em;
 border-radius: 50%;
 background: var(--jp-brand-color3);
 background: linear-gradient(
 to right,
 #f37626 10%,
 rgba(255, 255, 255, 0) 42%
 );
 position: relative;
 animation: load3 1s infinite linear, fadeIn 1s;
}

.jp-SpinnerContent:before {
 width: 50%;
 height: 50%;
 background: #f37626;
 border-radius: 100% 0 0 0;
 position: absolute;
 top: 0;
 left: 0;
 content: '';
}

.jp-SpinnerContent:after {
 background: var(--jp-layout-color0);
 width: 75%;
 height: 75%;
 border-radius: 50%;
 content: '';
 margin: auto;
 position: absolute;
 top: 0;
 left: 0;
 bottom: 0;
 right: 0;
}

@keyframes fadeIn {
 0% {
 opacity: 0;
 }
 100% {
 opacity: 1;
 }
}

@keyframes load3 {
 0% {
 transform: rotate(0deg);
 }
 100% {
 transform: rotate(360deg);
 }
}

/\*-----------------------------------------------------------------------------
| Copyright (c) 2014-2017, Jupyter Development Team.
|
| Distributed under the terms of the Modified BSD License.
|----------------------------------------------------------------------------\*/

button.jp-mod-styled {
 font-size: var(--jp-ui-font-size1);
 color: var(--jp-ui-font-color0);
 border: none;
 box-sizing: border-box;
 text-align: center;
 line-height: 32px;
 height: 32px;
 padding: 0px 12px;
 letter-spacing: 0.8px;
 outline: none;
 appearance: none;
 -webkit-appearance: none;
 -moz-appearance: none;
}

input.jp-mod-styled {
 background: var(--jp-input-background);
 height: 28px;
 box-sizing: border-box;
 border: var(--jp-border-width) solid var(--jp-border-color1);
 padding-left: 7px;
 padding-right: 7px;
 font-size: var(--jp-ui-font-size2);
 color: var(--jp-ui-font-color0);
 outline: none;
 appearance: none;
 -webkit-appearance: none;
 -moz-appearance: none;
}

input[type='checkbox'].jp-mod-styled {
 appearance: checkbox;
 -webkit-appearance: checkbox;
 -moz-appearance: checkbox;
 height: auto;
}

input.jp-mod-styled:focus {
 border: var(--jp-border-width) solid var(--md-blue-500);
 box-shadow: inset 0 0 4px var(--md-blue-300);
}

.jp-FileDialog-Checkbox {
 margin-top: 35px;
 display: flex;
 flex-direction: row;
 align-items: end;
 width: 100%;
}

.jp-FileDialog-Checkbox > label {
 flex: 1 1 auto;
}

.jp-select-wrapper {
 display: flex;
 position: relative;
 flex-direction: column;
 padding: 1px;
 background-color: var(--jp-layout-color1);
 height: 28px;
 box-sizing: border-box;
 margin-bottom: 12px;
}

.jp-select-wrapper.jp-mod-focused select.jp-mod-styled {
 border: var(--jp-border-width) solid var(--jp-input-active-border-color);
 box-shadow: var(--jp-input-box-shadow);
 background-color: var(--jp-input-active-background);
}

select.jp-mod-styled:hover {
 background-color: var(--jp-layout-color1);
 cursor: pointer;
 color: var(--jp-ui-font-color0);
 background-color: var(--jp-input-hover-background);
 box-shadow: inset 0 0px 1px rgba(0, 0, 0, 0.5);
}

select.jp-mod-styled {
 flex: 1 1 auto;
 height: 32px;
 width: 100%;
 font-size: var(--jp-ui-font-size2);
 background: var(--jp-input-background);
 color: var(--jp-ui-font-color0);
 padding: 0 25px 0 8px;
 border: var(--jp-border-width) solid var(--jp-input-border-color);
 border-radius: 0px;
 outline: none;
 appearance: none;
 -webkit-appearance: none;
 -moz-appearance: none;
}

/\*-----------------------------------------------------------------------------
| Copyright (c) 2014-2016, Jupyter Development Team.
|
| Distributed under the terms of the Modified BSD License.
|----------------------------------------------------------------------------\*/

:root {
 --jp-private-toolbar-height: calc(
 28px + var(--jp-border-width)
 ); /\* leave 28px for content \*/
}

.jp-Toolbar {
 color: var(--jp-ui-font-color1);
 flex: 0 0 auto;
 display: flex;
 flex-direction: row;
 border-bottom: var(--jp-border-width) solid var(--jp-toolbar-border-color);
 box-shadow: var(--jp-toolbar-box-shadow);
 background: var(--jp-toolbar-background);
 min-height: var(--jp-toolbar-micro-height);
 padding: 2px;
 z-index: 1;
 overflow-x: auto;
}

/\* Toolbar items \*/

.jp-Toolbar > .jp-Toolbar-item.jp-Toolbar-spacer {
 flex-grow: 1;
 flex-shrink: 1;
}

.jp-Toolbar-item.jp-Toolbar-kernelStatus {
 display: inline-block;
 width: 32px;
 background-repeat: no-repeat;
 background-position: center;
 background-size: 16px;
}

.jp-Toolbar > .jp-Toolbar-item {
 flex: 0 0 auto;
 display: flex;
 padding-left: 1px;
 padding-right: 1px;
 font-size: var(--jp-ui-font-size1);
 line-height: var(--jp-private-toolbar-height);
 height: 100%;
}

/\* Toolbar buttons \*/

/\* This is the div we use to wrap the react component into a Widget \*/
div.jp-ToolbarButton {
 color: transparent;
 border: none;
 box-sizing: border-box;
 outline: none;
 appearance: none;
 -webkit-appearance: none;
 -moz-appearance: none;
 padding: 0px;
 margin: 0px;
}

button.jp-ToolbarButtonComponent {
 background: var(--jp-layout-color1);
 border: none;
 box-sizing: border-box;
 outline: none;
 appearance: none;
 -webkit-appearance: none;
 -moz-appearance: none;
 padding: 0px 6px;
 margin: 0px;
 height: 24px;
 border-radius: var(--jp-border-radius);
 display: flex;
 align-items: center;
 text-align: center;
 font-size: 14px;
 min-width: unset;
 min-height: unset;
}

button.jp-ToolbarButtonComponent:disabled {
 opacity: 0.4;
}

button.jp-ToolbarButtonComponent span {
 padding: 0px;
 flex: 0 0 auto;
}

button.jp-ToolbarButtonComponent .jp-ToolbarButtonComponent-label {
 font-size: var(--jp-ui-font-size1);
 line-height: 100%;
 padding-left: 2px;
 color: var(--jp-ui-font-color1);
}

#jp-main-dock-panel[data-mode='single-document']
 .jp-MainAreaWidget
 > .jp-Toolbar.jp-Toolbar-micro {
 padding: 0;
 min-height: 0;
}

#jp-main-dock-panel[data-mode='single-document']
 .jp-MainAreaWidget
 > .jp-Toolbar {
 border: none;
 box-shadow: none;
}

/\*-----------------------------------------------------------------------------
| Copyright (c) 2014-2017, Jupyter Development Team.
|
| Distributed under the terms of the Modified BSD License.
|----------------------------------------------------------------------------\*/

/\*-----------------------------------------------------------------------------
| Copyright (c) Jupyter Development Team.
| Copyright (c) 2014-2017, PhosphorJS Contributors
|
| Distributed under the terms of the BSD 3-Clause License.
|
| The full license is in the file LICENSE, distributed with this software.
|----------------------------------------------------------------------------\*/


/\* <DEPRECATED> \*/ body.p-mod-override-cursor \*, /\* </DEPRECATED> \*/
body.lm-mod-override-cursor \* {
 cursor: inherit !important;
}

/\*-----------------------------------------------------------------------------
| Copyright (c) 2014-2016, Jupyter Development Team.
|
| Distributed under the terms of the Modified BSD License.
|----------------------------------------------------------------------------\*/

.jp-JSONEditor {
 display: flex;
 flex-direction: column;
 width: 100%;
}

.jp-JSONEditor-host {
 flex: 1 1 auto;
 border: var(--jp-border-width) solid var(--jp-input-border-color);
 border-radius: 0px;
 background: var(--jp-layout-color0);
 min-height: 50px;
 padding: 1px;
}

.jp-JSONEditor.jp-mod-error .jp-JSONEditor-host {
 border-color: red;
 outline-color: red;
}

.jp-JSONEditor-header {
 display: flex;
 flex: 1 0 auto;
 padding: 0 0 0 12px;
}

.jp-JSONEditor-header label {
 flex: 0 0 auto;
}

.jp-JSONEditor-commitButton {
 height: 16px;
 width: 16px;
 background-size: 18px;
 background-repeat: no-repeat;
 background-position: center;
}

.jp-JSONEditor-host.jp-mod-focused {
 background-color: var(--jp-input-active-background);
 border: 1px solid var(--jp-input-active-border-color);
 box-shadow: var(--jp-input-box-shadow);
}

.jp-Editor.jp-mod-dropTarget {
 border: var(--jp-border-width) solid var(--jp-input-active-border-color);
 box-shadow: var(--jp-input-box-shadow);
}

/\* BASICS \*/

.CodeMirror {
 /\* Set height, width, borders, and global font properties here \*/
 font-family: monospace;
 height: 300px;
 color: black;
 direction: ltr;
}

/\* PADDING \*/

.CodeMirror-lines {
 padding: 4px 0; /\* Vertical padding around content \*/
}
.CodeMirror pre.CodeMirror-line,
.CodeMirror pre.CodeMirror-line-like {
 padding: 0 4px; /\* Horizontal padding of content \*/
}

.CodeMirror-scrollbar-filler, .CodeMirror-gutter-filler {
 background-color: white; /\* The little square between H and V scrollbars \*/
}

/\* GUTTER \*/

.CodeMirror-gutters {
 border-right: 1px solid #ddd;
 background-color: #f7f7f7;
 white-space: nowrap;
}
.CodeMirror-linenumbers {}
.CodeMirror-linenumber {
 padding: 0 3px 0 5px;
 min-width: 20px;
 text-align: right;
 color: #999;
 white-space: nowrap;
}

.CodeMirror-guttermarker { color: black; }
.CodeMirror-guttermarker-subtle { color: #999; }

/\* CURSOR \*/

.CodeMirror-cursor {
 border-left: 1px solid black;
 border-right: none;
 width: 0;
}
/\* Shown when moving in bi-directional text \*/
.CodeMirror div.CodeMirror-secondarycursor {
 border-left: 1px solid silver;
}
.cm-fat-cursor .CodeMirror-cursor {
 width: auto;
 border: 0 !important;
 background: #7e7;
}
.cm-fat-cursor div.CodeMirror-cursors {
 z-index: 1;
}
.cm-fat-cursor-mark {
 background-color: rgba(20, 255, 20, 0.5);
 -webkit-animation: blink 1.06s steps(1) infinite;
 -moz-animation: blink 1.06s steps(1) infinite;
 animation: blink 1.06s steps(1) infinite;
}
.cm-animate-fat-cursor {
 width: auto;
 border: 0;
 -webkit-animation: blink 1.06s steps(1) infinite;
 -moz-animation: blink 1.06s steps(1) infinite;
 animation: blink 1.06s steps(1) infinite;
 background-color: #7e7;
}
@-moz-keyframes blink {
 0% {}
 50% { background-color: transparent; }
 100% {}
}
@-webkit-keyframes blink {
 0% {}
 50% { background-color: transparent; }
 100% {}
}
@keyframes blink {
 0% {}
 50% { background-color: transparent; }
 100% {}
}

/\* Can style cursor different in overwrite (non-insert) mode \*/
.CodeMirror-overwrite .CodeMirror-cursor {}

.cm-tab { display: inline-block; text-decoration: inherit; }

.CodeMirror-rulers {
 position: absolute;
 left: 0; right: 0; top: -50px; bottom: 0;
 overflow: hidden;
}
.CodeMirror-ruler {
 border-left: 1px solid #ccc;
 top: 0; bottom: 0;
 position: absolute;
}

/\* DEFAULT THEME \*/

.cm-s-default .cm-header {color: blue;}
.cm-s-default .cm-quote {color: #090;}
.cm-negative {color: #d44;}
.cm-positive {color: #292;}
.cm-header, .cm-strong {font-weight: bold;}
.cm-em {font-style: italic;}
.cm-link {text-decoration: underline;}
.cm-strikethrough {text-decoration: line-through;}

.cm-s-default .cm-keyword {color: #708;}
.cm-s-default .cm-atom {color: #219;}
.cm-s-default .cm-number {color: #164;}
.cm-s-default .cm-def {color: #00f;}
.cm-s-default .cm-variable,
.cm-s-default .cm-punctuation,
.cm-s-default .cm-property,
.cm-s-default .cm-operator {}
.cm-s-default .cm-variable-2 {color: #05a;}
.cm-s-default .cm-variable-3, .cm-s-default .cm-type {color: #085;}
.cm-s-default .cm-comment {color: #a50;}
.cm-s-default .cm-string {color: #a11;}
.cm-s-default .cm-string-2 {color: #f50;}
.cm-s-default .cm-meta {color: #555;}
.cm-s-default .cm-qualifier {color: #555;}
.cm-s-default .cm-builtin {color: #30a;}
.cm-s-default .cm-bracket {color: #997;}
.cm-s-default .cm-tag {color: #170;}
.cm-s-default .cm-attribute {color: #00c;}
.cm-s-default .cm-hr {color: #999;}
.cm-s-default .cm-link {color: #00c;}

.cm-s-default .cm-error {color: #f00;}
.cm-invalidchar {color: #f00;}

.CodeMirror-composing { border-bottom: 2px solid; }

/\* Default styles for common addons \*/

div.CodeMirror span.CodeMirror-matchingbracket {color: #0b0;}
div.CodeMirror span.CodeMirror-nonmatchingbracket {color: #a22;}
.CodeMirror-matchingtag { background: rgba(255, 150, 0, .3); }
.CodeMirror-activeline-background {background: #e8f2ff;}

/\* STOP \*/

/\* The rest of this file contains styles related to the mechanics of
 the editor. You probably shouldn't touch them. \*/

.CodeMirror {
 position: relative;
 overflow: hidden;
 background: white;
}

.CodeMirror-scroll {
 overflow: scroll !important; /\* Things will break if this is overridden \*/
 /\* 50px is the magic margin used to hide the element's real scrollbars \*/
 /\* See overflow: hidden in .CodeMirror \*/
 margin-bottom: -50px; margin-right: -50px;
 padding-bottom: 50px;
 height: 100%;
 outline: none; /\* Prevent dragging from highlighting the element \*/
 position: relative;
}
.CodeMirror-sizer {
 position: relative;
 border-right: 50px solid transparent;
}

/\* The fake, visible scrollbars. Used to force redraw during scrolling
 before actual scrolling happens, thus preventing shaking and
 flickering artifacts. \*/
.CodeMirror-vscrollbar, .CodeMirror-hscrollbar, .CodeMirror-scrollbar-filler, .CodeMirror-gutter-filler {
 position: absolute;
 z-index: 6;
 display: none;
 outline: none;
}
.CodeMirror-vscrollbar {
 right: 0; top: 0;
 overflow-x: hidden;
 overflow-y: scroll;
}
.CodeMirror-hscrollbar {
 bottom: 0; left: 0;
 overflow-y: hidden;
 overflow-x: scroll;
}
.CodeMirror-scrollbar-filler {
 right: 0; bottom: 0;
}
.CodeMirror-gutter-filler {
 left: 0; bottom: 0;
}

.CodeMirror-gutters {
 position: absolute; left: 0; top: 0;
 min-height: 100%;
 z-index: 3;
}
.CodeMirror-gutter {
 white-space: normal;
 height: 100%;
 display: inline-block;
 vertical-align: top;
 margin-bottom: -50px;
}
.CodeMirror-gutter-wrapper {
 position: absolute;
 z-index: 4;
 background: none !important;
 border: none !important;
}
.CodeMirror-gutter-background {
 position: absolute;
 top: 0; bottom: 0;
 z-index: 4;
}
.CodeMirror-gutter-elt {
 position: absolute;
 cursor: default;
 z-index: 4;
}
.CodeMirror-gutter-wrapper ::selection { background-color: transparent }
.CodeMirror-gutter-wrapper ::-moz-selection { background-color: transparent }

.CodeMirror-lines {
 cursor: text;
 min-height: 1px; /\* prevents collapsing before first draw \*/
}
.CodeMirror pre.CodeMirror-line,
.CodeMirror pre.CodeMirror-line-like {
 /\* Reset some styles that the rest of the page might have set \*/
 -moz-border-radius: 0; -webkit-border-radius: 0; border-radius: 0;
 border-width: 0;
 background: transparent;
 font-family: inherit;
 font-size: inherit;
 margin: 0;
 white-space: pre;
 word-wrap: normal;
 line-height: inherit;
 color: inherit;
 z-index: 2;
 position: relative;
 overflow: visible;
 -webkit-tap-highlight-color: transparent;
 -webkit-font-variant-ligatures: contextual;
 font-variant-ligatures: contextual;
}
.CodeMirror-wrap pre.CodeMirror-line,
.CodeMirror-wrap pre.CodeMirror-line-like {
 word-wrap: break-word;
 white-space: pre-wrap;
 word-break: normal;
}

.CodeMirror-linebackground {
 position: absolute;
 left: 0; right: 0; top: 0; bottom: 0;
 z-index: 0;
}

.CodeMirror-linewidget {
 position: relative;
 z-index: 2;
 padding: 0.1px; /\* Force widget margins to stay inside of the container \*/
}

.CodeMirror-widget {}

.CodeMirror-rtl pre { direction: rtl; }

.CodeMirror-code {
 outline: none;
}

/\* Force content-box sizing for the elements where we expect it \*/
.CodeMirror-scroll,
.CodeMirror-sizer,
.CodeMirror-gutter,
.CodeMirror-gutters,
.CodeMirror-linenumber {
 -moz-box-sizing: content-box;
 box-sizing: content-box;
}

.CodeMirror-measure {
 position: absolute;
 width: 100%;
 height: 0;
 overflow: hidden;
 visibility: hidden;
}

.CodeMirror-cursor {
 position: absolute;
 pointer-events: none;
}
.CodeMirror-measure pre { position: static; }

div.CodeMirror-cursors {
 visibility: hidden;
 position: relative;
 z-index: 3;
}
div.CodeMirror-dragcursors {
 visibility: visible;
}

.CodeMirror-focused div.CodeMirror-cursors {
 visibility: visible;
}

.CodeMirror-selected { background: #d9d9d9; }
.CodeMirror-focused .CodeMirror-selected { background: #d7d4f0; }
.CodeMirror-crosshair { cursor: crosshair; }
.CodeMirror-line::selection, .CodeMirror-line > span::selection, .CodeMirror-line > span > span::selection { background: #d7d4f0; }
.CodeMirror-line::-moz-selection, .CodeMirror-line > span::-moz-selection, .CodeMirror-line > span > span::-moz-selection { background: #d7d4f0; }

.cm-searching {
 background-color: #ffa;
 background-color: rgba(255, 255, 0, .4);
}

/\* Used to force a border model for a node \*/
.cm-force-border { padding-right: .1px; }

@media print {
 /\* Hide the cursor when printing \*/
 .CodeMirror div.CodeMirror-cursors {
 visibility: hidden;
 }
}

/\* See issue #2901 \*/
.cm-tab-wrap-hack:after { content: ''; }

/\* Help users use markselection to safely style text background \*/
span.CodeMirror-selectedtext { background: none; }

.CodeMirror-dialog {
 position: absolute;
 left: 0; right: 0;
 background: inherit;
 z-index: 15;
 padding: .1em .8em;
 overflow: hidden;
 color: inherit;
}

.CodeMirror-dialog-top {
 border-bottom: 1px solid #eee;
 top: 0;
}

.CodeMirror-dialog-bottom {
 border-top: 1px solid #eee;
 bottom: 0;
}

.CodeMirror-dialog input {
 border: none;
 outline: none;
 background: transparent;
 width: 20em;
 color: inherit;
 font-family: monospace;
}

.CodeMirror-dialog button {
 font-size: 70%;
}

.CodeMirror-foldmarker {
 color: blue;
 text-shadow: #b9f 1px 1px 2px, #b9f -1px -1px 2px, #b9f 1px -1px 2px, #b9f -1px 1px 2px;
 font-family: arial;
 line-height: .3;
 cursor: pointer;
}
.CodeMirror-foldgutter {
 width: .7em;
}
.CodeMirror-foldgutter-open,
.CodeMirror-foldgutter-folded {
 cursor: pointer;
}
.CodeMirror-foldgutter-open:after {
 content: "\25BE";
}
.CodeMirror-foldgutter-folded:after {
 content: "\25B8";
}

/\*-----------------------------------------------------------------------------
| Copyright (c) Jupyter Development Team.
| Distributed under the terms of the Modified BSD License.
|----------------------------------------------------------------------------\*/

.CodeMirror {
 line-height: var(--jp-code-line-height);
 font-size: var(--jp-code-font-size);
 font-family: var(--jp-code-font-family);
 border: 0;
 border-radius: 0;
 height: auto;
 /\* Changed to auto to autogrow \*/
}

.CodeMirror pre {
 padding: 0 var(--jp-code-padding);
}

.jp-CodeMirrorEditor[data-type='inline'] .CodeMirror-dialog {
 background-color: var(--jp-layout-color0);
 color: var(--jp-content-font-color1);
}

/\* This causes https://github.com/jupyter/jupyterlab/issues/522 \*/
/\* May not cause it not because we changed it! \*/
.CodeMirror-lines {
 padding: var(--jp-code-padding) 0;
}

.CodeMirror-linenumber {
 padding: 0 8px;
}

.jp-CodeMirrorEditor {
 cursor: text;
}

.jp-CodeMirrorEditor[data-type='inline'] .CodeMirror-cursor {
 border-left: var(--jp-code-cursor-width0) solid var(--jp-editor-cursor-color);
}

/\* When zoomed out 67% and 33% on a screen of 1440 width x 900 height \*/
@media screen and (min-width: 2138px) and (max-width: 4319px) {
 .jp-CodeMirrorEditor[data-type='inline'] .CodeMirror-cursor {
 border-left: var(--jp-code-cursor-width1) solid
 var(--jp-editor-cursor-color);
 }
}

/\* When zoomed out less than 33% \*/
@media screen and (min-width: 4320px) {
 .jp-CodeMirrorEditor[data-type='inline'] .CodeMirror-cursor {
 border-left: var(--jp-code-cursor-width2) solid
 var(--jp-editor-cursor-color);
 }
}

.CodeMirror.jp-mod-readOnly .CodeMirror-cursor {
 display: none;
}

.CodeMirror-gutters {
 border-right: 1px solid var(--jp-border-color2);
 background-color: var(--jp-layout-color0);
}

.jp-CollaboratorCursor {
 border-left: 5px solid transparent;
 border-right: 5px solid transparent;
 border-top: none;
 border-bottom: 3px solid;
 background-clip: content-box;
 margin-left: -5px;
 margin-right: -5px;
}

.CodeMirror-selectedtext.cm-searching {
 background-color: var(--jp-search-selected-match-background-color) !important;
 color: var(--jp-search-selected-match-color) !important;
}

.cm-searching {
 background-color: var(
 --jp-search-unselected-match-background-color
 ) !important;
 color: var(--jp-search-unselected-match-color) !important;
}

.CodeMirror-focused .CodeMirror-selected {
 background-color: var(--jp-editor-selected-focused-background);
}

.CodeMirror-selected {
 background-color: var(--jp-editor-selected-background);
}

.jp-CollaboratorCursor-hover {
 position: absolute;
 z-index: 1;
 transform: translateX(-50%);
 color: white;
 border-radius: 3px;
 padding-left: 4px;
 padding-right: 4px;
 padding-top: 1px;
 padding-bottom: 1px;
 text-align: center;
 font-size: var(--jp-ui-font-size1);
 white-space: nowrap;
}

.jp-CodeMirror-ruler {
 border-left: 1px dashed var(--jp-border-color2);
}

/\*\*
 \* Here is our jupyter theme for CodeMirror syntax highlighting
 \* This is used in our marked.js syntax highlighting and CodeMirror itself
 \* The string "jupyter" is set in ../codemirror/widget.DEFAULT\_CODEMIRROR\_THEME
 \* This came from the classic notebook, which came form highlight.js/GitHub
 \*/

/\*\*
 \* CodeMirror themes are handling the background/color in this way. This works
 \* fine for CodeMirror editors outside the notebook, but the notebook styles
 \* these things differently.
 \*/
.CodeMirror.cm-s-jupyter {
 background: var(--jp-layout-color0);
 color: var(--jp-content-font-color1);
}

/\* In the notebook, we want this styling to be handled by its container \*/
.jp-CodeConsole .CodeMirror.cm-s-jupyter,
.jp-Notebook .CodeMirror.cm-s-jupyter {
 background: transparent;
}

.cm-s-jupyter .CodeMirror-cursor {
 border-left: var(--jp-code-cursor-width0) solid var(--jp-editor-cursor-color);
}
.cm-s-jupyter span.cm-keyword {
 color: var(--jp-mirror-editor-keyword-color);
 font-weight: bold;
}
.cm-s-jupyter span.cm-atom {
 color: var(--jp-mirror-editor-atom-color);
}
.cm-s-jupyter span.cm-number {
 color: var(--jp-mirror-editor-number-color);
}
.cm-s-jupyter span.cm-def {
 color: var(--jp-mirror-editor-def-color);
}
.cm-s-jupyter span.cm-variable {
 color: var(--jp-mirror-editor-variable-color);
}
.cm-s-jupyter span.cm-variable-2 {
 color: var(--jp-mirror-editor-variable-2-color);
}
.cm-s-jupyter span.cm-variable-3 {
 color: var(--jp-mirror-editor-variable-3-color);
}
.cm-s-jupyter span.cm-punctuation {
 color: var(--jp-mirror-editor-punctuation-color);
}
.cm-s-jupyter span.cm-property {
 color: var(--jp-mirror-editor-property-color);
}
.cm-s-jupyter span.cm-operator {
 color: var(--jp-mirror-editor-operator-color);
 font-weight: bold;
}
.cm-s-jupyter span.cm-comment {
 color: var(--jp-mirror-editor-comment-color);
 font-style: italic;
}
.cm-s-jupyter span.cm-string {
 color: var(--jp-mirror-editor-string-color);
}
.cm-s-jupyter span.cm-string-2 {
 color: var(--jp-mirror-editor-string-2-color);
}
.cm-s-jupyter span.cm-meta {
 color: var(--jp-mirror-editor-meta-color);
}
.cm-s-jupyter span.cm-qualifier {
 color: var(--jp-mirror-editor-qualifier-color);
}
.cm-s-jupyter span.cm-builtin {
 color: var(--jp-mirror-editor-builtin-color);
}
.cm-s-jupyter span.cm-bracket {
 color: var(--jp-mirror-editor-bracket-color);
}
.cm-s-jupyter span.cm-tag {
 color: var(--jp-mirror-editor-tag-color);
}
.cm-s-jupyter span.cm-attribute {
 color: var(--jp-mirror-editor-attribute-color);
}
.cm-s-jupyter span.cm-header {
 color: var(--jp-mirror-editor-header-color);
}
.cm-s-jupyter span.cm-quote {
 color: var(--jp-mirror-editor-quote-color);
}
.cm-s-jupyter span.cm-link {
 color: var(--jp-mirror-editor-link-color);
}
.cm-s-jupyter span.cm-error {
 color: var(--jp-mirror-editor-error-color);
}
.cm-s-jupyter span.cm-hr {
 color: #999;
}

.cm-s-jupyter span.cm-tab {
 background: url(data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAADAAAAAMCAYAAAAkuj5RAAAAAXNSR0IArs4c6QAAAGFJREFUSMft1LsRQFAQheHPowAKoACx3IgEKtaEHujDjORSgWTH/ZOdnZOcM/sgk/kFFWY0qV8foQwS4MKBCS3qR6ixBJvElOobYAtivseIE120FaowJPN75GMu8j/LfMwNjh4HUpwg4LUAAAAASUVORK5CYII=);
 background-position: right;
 background-repeat: no-repeat;
}

.cm-s-jupyter .CodeMirror-activeline-background,
.cm-s-jupyter .CodeMirror-gutter {
 background-color: var(--jp-layout-color2);
}

/\* Styles for shared cursors (remote cursor locations and selected ranges) \*/
.jp-CodeMirrorEditor .remote-caret {
 position: relative;
 border-left: 2px solid black;
 margin-left: -1px;
 margin-right: -1px;
 box-sizing: border-box;
}

.jp-CodeMirrorEditor .remote-caret > div {
 white-space: nowrap;
 position: absolute;
 top: -1.15em;
 padding-bottom: 0.05em;
 left: -2px;
 font-size: 0.95em;
 background-color: rgb(250, 129, 0);
 font-family: var(--jp-ui-font-family);
 font-weight: bold;
 line-height: normal;
 user-select: none;
 color: white;
 padding-left: 2px;
 padding-right: 2px;
 z-index: 3;
 transition: opacity 0.3s ease-in-out;
}

.jp-CodeMirrorEditor .remote-caret.hide-name > div {
 transition-delay: 0.7s;
 opacity: 0;
}

.jp-CodeMirrorEditor .remote-caret:hover > div {
 opacity: 1;
 transition-delay: 0s;
}

/\*-----------------------------------------------------------------------------
| Copyright (c) Jupyter Development Team.
| Distributed under the terms of the Modified BSD License.
|----------------------------------------------------------------------------\*/

/\*-----------------------------------------------------------------------------
| RenderedText
|----------------------------------------------------------------------------\*/

:root {
 /\* This is the padding value to fill the gaps between lines containing spans with background color. \*/
 --jp-private-code-span-padding: calc(
 (var(--jp-code-line-height) - 1) \* var(--jp-code-font-size) / 2
 );
}

.jp-RenderedText {
 text-align: left;
 padding-left: var(--jp-code-padding);
 line-height: var(--jp-code-line-height);
 font-family: var(--jp-code-font-family);
}

.jp-RenderedText pre,
.jp-RenderedJavaScript pre,
.jp-RenderedHTMLCommon pre {
 color: var(--jp-content-font-color1);
 font-size: var(--jp-code-font-size);
 border: none;
 margin: 0px;
 padding: 0px;
}

.jp-RenderedText pre a:link {
 text-decoration: none;
 color: var(--jp-content-link-color);
}
.jp-RenderedText pre a:hover {
 text-decoration: underline;
 color: var(--jp-content-link-color);
}
.jp-RenderedText pre a:visited {
 text-decoration: none;
 color: var(--jp-content-link-color);
}

/\* console foregrounds and backgrounds \*/
.jp-RenderedText pre .ansi-black-fg {
 color: #3e424d;
}
.jp-RenderedText pre .ansi-red-fg {
 color: #e75c58;
}
.jp-RenderedText pre .ansi-green-fg {
 color: #00a250;
}
.jp-RenderedText pre .ansi-yellow-fg {
 color: #ddb62b;
}
.jp-RenderedText pre .ansi-blue-fg {
 color: #208ffb;
}
.jp-RenderedText pre .ansi-magenta-fg {
 color: #d160c4;
}
.jp-RenderedText pre .ansi-cyan-fg {
 color: #60c6c8;
}
.jp-RenderedText pre .ansi-white-fg {
 color: #c5c1b4;
}

.jp-RenderedText pre .ansi-black-bg {
 background-color: #3e424d;
 padding: var(--jp-private-code-span-padding) 0;
}
.jp-RenderedText pre .ansi-red-bg {
 background-color: #e75c58;
 padding: var(--jp-private-code-span-padding) 0;
}
.jp-RenderedText pre .ansi-green-bg {
 background-color: #00a250;
 padding: var(--jp-private-code-span-padding) 0;
}
.jp-RenderedText pre .ansi-yellow-bg {
 background-color: #ddb62b;
 padding: var(--jp-private-code-span-padding) 0;
}
.jp-RenderedText pre .ansi-blue-bg {
 background-color: #208ffb;
 padding: var(--jp-private-code-span-padding) 0;
}
.jp-RenderedText pre .ansi-magenta-bg {
 background-color: #d160c4;
 padding: var(--jp-private-code-span-padding) 0;
}
.jp-RenderedText pre .ansi-cyan-bg {
 background-color: #60c6c8;
 padding: var(--jp-private-code-span-padding) 0;
}
.jp-RenderedText pre .ansi-white-bg {
 background-color: #c5c1b4;
 padding: var(--jp-private-code-span-padding) 0;
}

.jp-RenderedText pre .ansi-black-intense-fg {
 color: #282c36;
}
.jp-RenderedText pre .ansi-red-intense-fg {
 color: #b22b31;
}
.jp-RenderedText pre .ansi-green-intense-fg {
 color: #007427;
}
.jp-RenderedText pre .ansi-yellow-intense-fg {
 color: #b27d12;
}
.jp-RenderedText pre .ansi-blue-intense-fg {
 color: #0065ca;
}
.jp-RenderedText pre .ansi-magenta-intense-fg {
 color: #a03196;
}
.jp-RenderedText pre .ansi-cyan-intense-fg {
 color: #258f8f;
}
.jp-RenderedText pre .ansi-white-intense-fg {
 color: #a1a6b2;
}

.jp-RenderedText pre .ansi-black-intense-bg {
 background-color: #282c36;
 padding: var(--jp-private-code-span-padding) 0;
}
.jp-RenderedText pre .ansi-red-intense-bg {
 background-color: #b22b31;
 padding: var(--jp-private-code-span-padding) 0;
}
.jp-RenderedText pre .ansi-green-intense-bg {
 background-color: #007427;
 padding: var(--jp-private-code-span-padding) 0;
}
.jp-RenderedText pre .ansi-yellow-intense-bg {
 background-color: #b27d12;
 padding: var(--jp-private-code-span-padding) 0;
}
.jp-RenderedText pre .ansi-blue-intense-bg {
 background-color: #0065ca;
 padding: var(--jp-private-code-span-padding) 0;
}
.jp-RenderedText pre .ansi-magenta-intense-bg {
 background-color: #a03196;
 padding: var(--jp-private-code-span-padding) 0;
}
.jp-RenderedText pre .ansi-cyan-intense-bg {
 background-color: #258f8f;
 padding: var(--jp-private-code-span-padding) 0;
}
.jp-RenderedText pre .ansi-white-intense-bg {
 background-color: #a1a6b2;
 padding: var(--jp-private-code-span-padding) 0;
}

.jp-RenderedText pre .ansi-default-inverse-fg {
 color: var(--jp-ui-inverse-font-color0);
}
.jp-RenderedText pre .ansi-default-inverse-bg {
 background-color: var(--jp-inverse-layout-color0);
 padding: var(--jp-private-code-span-padding) 0;
}

.jp-RenderedText pre .ansi-bold {
 font-weight: bold;
}
.jp-RenderedText pre .ansi-underline {
 text-decoration: underline;
}

.jp-RenderedText[data-mime-type='application/vnd.jupyter.stderr'] {
 background: var(--jp-rendermime-error-background);
 padding-top: var(--jp-code-padding);
}

/\*-----------------------------------------------------------------------------
| RenderedLatex
|----------------------------------------------------------------------------\*/

.jp-RenderedLatex {
 color: var(--jp-content-font-color1);
 font-size: var(--jp-content-font-size1);
 line-height: var(--jp-content-line-height);
}

/\* Left-justify outputs.\*/
.jp-OutputArea-output.jp-RenderedLatex {
 padding: var(--jp-code-padding);
 text-align: left;
}

/\*-----------------------------------------------------------------------------
| RenderedHTML
|----------------------------------------------------------------------------\*/

.jp-RenderedHTMLCommon {
 color: var(--jp-content-font-color1);
 font-family: var(--jp-content-font-family);
 font-size: var(--jp-content-font-size1);
 line-height: var(--jp-content-line-height);
 /\* Give a bit more R padding on Markdown text to keep line lengths reasonable \*/
 padding-right: 20px;
}

.jp-RenderedHTMLCommon em {
 font-style: italic;
}

.jp-RenderedHTMLCommon strong {
 font-weight: bold;
}

.jp-RenderedHTMLCommon u {
 text-decoration: underline;
}

.jp-RenderedHTMLCommon a:link {
 text-decoration: none;
 color: var(--jp-content-link-color);
}

.jp-RenderedHTMLCommon a:hover {
 text-decoration: underline;
 color: var(--jp-content-link-color);
}

.jp-RenderedHTMLCommon a:visited {
 text-decoration: none;
 color: var(--jp-content-link-color);
}

/\* Headings \*/

.jp-RenderedHTMLCommon h1,
.jp-RenderedHTMLCommon h2,
.jp-RenderedHTMLCommon h3,
.jp-RenderedHTMLCommon h4,
.jp-RenderedHTMLCommon h5,
.jp-RenderedHTMLCommon h6 {
 line-height: var(--jp-content-heading-line-height);
 font-weight: var(--jp-content-heading-font-weight);
 font-style: normal;
 margin: var(--jp-content-heading-margin-top) 0
 var(--jp-content-heading-margin-bottom) 0;
}

.jp-RenderedHTMLCommon h1:first-child,
.jp-RenderedHTMLCommon h2:first-child,
.jp-RenderedHTMLCommon h3:first-child,
.jp-RenderedHTMLCommon h4:first-child,
.jp-RenderedHTMLCommon h5:first-child,
.jp-RenderedHTMLCommon h6:first-child {
 margin-top: calc(0.5 \* var(--jp-content-heading-margin-top));
}

.jp-RenderedHTMLCommon h1:last-child,
.jp-RenderedHTMLCommon h2:last-child,
.jp-RenderedHTMLCommon h3:last-child,
.jp-RenderedHTMLCommon h4:last-child,
.jp-RenderedHTMLCommon h5:last-child,
.jp-RenderedHTMLCommon h6:last-child {
 margin-bottom: calc(0.5 \* var(--jp-content-heading-margin-bottom));
}

.jp-RenderedHTMLCommon h1 {
 font-size: var(--jp-content-font-size5);
}

.jp-RenderedHTMLCommon h2 {
 font-size: var(--jp-content-font-size4);
}

.jp-RenderedHTMLCommon h3 {
 font-size: var(--jp-content-font-size3);
}

.jp-RenderedHTMLCommon h4 {
 font-size: var(--jp-content-font-size2);
}

.jp-RenderedHTMLCommon h5 {
 font-size: var(--jp-content-font-size1);
}

.jp-RenderedHTMLCommon h6 {
 font-size: var(--jp-content-font-size0);
}

/\* Lists \*/

.jp-RenderedHTMLCommon ul:not(.list-inline),
.jp-RenderedHTMLCommon ol:not(.list-inline) {
 padding-left: 2em;
}

.jp-RenderedHTMLCommon ul {
 list-style: disc;
}

.jp-RenderedHTMLCommon ul ul {
 list-style: square;
}

.jp-RenderedHTMLCommon ul ul ul {
 list-style: circle;
}

.jp-RenderedHTMLCommon ol {
 list-style: decimal;
}

.jp-RenderedHTMLCommon ol ol {
 list-style: upper-alpha;
}

.jp-RenderedHTMLCommon ol ol ol {
 list-style: lower-alpha;
}

.jp-RenderedHTMLCommon ol ol ol ol {
 list-style: lower-roman;
}

.jp-RenderedHTMLCommon ol ol ol ol ol {
 list-style: decimal;
}

.jp-RenderedHTMLCommon ol,
.jp-RenderedHTMLCommon ul {
 margin-bottom: 1em;
}

.jp-RenderedHTMLCommon ul ul,
.jp-RenderedHTMLCommon ul ol,
.jp-RenderedHTMLCommon ol ul,
.jp-RenderedHTMLCommon ol ol {
 margin-bottom: 0em;
}

.jp-RenderedHTMLCommon hr {
 color: var(--jp-border-color2);
 background-color: var(--jp-border-color1);
 margin-top: 1em;
 margin-bottom: 1em;
}

.jp-RenderedHTMLCommon > pre {
 margin: 1.5em 2em;
}

.jp-RenderedHTMLCommon pre,
.jp-RenderedHTMLCommon code {
 border: 0;
 background-color: var(--jp-layout-color0);
 color: var(--jp-content-font-color1);
 font-family: var(--jp-code-font-family);
 font-size: inherit;
 line-height: var(--jp-code-line-height);
 padding: 0;
 white-space: pre-wrap;
}

.jp-RenderedHTMLCommon :not(pre) > code {
 background-color: var(--jp-layout-color2);
 padding: 1px 5px;
}

/\* Tables \*/

.jp-RenderedHTMLCommon table {
 border-collapse: collapse;
 border-spacing: 0;
 border: none;
 color: var(--jp-ui-font-color1);
 font-size: 12px;
 table-layout: fixed;
 margin-left: auto;
 margin-right: auto;
}

.jp-RenderedHTMLCommon thead {
 border-bottom: var(--jp-border-width) solid var(--jp-border-color1);
 vertical-align: bottom;
}

.jp-RenderedHTMLCommon td,
.jp-RenderedHTMLCommon th,
.jp-RenderedHTMLCommon tr {
 vertical-align: middle;
 padding: 0.5em 0.5em;
 line-height: normal;
 white-space: normal;
 max-width: none;
 border: none;
}

.jp-RenderedMarkdown.jp-RenderedHTMLCommon td,
.jp-RenderedMarkdown.jp-RenderedHTMLCommon th {
 max-width: none;
}

:not(.jp-RenderedMarkdown).jp-RenderedHTMLCommon td,
:not(.jp-RenderedMarkdown).jp-RenderedHTMLCommon th,
:not(.jp-RenderedMarkdown).jp-RenderedHTMLCommon tr {
 text-align: right;
}

.jp-RenderedHTMLCommon th {
 font-weight: bold;
}

.jp-RenderedHTMLCommon tbody tr:nth-child(odd) {
 background: var(--jp-layout-color0);
}

.jp-RenderedHTMLCommon tbody tr:nth-child(even) {
 background: var(--jp-rendermime-table-row-background);
}

.jp-RenderedHTMLCommon tbody tr:hover {
 background: var(--jp-rendermime-table-row-hover-background);
}

.jp-RenderedHTMLCommon table {
 margin-bottom: 1em;
}

.jp-RenderedHTMLCommon p {
 text-align: left;
 margin: 0px;
}

.jp-RenderedHTMLCommon p {
 margin-bottom: 1em;
}

.jp-RenderedHTMLCommon img {
 -moz-force-broken-image-icon: 1;
}

/\* Restrict to direct children as other images could be nested in other content. \*/
.jp-RenderedHTMLCommon > img {
 display: block;
 margin-left: 0;
 margin-right: 0;
 margin-bottom: 1em;
}

/\* Change color behind transparent images if they need it... \*/
[data-jp-theme-light='false'] .jp-RenderedImage img.jp-needs-light-background {
 background-color: var(--jp-inverse-layout-color1);
}
[data-jp-theme-light='true'] .jp-RenderedImage img.jp-needs-dark-background {
 background-color: var(--jp-inverse-layout-color1);
}
/\* ...or leave it untouched if they don't \*/
[data-jp-theme-light='false'] .jp-RenderedImage img.jp-needs-dark-background {
}
[data-jp-theme-light='true'] .jp-RenderedImage img.jp-needs-light-background {
}

.jp-RenderedHTMLCommon img,
.jp-RenderedImage img,
.jp-RenderedHTMLCommon svg,
.jp-RenderedSVG svg {
 max-width: 100%;
 height: auto;
}

.jp-RenderedHTMLCommon img.jp-mod-unconfined,
.jp-RenderedImage img.jp-mod-unconfined,
.jp-RenderedHTMLCommon svg.jp-mod-unconfined,
.jp-RenderedSVG svg.jp-mod-unconfined {
 max-width: none;
}

.jp-RenderedHTMLCommon .alert {
 padding: var(--jp-notebook-padding);
 border: var(--jp-border-width) solid transparent;
 border-radius: var(--jp-border-radius);
 margin-bottom: 1em;
}

.jp-RenderedHTMLCommon .alert-info {
 color: var(--jp-info-color0);
 background-color: var(--jp-info-color3);
 border-color: var(--jp-info-color2);
}
.jp-RenderedHTMLCommon .alert-info hr {
 border-color: var(--jp-info-color3);
}
.jp-RenderedHTMLCommon .alert-info > p:last-child,
.jp-RenderedHTMLCommon .alert-info > ul:last-child {
 margin-bottom: 0;
}

.jp-RenderedHTMLCommon .alert-warning {
 color: var(--jp-warn-color0);
 background-color: var(--jp-warn-color3);
 border-color: var(--jp-warn-color2);
}
.jp-RenderedHTMLCommon .alert-warning hr {
 border-color: var(--jp-warn-color3);
}
.jp-RenderedHTMLCommon .alert-warning > p:last-child,
.jp-RenderedHTMLCommon .alert-warning > ul:last-child {
 margin-bottom: 0;
}

.jp-RenderedHTMLCommon .alert-success {
 color: var(--jp-success-color0);
 background-color: var(--jp-success-color3);
 border-color: var(--jp-success-color2);
}
.jp-RenderedHTMLCommon .alert-success hr {
 border-color: var(--jp-success-color3);
}
.jp-RenderedHTMLCommon .alert-success > p:last-child,
.jp-RenderedHTMLCommon .alert-success > ul:last-child {
 margin-bottom: 0;
}

.jp-RenderedHTMLCommon .alert-danger {
 color: var(--jp-error-color0);
 background-color: var(--jp-error-color3);
 border-color: var(--jp-error-color2);
}
.jp-RenderedHTMLCommon .alert-danger hr {
 border-color: var(--jp-error-color3);
}
.jp-RenderedHTMLCommon .alert-danger > p:last-child,
.jp-RenderedHTMLCommon .alert-danger > ul:last-child {
 margin-bottom: 0;
}

.jp-RenderedHTMLCommon blockquote {
 margin: 1em 2em;
 padding: 0 1em;
 border-left: 5px solid var(--jp-border-color2);
}

a.jp-InternalAnchorLink {
 visibility: hidden;
 margin-left: 8px;
 color: var(--md-blue-800);
}

h1:hover .jp-InternalAnchorLink,
h2:hover .jp-InternalAnchorLink,
h3:hover .jp-InternalAnchorLink,
h4:hover .jp-InternalAnchorLink,
h5:hover .jp-InternalAnchorLink,
h6:hover .jp-InternalAnchorLink {
 visibility: visible;
}

.jp-RenderedHTMLCommon kbd {
 background-color: var(--jp-rendermime-table-row-background);
 border: 1px solid var(--jp-border-color0);
 border-bottom-color: var(--jp-border-color2);
 border-radius: 3px;
 box-shadow: inset 0 -1px 0 rgba(0, 0, 0, 0.25);
 display: inline-block;
 font-size: 0.8em;
 line-height: 1em;
 padding: 0.2em 0.5em;
}

/\* Most direct children of .jp-RenderedHTMLCommon have a margin-bottom of 1.0.
 \* At the bottom of cells this is a bit too much as there is also spacing
 \* between cells. Going all the way to 0 gets too tight between markdown and
 \* code cells.
 \*/
.jp-RenderedHTMLCommon > \*:last-child {
 margin-bottom: 0.5em;
}

/\*-----------------------------------------------------------------------------
| Copyright (c) Jupyter Development Team.
| Distributed under the terms of the Modified BSD License.
|----------------------------------------------------------------------------\*/

.jp-MimeDocument {
 outline: none;
}

/\*-----------------------------------------------------------------------------
| Copyright (c) Jupyter Development Team.
| Distributed under the terms of the Modified BSD License.
|----------------------------------------------------------------------------\*/

/\*-----------------------------------------------------------------------------
| Variables
|----------------------------------------------------------------------------\*/

:root {
 --jp-private-filebrowser-button-height: 28px;
 --jp-private-filebrowser-button-width: 48px;
}

/\*-----------------------------------------------------------------------------
| Copyright (c) Jupyter Development Team.
| Distributed under the terms of the Modified BSD License.
|----------------------------------------------------------------------------\*/

.jp-FileBrowser {
 display: flex;
 flex-direction: column;
 color: var(--jp-ui-font-color1);
 background: var(--jp-layout-color1);
 /\* This is needed so that all font sizing of children done in ems is
 \* relative to this base size \*/
 font-size: var(--jp-ui-font-size1);
}

.jp-FileBrowser-toolbar.jp-Toolbar {
 border-bottom: none;
 height: auto;
 margin: var(--jp-toolbar-header-margin);
 box-shadow: none;
}

.jp-BreadCrumbs {
 flex: 0 0 auto;
 margin: 8px 12px 8px 12px;
}

.jp-BreadCrumbs-item {
 margin: 0px 2px;
 padding: 0px 2px;
 border-radius: var(--jp-border-radius);
 cursor: pointer;
}

.jp-BreadCrumbs-item:hover {
 background-color: var(--jp-layout-color2);
}

.jp-BreadCrumbs-item:first-child {
 margin-left: 0px;
}

.jp-BreadCrumbs-item.jp-mod-dropTarget {
 background-color: var(--jp-brand-color2);
 opacity: 0.7;
}

/\*-----------------------------------------------------------------------------
| Buttons
|----------------------------------------------------------------------------\*/

.jp-FileBrowser-toolbar.jp-Toolbar {
 padding: 0px;
 margin: 8px 12px 0px 12px;
}

.jp-FileBrowser-toolbar.jp-Toolbar {
 justify-content: flex-start;
}

.jp-FileBrowser-toolbar.jp-Toolbar .jp-Toolbar-item {
 flex: 0 0 auto;
 padding-left: 0px;
 padding-right: 2px;
}

.jp-FileBrowser-toolbar.jp-Toolbar .jp-ToolbarButtonComponent {
 width: 40px;
}

.jp-FileBrowser-toolbar.jp-Toolbar
 .jp-Toolbar-item:first-child
 .jp-ToolbarButtonComponent {
 width: 72px;
 background: var(--jp-brand-color1);
}

.jp-FileBrowser-toolbar.jp-Toolbar
 .jp-Toolbar-item:first-child
 .jp-ToolbarButtonComponent:focus-visible {
 background-color: var(--jp-brand-color0);
}

.jp-FileBrowser-toolbar.jp-Toolbar
 .jp-Toolbar-item:first-child
 .jp-ToolbarButtonComponent
 .jp-icon3 {
 fill: white;
}

/\*-----------------------------------------------------------------------------
| Other styles
|----------------------------------------------------------------------------\*/

.jp-FileDialog.jp-mod-conflict input {
 color: var(--jp-error-color1);
}

.jp-FileDialog .jp-new-name-title {
 margin-top: 12px;
}

.jp-LastModified-hidden {
 display: none;
}

.jp-FileBrowser-filterBox {
 padding: 0px;
 flex: 0 0 auto;
 margin: 8px 12px 0px 12px;
}

/\*-----------------------------------------------------------------------------
| DirListing
|----------------------------------------------------------------------------\*/

.jp-DirListing {
 flex: 1 1 auto;
 display: flex;
 flex-direction: column;
 outline: 0;
}

.jp-DirListing:focus-visible {
 border: 1px solid var(--jp-brand-color1);
}

.jp-DirListing-header {
 flex: 0 0 auto;
 display: flex;
 flex-direction: row;
 overflow: hidden;
 border-top: var(--jp-border-width) solid var(--jp-border-color2);
 border-bottom: var(--jp-border-width) solid var(--jp-border-color1);
 box-shadow: var(--jp-toolbar-box-shadow);
 z-index: 2;
}

.jp-DirListing-headerItem {
 padding: 4px 12px 2px 12px;
 font-weight: 500;
}

.jp-DirListing-headerItem:hover {
 background: var(--jp-layout-color2);
}

.jp-DirListing-headerItem.jp-id-name {
 flex: 1 0 84px;
}

.jp-DirListing-headerItem.jp-id-modified {
 flex: 0 0 112px;
 border-left: var(--jp-border-width) solid var(--jp-border-color2);
 text-align: right;
}

.jp-id-narrow {
 display: none;
 flex: 0 0 5px;
 padding: 4px 4px;
 border-left: var(--jp-border-width) solid var(--jp-border-color2);
 text-align: right;
 color: var(--jp-border-color2);
}

.jp-DirListing-narrow .jp-id-narrow {
 display: block;
}

.jp-DirListing-narrow .jp-id-modified,
.jp-DirListing-narrow .jp-DirListing-itemModified {
 display: none;
}

.jp-DirListing-headerItem.jp-mod-selected {
 font-weight: 600;
}

/\* increase specificity to override bundled default \*/
.jp-DirListing-content {
 flex: 1 1 auto;
 margin: 0;
 padding: 0;
 list-style-type: none;
 overflow: auto;
 background-color: var(--jp-layout-color1);
}

.jp-DirListing-content mark {
 color: var(--jp-ui-font-color0);
 background-color: transparent;
 font-weight: bold;
}

.jp-DirListing-content .jp-DirListing-item.jp-mod-selected mark {
 color: var(--jp-ui-inverse-font-color0);
}

/\* Style the directory listing content when a user drops a file to upload \*/
.jp-DirListing.jp-mod-native-drop .jp-DirListing-content {
 outline: 5px dashed rgba(128, 128, 128, 0.5);
 outline-offset: -10px;
 cursor: copy;
}

.jp-DirListing-item {
 display: flex;
 flex-direction: row;
 padding: 4px 12px;
 -webkit-user-select: none;
 -moz-user-select: none;
 -ms-user-select: none;
 user-select: none;
}

.jp-DirListing-item[data-is-dot] {
 opacity: 75%;
}

.jp-DirListing-item.jp-mod-selected {
 color: var(--jp-ui-inverse-font-color1);
 background: var(--jp-brand-color1);
}

.jp-DirListing-item.jp-mod-dropTarget {
 background: var(--jp-brand-color3);
}

.jp-DirListing-item:hover:not(.jp-mod-selected) {
 background: var(--jp-layout-color2);
}

.jp-DirListing-itemIcon {
 flex: 0 0 20px;
 margin-right: 4px;
}

.jp-DirListing-itemText {
 flex: 1 0 64px;
 white-space: nowrap;
 overflow: hidden;
 text-overflow: ellipsis;
 user-select: none;
}

.jp-DirListing-itemModified {
 flex: 0 0 125px;
 text-align: right;
}

.jp-DirListing-editor {
 flex: 1 0 64px;
 outline: none;
 border: none;
}

.jp-DirListing-item.jp-mod-running .jp-DirListing-itemIcon:before {
 color: var(--jp-success-color1);
 content: '\25CF';
 font-size: 8px;
 position: absolute;
 left: -8px;
}

.jp-DirListing-item.jp-mod-running.jp-mod-selected
 .jp-DirListing-itemIcon:before {
 color: var(--jp-ui-inverse-font-color1);
}

.jp-DirListing-item.lm-mod-drag-image,
.jp-DirListing-item.jp-mod-selected.lm-mod-drag-image {
 font-size: var(--jp-ui-font-size1);
 padding-left: 4px;
 margin-left: 4px;
 width: 160px;
 background-color: var(--jp-ui-inverse-font-color2);
 box-shadow: var(--jp-elevation-z2);
 border-radius: 0px;
 color: var(--jp-ui-font-color1);
 transform: translateX(-40%) translateY(-58%);
}

.jp-DirListing-deadSpace {
 flex: 1 1 auto;
 margin: 0;
 padding: 0;
 list-style-type: none;
 overflow: auto;
 background-color: var(--jp-layout-color1);
}

.jp-Document {
 min-width: 120px;
 min-height: 120px;
 outline: none;
}

/\*-----------------------------------------------------------------------------
| Copyright (c) Jupyter Development Team.
| Distributed under the terms of the Modified BSD License.
|----------------------------------------------------------------------------\*/

/\*-----------------------------------------------------------------------------
| Private CSS variables
|----------------------------------------------------------------------------\*/

:root {
}

/\*-----------------------------------------------------------------------------
| Main OutputArea
| OutputArea has a list of Outputs
|----------------------------------------------------------------------------\*/

.jp-OutputArea {
 overflow-y: auto;
}

.jp-OutputArea-child {
 display: flex;
 flex-direction: row;
}

body[data-format='mobile'] .jp-OutputArea-child {
 flex-direction: column;
}

.jp-OutputPrompt {
 flex: 0 0 var(--jp-cell-prompt-width);
 color: var(--jp-cell-outprompt-font-color);
 font-family: var(--jp-cell-prompt-font-family);
 padding: var(--jp-code-padding);
 letter-spacing: var(--jp-cell-prompt-letter-spacing);
 line-height: var(--jp-code-line-height);
 font-size: var(--jp-code-font-size);
 border: var(--jp-border-width) solid transparent;
 opacity: var(--jp-cell-prompt-opacity);
 /\* Right align prompt text, don't wrap to handle large prompt numbers \*/
 text-align: right;
 white-space: nowrap;
 overflow: hidden;
 text-overflow: ellipsis;
 /\* Disable text selection \*/
 -webkit-user-select: none;
 -moz-user-select: none;
 -ms-user-select: none;
 user-select: none;
}

body[data-format='mobile'] .jp-OutputPrompt {
 flex: 0 0 auto;
 text-align: left;
}

.jp-OutputArea-output {
 height: auto;
 overflow: auto;
 user-select: text;
 -moz-user-select: text;
 -webkit-user-select: text;
 -ms-user-select: text;
}

.jp-OutputArea-child .jp-OutputArea-output {
 flex-grow: 1;
 flex-shrink: 1;
}

body[data-format='mobile'] .jp-OutputArea-child .jp-OutputArea-output {
 margin-left: var(--jp-notebook-padding);
}

/\*\*
 \* Isolated output.
 \*/
.jp-OutputArea-output.jp-mod-isolated {
 width: 100%;
 display: block;
}

/\*
When drag events occur, `p-mod-override-cursor` is added to the body.
Because iframes steal all cursor events, the following two rules are necessary
to suppress pointer events while resize drags are occurring. There may be a
better solution to this problem.
\*/
body.lm-mod-override-cursor .jp-OutputArea-output.jp-mod-isolated {
 position: relative;
}

body.lm-mod-override-cursor .jp-OutputArea-output.jp-mod-isolated:before {
 content: '';
 position: absolute;
 top: 0;
 left: 0;
 right: 0;
 bottom: 0;
 background: transparent;
}

/\* pre \*/

.jp-OutputArea-output pre {
 border: none;
 margin: 0px;
 padding: 0px;
 overflow-x: auto;
 overflow-y: auto;
 word-break: break-all;
 word-wrap: break-word;
 white-space: pre-wrap;
}

/\* tables \*/

.jp-OutputArea-output.jp-RenderedHTMLCommon table {
 margin-left: 0;
 margin-right: 0;
}

/\* description lists \*/

.jp-OutputArea-output dl,
.jp-OutputArea-output dt,
.jp-OutputArea-output dd {
 display: block;
}

.jp-OutputArea-output dl {
 width: 100%;
 overflow: hidden;
 padding: 0;
 margin: 0;
}

.jp-OutputArea-output dt {
 font-weight: bold;
 float: left;
 width: 20%;
 padding: 0;
 margin: 0;
}

.jp-OutputArea-output dd {
 float: left;
 width: 80%;
 padding: 0;
 margin: 0;
}

/\* Hide the gutter in case of
 \* - nested output areas (e.g. in the case of output widgets)
 \* - mirrored output areas
 \*/
.jp-OutputArea .jp-OutputArea .jp-OutputArea-prompt {
 display: none;
}

/\*-----------------------------------------------------------------------------
| executeResult is added to any Output-result for the display of the object
| returned by a cell
|----------------------------------------------------------------------------\*/

.jp-OutputArea-output.jp-OutputArea-executeResult {
 margin-left: 0px;
 flex: 1 1 auto;
}

/\* Text output with the Out[] prompt needs a top padding to match the
 \* alignment of the Out[] prompt itself.
 \*/
.jp-OutputArea-executeResult .jp-RenderedText.jp-OutputArea-output {
 padding-top: var(--jp-code-padding);
 border-top: var(--jp-border-width) solid transparent;
}

/\*-----------------------------------------------------------------------------
| The Stdin output
|----------------------------------------------------------------------------\*/

.jp-OutputArea-stdin {
 line-height: var(--jp-code-line-height);
 padding-top: var(--jp-code-padding);
 display: flex;
}

.jp-Stdin-prompt {
 color: var(--jp-content-font-color0);
 padding-right: var(--jp-code-padding);
 vertical-align: baseline;
 flex: 0 0 auto;
}

.jp-Stdin-input {
 font-family: var(--jp-code-font-family);
 font-size: inherit;
 color: inherit;
 background-color: inherit;
 width: 42%;
 min-width: 200px;
 /\* make sure input baseline aligns with prompt \*/
 vertical-align: baseline;
 /\* padding + margin = 0.5em between prompt and cursor \*/
 padding: 0em 0.25em;
 margin: 0em 0.25em;
 flex: 0 0 70%;
}

.jp-Stdin-input:focus {
 box-shadow: none;
}

/\*-----------------------------------------------------------------------------
| Output Area View
|----------------------------------------------------------------------------\*/

.jp-LinkedOutputView .jp-OutputArea {
 height: 100%;
 display: block;
}

.jp-LinkedOutputView .jp-OutputArea-output:only-child {
 height: 100%;
}

/\*-----------------------------------------------------------------------------
| Copyright (c) Jupyter Development Team.
| Distributed under the terms of the Modified BSD License.
|----------------------------------------------------------------------------\*/

.jp-Collapser {
 flex: 0 0 var(--jp-cell-collapser-width);
 padding: 0px;
 margin: 0px;
 border: none;
 outline: none;
 background: transparent;
 border-radius: var(--jp-border-radius);
 opacity: 1;
}

.jp-Collapser-child {
 display: block;
 width: 100%;
 box-sizing: border-box;
 /\* height: 100% doesn't work because the height of its parent is computed from content \*/
 position: absolute;
 top: 0px;
 bottom: 0px;
}

/\*-----------------------------------------------------------------------------
| Copyright (c) Jupyter Development Team.
| Distributed under the terms of the Modified BSD License.
|----------------------------------------------------------------------------\*/

/\*-----------------------------------------------------------------------------
| Header/Footer
|----------------------------------------------------------------------------\*/

/\* Hidden by zero height by default \*/
.jp-CellHeader,
.jp-CellFooter {
 height: 0px;
 width: 100%;
 padding: 0px;
 margin: 0px;
 border: none;
 outline: none;
 background: transparent;
}

/\*-----------------------------------------------------------------------------
| Copyright (c) Jupyter Development Team.
| Distributed under the terms of the Modified BSD License.
|----------------------------------------------------------------------------\*/

/\*-----------------------------------------------------------------------------
| Input
|----------------------------------------------------------------------------\*/

/\* All input areas \*/
.jp-InputArea {
 display: flex;
 flex-direction: row;
 overflow: hidden;
}

body[data-format='mobile'] .jp-InputArea {
 flex-direction: column;
}

.jp-InputArea-editor {
 flex: 1 1 auto;
 overflow: hidden;
}

.jp-InputArea-editor {
 /\* This is the non-active, default styling \*/
 border: var(--jp-border-width) solid var(--jp-cell-editor-border-color);
 border-radius: 0px;
 background: var(--jp-cell-editor-background);
}

body[data-format='mobile'] .jp-InputArea-editor {
 margin-left: var(--jp-notebook-padding);
}

.jp-InputPrompt {
 flex: 0 0 var(--jp-cell-prompt-width);
 color: var(--jp-cell-inprompt-font-color);
 font-family: var(--jp-cell-prompt-font-family);
 padding: var(--jp-code-padding);
 letter-spacing: var(--jp-cell-prompt-letter-spacing);
 opacity: var(--jp-cell-prompt-opacity);
 line-height: var(--jp-code-line-height);
 font-size: var(--jp-code-font-size);
 border: var(--jp-border-width) solid transparent;
 opacity: var(--jp-cell-prompt-opacity);
 /\* Right align prompt text, don't wrap to handle large prompt numbers \*/
 text-align: right;
 white-space: nowrap;
 overflow: hidden;
 text-overflow: ellipsis;
 /\* Disable text selection \*/
 -webkit-user-select: none;
 -moz-user-select: none;
 -ms-user-select: none;
 user-select: none;
}

body[data-format='mobile'] .jp-InputPrompt {
 flex: 0 0 auto;
 text-align: left;
}

/\*-----------------------------------------------------------------------------
| Copyright (c) Jupyter Development Team.
| Distributed under the terms of the Modified BSD License.
|----------------------------------------------------------------------------\*/

/\*-----------------------------------------------------------------------------
| Placeholder
|----------------------------------------------------------------------------\*/

.jp-Placeholder {
 display: flex;
 flex-direction: row;
 flex: 1 1 auto;
}

.jp-Placeholder-prompt {
 box-sizing: border-box;
}

.jp-Placeholder-content {
 flex: 1 1 auto;
 border: none;
 background: transparent;
 height: 20px;
 box-sizing: border-box;
}

.jp-Placeholder-content .jp-MoreHorizIcon {
 width: 32px;
 height: 16px;
 border: 1px solid transparent;
 border-radius: var(--jp-border-radius);
}

.jp-Placeholder-content .jp-MoreHorizIcon:hover {
 border: 1px solid var(--jp-border-color1);
 box-shadow: 0px 0px 2px 0px rgba(0, 0, 0, 0.25);
 background-color: var(--jp-layout-color0);
}

/\*-----------------------------------------------------------------------------
| Copyright (c) Jupyter Development Team.
| Distributed under the terms of the Modified BSD License.
|----------------------------------------------------------------------------\*/

/\*-----------------------------------------------------------------------------
| Private CSS variables
|----------------------------------------------------------------------------\*/

:root {
 --jp-private-cell-scrolling-output-offset: 5px;
}

/\*-----------------------------------------------------------------------------
| Cell
|----------------------------------------------------------------------------\*/

.jp-Cell {
 padding: var(--jp-cell-padding);
 margin: 0px;
 border: none;
 outline: none;
 background: transparent;
}

/\*-----------------------------------------------------------------------------
| Common input/output
|----------------------------------------------------------------------------\*/

.jp-Cell-inputWrapper,
.jp-Cell-outputWrapper {
 display: flex;
 flex-direction: row;
 padding: 0px;
 margin: 0px;
 /\* Added to reveal the box-shadow on the input and output collapsers. \*/
 overflow: visible;
}

/\* Only input/output areas inside cells \*/
.jp-Cell-inputArea,
.jp-Cell-outputArea {
 flex: 1 1 auto;
}

/\*-----------------------------------------------------------------------------
| Collapser
|----------------------------------------------------------------------------\*/

/\* Make the output collapser disappear when there is not output, but do so
 \* in a manner that leaves it in the layout and preserves its width.
 \*/
.jp-Cell.jp-mod-noOutputs .jp-Cell-outputCollapser {
 border: none !important;
 background: transparent !important;
}

.jp-Cell:not(.jp-mod-noOutputs) .jp-Cell-outputCollapser {
 min-height: var(--jp-cell-collapser-min-height);
}

/\*-----------------------------------------------------------------------------
| Output
|----------------------------------------------------------------------------\*/

/\* Put a space between input and output when there IS output \*/
.jp-Cell:not(.jp-mod-noOutputs) .jp-Cell-outputWrapper {
 margin-top: 5px;
}

.jp-CodeCell.jp-mod-outputsScrolled .jp-Cell-outputArea {
 overflow-y: auto;
 max-height: 200px;
 box-shadow: inset 0 0 6px 2px rgba(0, 0, 0, 0.3);
 margin-left: var(--jp-private-cell-scrolling-output-offset);
}

.jp-CodeCell.jp-mod-outputsScrolled .jp-OutputArea-prompt {
 flex: 0 0
 calc(
 var(--jp-cell-prompt-width) -
 var(--jp-private-cell-scrolling-output-offset)
 );
}

/\*-----------------------------------------------------------------------------
| CodeCell
|----------------------------------------------------------------------------\*/

/\*-----------------------------------------------------------------------------
| MarkdownCell
|----------------------------------------------------------------------------\*/

.jp-MarkdownOutput {
 flex: 1 1 auto;
 margin-top: 0;
 margin-bottom: 0;
 padding-left: var(--jp-code-padding);
}

.jp-MarkdownOutput.jp-RenderedHTMLCommon {
 overflow: auto;
}

.jp-showHiddenCellsButton {
 margin-left: calc(var(--jp-cell-prompt-width) + 2 \* var(--jp-code-padding));
 margin-top: var(--jp-code-padding);
 border: 1px solid var(--jp-border-color2);
 background-color: var(--jp-border-color3) !important;
 color: var(--jp-content-font-color0) !important;
}

.jp-showHiddenCellsButton:hover {
 background-color: var(--jp-border-color2) !important;
}

.jp-collapseHeadingButton {
 display: none;
}

.jp-MarkdownCell:hover .jp-collapseHeadingButton {
 display: flex;
 min-height: var(--jp-cell-collapser-min-height);
 position: absolute;
 right: 0;
 top: 0;
 bottom: 0;
}

/\*-----------------------------------------------------------------------------
| Copyright (c) Jupyter Development Team.
| Distributed under the terms of the Modified BSD License.
|----------------------------------------------------------------------------\*/

/\*-----------------------------------------------------------------------------
| Copyright (c) Jupyter Development Team.
| Distributed under the terms of the Modified BSD License.
|----------------------------------------------------------------------------\*/

/\*-----------------------------------------------------------------------------
| Variables
|----------------------------------------------------------------------------\*/

/\*-----------------------------------------------------------------------------

/\*-----------------------------------------------------------------------------
| Styles
|----------------------------------------------------------------------------\*/

.jp-NotebookPanel-toolbar {
 padding: 2px;
}

.jp-Toolbar-item.jp-Notebook-toolbarCellType .jp-select-wrapper.jp-mod-focused {
 border: none;
 box-shadow: none;
}

.jp-Notebook-toolbarCellTypeDropdown select {
 height: 24px;
 font-size: var(--jp-ui-font-size1);
 line-height: 14px;
 border-radius: 0;
 display: block;
}

.jp-Notebook-toolbarCellTypeDropdown span {
 top: 5px !important;
}

/\*-----------------------------------------------------------------------------
| Copyright (c) Jupyter Development Team.
| Distributed under the terms of the Modified BSD License.
|----------------------------------------------------------------------------\*/

/\*-----------------------------------------------------------------------------
| Private CSS variables
|----------------------------------------------------------------------------\*/

:root {
 --jp-private-notebook-dragImage-width: 304px;
 --jp-private-notebook-dragImage-height: 36px;
 --jp-private-notebook-selected-color: var(--md-blue-400);
 --jp-private-notebook-active-color: var(--md-green-400);
}

/\*-----------------------------------------------------------------------------
| Imports
|----------------------------------------------------------------------------\*/

/\*-----------------------------------------------------------------------------
| Notebook
|----------------------------------------------------------------------------\*/

.jp-NotebookPanel {
 display: block;
 height: 100%;
}

.jp-NotebookPanel.jp-Document {
 min-width: 240px;
 min-height: 120px;
}

.jp-Notebook {
 padding: var(--jp-notebook-padding);
 outline: none;
 overflow: auto;
 background: var(--jp-layout-color0);
}

.jp-Notebook.jp-mod-scrollPastEnd::after {
 display: block;
 content: '';
 min-height: var(--jp-notebook-scroll-padding);
}

.jp-MainAreaWidget-ContainStrict .jp-Notebook \* {
 contain: strict;
}

.jp-Notebook-render \* {
 contain: none !important;
}

.jp-Notebook .jp-Cell {
 overflow: visible;
}

.jp-Notebook .jp-Cell .jp-InputPrompt {
 cursor: move;
 float: left;
}

/\*-----------------------------------------------------------------------------
| Notebook state related styling
|
| The notebook and cells each have states, here are the possibilities:
|
| - Notebook
| - Command
| - Edit
| - Cell
| - None
| - Active (only one can be active)
| - Selected (the cells actions are applied to)
| - Multiselected (when multiple selected, the cursor)
| - No outputs
|----------------------------------------------------------------------------\*/

/\* Command or edit modes \*/

.jp-Notebook .jp-Cell:not(.jp-mod-active) .jp-InputPrompt {
 opacity: var(--jp-cell-prompt-not-active-opacity);
 color: var(--jp-cell-prompt-not-active-font-color);
}

.jp-Notebook .jp-Cell:not(.jp-mod-active) .jp-OutputPrompt {
 opacity: var(--jp-cell-prompt-not-active-opacity);
 color: var(--jp-cell-prompt-not-active-font-color);
}

/\* cell is active \*/
.jp-Notebook .jp-Cell.jp-mod-active .jp-Collapser {
 background: var(--jp-brand-color1);
}

/\* cell is dirty \*/
.jp-Notebook .jp-Cell.jp-mod-dirty .jp-InputPrompt {
 color: var(--jp-warn-color1);
}
.jp-Notebook .jp-Cell.jp-mod-dirty .jp-InputPrompt:before {
 color: var(--jp-warn-color1);
 content: '•';
}

.jp-Notebook .jp-Cell.jp-mod-active.jp-mod-dirty .jp-Collapser {
 background: var(--jp-warn-color1);
}

/\* collapser is hovered \*/
.jp-Notebook .jp-Cell .jp-Collapser:hover {
 box-shadow: var(--jp-elevation-z2);
 background: var(--jp-brand-color1);
 opacity: var(--jp-cell-collapser-not-active-hover-opacity);
}

/\* cell is active and collapser is hovered \*/
.jp-Notebook .jp-Cell.jp-mod-active .jp-Collapser:hover {
 background: var(--jp-brand-color0);
 opacity: 1;
}

/\* Command mode \*/

.jp-Notebook.jp-mod-commandMode .jp-Cell.jp-mod-selected {
 background: var(--jp-notebook-multiselected-color);
}

.jp-Notebook.jp-mod-commandMode
 .jp-Cell.jp-mod-active.jp-mod-selected:not(.jp-mod-multiSelected) {
 background: transparent;
}

/\* Edit mode \*/

.jp-Notebook.jp-mod-editMode .jp-Cell.jp-mod-active .jp-InputArea-editor {
 border: var(--jp-border-width) solid var(--jp-cell-editor-active-border-color);
 box-shadow: var(--jp-input-box-shadow);
 background-color: var(--jp-cell-editor-active-background);
}

/\*-----------------------------------------------------------------------------
| Notebook drag and drop
|----------------------------------------------------------------------------\*/

.jp-Notebook-cell.jp-mod-dropSource {
 opacity: 0.5;
}

.jp-Notebook-cell.jp-mod-dropTarget,
.jp-Notebook.jp-mod-commandMode
 .jp-Notebook-cell.jp-mod-active.jp-mod-selected.jp-mod-dropTarget {
 border-top-color: var(--jp-private-notebook-selected-color);
 border-top-style: solid;
 border-top-width: 2px;
}

.jp-dragImage {
 display: block;
 flex-direction: row;
 width: var(--jp-private-notebook-dragImage-width);
 height: var(--jp-private-notebook-dragImage-height);
 border: var(--jp-border-width) solid var(--jp-cell-editor-border-color);
 background: var(--jp-cell-editor-background);
 overflow: visible;
}

.jp-dragImage-singlePrompt {
 box-shadow: 2px 2px 4px 0px rgba(0, 0, 0, 0.12);
}

.jp-dragImage .jp-dragImage-content {
 flex: 1 1 auto;
 z-index: 2;
 font-size: var(--jp-code-font-size);
 font-family: var(--jp-code-font-family);
 line-height: var(--jp-code-line-height);
 padding: var(--jp-code-padding);
 border: var(--jp-border-width) solid var(--jp-cell-editor-border-color);
 background: var(--jp-cell-editor-background-color);
 color: var(--jp-content-font-color3);
 text-align: left;
 margin: 4px 4px 4px 0px;
}

.jp-dragImage .jp-dragImage-prompt {
 flex: 0 0 auto;
 min-width: 36px;
 color: var(--jp-cell-inprompt-font-color);
 padding: var(--jp-code-padding);
 padding-left: 12px;
 font-family: var(--jp-cell-prompt-font-family);
 letter-spacing: var(--jp-cell-prompt-letter-spacing);
 line-height: 1.9;
 font-size: var(--jp-code-font-size);
 border: var(--jp-border-width) solid transparent;
}

.jp-dragImage-multipleBack {
 z-index: -1;
 position: absolute;
 height: 32px;
 width: 300px;
 top: 8px;
 left: 8px;
 background: var(--jp-layout-color2);
 border: var(--jp-border-width) solid var(--jp-input-border-color);
 box-shadow: 2px 2px 4px 0px rgba(0, 0, 0, 0.12);
}

/\*-----------------------------------------------------------------------------
| Cell toolbar
|----------------------------------------------------------------------------\*/

.jp-NotebookTools {
 display: block;
 min-width: var(--jp-sidebar-min-width);
 color: var(--jp-ui-font-color1);
 background: var(--jp-layout-color1);
 /\* This is needed so that all font sizing of children done in ems is
 \* relative to this base size \*/
 font-size: var(--jp-ui-font-size1);
 overflow: auto;
}

.jp-NotebookTools-tool {
 padding: 0px 12px 0 12px;
}

.jp-ActiveCellTool {
 padding: 12px;
 background-color: var(--jp-layout-color1);
 border-top: none !important;
}

.jp-ActiveCellTool .jp-InputArea-prompt {
 flex: 0 0 auto;
 padding-left: 0px;
}

.jp-ActiveCellTool .jp-InputArea-editor {
 flex: 1 1 auto;
 background: var(--jp-cell-editor-background);
 border-color: var(--jp-cell-editor-border-color);
}

.jp-ActiveCellTool .jp-InputArea-editor .CodeMirror {
 background: transparent;
}

.jp-MetadataEditorTool {
 flex-direction: column;
 padding: 12px 0px 12px 0px;
}

.jp-RankedPanel > :not(:first-child) {
 margin-top: 12px;
}

.jp-KeySelector select.jp-mod-styled {
 font-size: var(--jp-ui-font-size1);
 color: var(--jp-ui-font-color0);
 border: var(--jp-border-width) solid var(--jp-border-color1);
}

.jp-KeySelector label,
.jp-MetadataEditorTool label {
 line-height: 1.4;
}

.jp-NotebookTools .jp-select-wrapper {
 margin-top: 4px;
 margin-bottom: 0px;
}

.jp-NotebookTools .jp-Collapse {
 margin-top: 16px;
}

/\*-----------------------------------------------------------------------------
| Presentation Mode (.jp-mod-presentationMode)
|----------------------------------------------------------------------------\*/

.jp-mod-presentationMode .jp-Notebook {
 --jp-content-font-size1: var(--jp-content-presentation-font-size1);
 --jp-code-font-size: var(--jp-code-presentation-font-size);
}

.jp-mod-presentationMode .jp-Notebook .jp-Cell .jp-InputPrompt,
.jp-mod-presentationMode .jp-Notebook .jp-Cell .jp-OutputPrompt {
 flex: 0 0 110px;
}

/\*-----------------------------------------------------------------------------
| Placeholder
|----------------------------------------------------------------------------\*/

.jp-Cell-Placeholder {
 padding-left: 55px;
}

.jp-Cell-Placeholder-wrapper {
 background: #fff;
 border: 1px solid;
 border-color: #e5e6e9 #dfe0e4 #d0d1d5;
 border-radius: 4px;
 -webkit-border-radius: 4px;
 margin: 10px 15px;
}

.jp-Cell-Placeholder-wrapper-inner {
 padding: 15px;
 position: relative;
}

.jp-Cell-Placeholder-wrapper-body {
 background-repeat: repeat;
 background-size: 50% auto;
}

.jp-Cell-Placeholder-wrapper-body div {
 background: #f6f7f8;
 background-image: -webkit-linear-gradient(
 left,
 #f6f7f8 0%,
 #edeef1 20%,
 #f6f7f8 40%,
 #f6f7f8 100%
 );
 background-repeat: no-repeat;
 background-size: 800px 104px;
 height: 104px;
 position: relative;
}

.jp-Cell-Placeholder-wrapper-body div {
 position: absolute;
 right: 15px;
 left: 15px;
 top: 15px;
}

div.jp-Cell-Placeholder-h1 {
 top: 20px;
 height: 20px;
 left: 15px;
 width: 150px;
}

div.jp-Cell-Placeholder-h2 {
 left: 15px;
 top: 50px;
 height: 10px;
 width: 100px;
}

div.jp-Cell-Placeholder-content-1,
div.jp-Cell-Placeholder-content-2,
div.jp-Cell-Placeholder-content-3 {
 left: 15px;
 right: 15px;
 height: 10px;
}

div.jp-Cell-Placeholder-content-1 {
 top: 100px;
}

div.jp-Cell-Placeholder-content-2 {
 top: 120px;
}

div.jp-Cell-Placeholder-content-3 {
 top: 140px;
}



/\*-----------------------------------------------------------------------------
| Copyright (c) Jupyter Development Team.
| Distributed under the terms of the Modified BSD License.
|----------------------------------------------------------------------------\*/

/\*
The following CSS variables define the main, public API for styling JupyterLab.
These variables should be used by all plugins wherever possible. In other
words, plugins should not define custom colors, sizes, etc unless absolutely
necessary. This enables users to change the visual theme of JupyterLab
by changing these variables.

Many variables appear in an ordered sequence (0,1,2,3). These sequences
are designed to work well together, so for example, `--jp-border-color1` should
be used with `--jp-layout-color1`. The numbers have the following meanings:

\* 0: super-primary, reserved for special emphasis
\* 1: primary, most important under normal situations
\* 2: secondary, next most important under normal situations
\* 3: tertiary, next most important under normal situations

Throughout JupyterLab, we are mostly following principles from Google's
Material Design when selecting colors. We are not, however, following
all of MD as it is not optimized for dense, information rich UIs.
\*/

:root {
 /\* Elevation
 \*
 \* We style box-shadows using Material Design's idea of elevation. These particular numbers are taken from here:
 \*
 \* https://github.com/material-components/material-components-web
 \* https://material-components-web.appspot.com/elevation.html
 \*/

 --jp-shadow-base-lightness: 0;
 --jp-shadow-umbra-color: rgba(
 var(--jp-shadow-base-lightness),
 var(--jp-shadow-base-lightness),
 var(--jp-shadow-base-lightness),
 0.2
 );
 --jp-shadow-penumbra-color: rgba(
 var(--jp-shadow-base-lightness),
 var(--jp-shadow-base-lightness),
 var(--jp-shadow-base-lightness),
 0.14
 );
 --jp-shadow-ambient-color: rgba(
 var(--jp-shadow-base-lightness),
 var(--jp-shadow-base-lightness),
 var(--jp-shadow-base-lightness),
 0.12
 );
 --jp-elevation-z0: none;
 --jp-elevation-z1: 0px 2px 1px -1px var(--jp-shadow-umbra-color),
 0px 1px 1px 0px var(--jp-shadow-penumbra-color),
 0px 1px 3px 0px var(--jp-shadow-ambient-color);
 --jp-elevation-z2: 0px 3px 1px -2px var(--jp-shadow-umbra-color),
 0px 2px 2px 0px var(--jp-shadow-penumbra-color),
 0px 1px 5px 0px var(--jp-shadow-ambient-color);
 --jp-elevation-z4: 0px 2px 4px -1px var(--jp-shadow-umbra-color),
 0px 4px 5px 0px var(--jp-shadow-penumbra-color),
 0px 1px 10px 0px var(--jp-shadow-ambient-color);
 --jp-elevation-z6: 0px 3px 5px -1px var(--jp-shadow-umbra-color),
 0px 6px 10px 0px var(--jp-shadow-penumbra-color),
 0px 1px 18px 0px var(--jp-shadow-ambient-color);
 --jp-elevation-z8: 0px 5px 5px -3px var(--jp-shadow-umbra-color),
 0px 8px 10px 1px var(--jp-shadow-penumbra-color),
 0px 3px 14px 2px var(--jp-shadow-ambient-color);
 --jp-elevation-z12: 0px 7px 8px -4px var(--jp-shadow-umbra-color),
 0px 12px 17px 2px var(--jp-shadow-penumbra-color),
 0px 5px 22px 4px var(--jp-shadow-ambient-color);
 --jp-elevation-z16: 0px 8px 10px -5px var(--jp-shadow-umbra-color),
 0px 16px 24px 2px var(--jp-shadow-penumbra-color),
 0px 6px 30px 5px var(--jp-shadow-ambient-color);
 --jp-elevation-z20: 0px 10px 13px -6px var(--jp-shadow-umbra-color),
 0px 20px 31px 3px var(--jp-shadow-penumbra-color),
 0px 8px 38px 7px var(--jp-shadow-ambient-color);
 --jp-elevation-z24: 0px 11px 15px -7px var(--jp-shadow-umbra-color),
 0px 24px 38px 3px var(--jp-shadow-penumbra-color),
 0px 9px 46px 8px var(--jp-shadow-ambient-color);

 /\* Borders
 \*
 \* The following variables, specify the visual styling of borders in JupyterLab.
 \*/

 --jp-border-width: 1px;
 --jp-border-color0: var(--md-grey-400);
 --jp-border-color1: var(--md-grey-400);
 --jp-border-color2: var(--md-grey-300);
 --jp-border-color3: var(--md-grey-200);
 --jp-border-radius: 2px;

 /\* UI Fonts
 \*
 \* The UI font CSS variables are used for the typography all of the JupyterLab
 \* user interface elements that are not directly user generated content.
 \*
 \* The font sizing here is done assuming that the body font size of --jp-ui-font-size1
 \* is applied to a parent element. When children elements, such as headings, are sized
 \* in em all things will be computed relative to that body size.
 \*/

 --jp-ui-font-scale-factor: 1.2;
 --jp-ui-font-size0: 0.83333em;
 --jp-ui-font-size1: 13px; /\* Base font size \*/
 --jp-ui-font-size2: 1.2em;
 --jp-ui-font-size3: 1.44em;

 --jp-ui-font-family: -apple-system, BlinkMacSystemFont, 'Segoe UI', Helvetica,
 Arial, sans-serif, 'Apple Color Emoji', 'Segoe UI Emoji', 'Segoe UI Symbol';

 /\*
 \* Use these font colors against the corresponding main layout colors.
 \* In a light theme, these go from dark to light.
 \*/

 /\* Defaults use Material Design specification \*/
 --jp-ui-font-color0: rgba(0, 0, 0, 1);
 --jp-ui-font-color1: rgba(0, 0, 0, 0.87);
 --jp-ui-font-color2: rgba(0, 0, 0, 0.54);
 --jp-ui-font-color3: rgba(0, 0, 0, 0.38);

 /\*
 \* Use these against the brand/accent/warn/error colors.
 \* These will typically go from light to darker, in both a dark and light theme.
 \*/

 --jp-ui-inverse-font-color0: rgba(255, 255, 255, 1);
 --jp-ui-inverse-font-color1: rgba(255, 255, 255, 1);
 --jp-ui-inverse-font-color2: rgba(255, 255, 255, 0.7);
 --jp-ui-inverse-font-color3: rgba(255, 255, 255, 0.5);

 /\* Content Fonts
 \*
 \* Content font variables are used for typography of user generated content.
 \*
 \* The font sizing here is done assuming that the body font size of --jp-content-font-size1
 \* is applied to a parent element. When children elements, such as headings, are sized
 \* in em all things will be computed relative to that body size.
 \*/

 --jp-content-line-height: 1.6;
 --jp-content-font-scale-factor: 1.2;
 --jp-content-font-size0: 0.83333em;
 --jp-content-font-size1: 14px; /\* Base font size \*/
 --jp-content-font-size2: 1.2em;
 --jp-content-font-size3: 1.44em;
 --jp-content-font-size4: 1.728em;
 --jp-content-font-size5: 2.0736em;

 /\* This gives a magnification of about 125% in presentation mode over normal. \*/
 --jp-content-presentation-font-size1: 17px;

 --jp-content-heading-line-height: 1;
 --jp-content-heading-margin-top: 1.2em;
 --jp-content-heading-margin-bottom: 0.8em;
 --jp-content-heading-font-weight: 500;

 /\* Defaults use Material Design specification \*/
 --jp-content-font-color0: rgba(0, 0, 0, 1);
 --jp-content-font-color1: rgba(0, 0, 0, 0.87);
 --jp-content-font-color2: rgba(0, 0, 0, 0.54);
 --jp-content-font-color3: rgba(0, 0, 0, 0.38);

 --jp-content-link-color: var(--md-blue-700);

 --jp-content-font-family: -apple-system, BlinkMacSystemFont, 'Segoe UI',
 Helvetica, Arial, sans-serif, 'Apple Color Emoji', 'Segoe UI Emoji',
 'Segoe UI Symbol';

 /\*
 \* Code Fonts
 \*
 \* Code font variables are used for typography of code and other monospaces content.
 \*/

 --jp-code-font-size: 13px;
 --jp-code-line-height: 1.3077; /\* 17px for 13px base \*/
 --jp-code-padding: 5px; /\* 5px for 13px base, codemirror highlighting needs integer px value \*/
 --jp-code-font-family-default: Menlo, Consolas, 'DejaVu Sans Mono', monospace;
 --jp-code-font-family: var(--jp-code-font-family-default);

 /\* This gives a magnification of about 125% in presentation mode over normal. \*/
 --jp-code-presentation-font-size: 16px;

 /\* may need to tweak cursor width if you change font size \*/
 --jp-code-cursor-width0: 1.4px;
 --jp-code-cursor-width1: 2px;
 --jp-code-cursor-width2: 4px;

 /\* Layout
 \*
 \* The following are the main layout colors use in JupyterLab. In a light
 \* theme these would go from light to dark.
 \*/

 --jp-layout-color0: white;
 --jp-layout-color1: white;
 --jp-layout-color2: var(--md-grey-200);
 --jp-layout-color3: var(--md-grey-400);
 --jp-layout-color4: var(--md-grey-600);

 /\* Inverse Layout
 \*
 \* The following are the inverse layout colors use in JupyterLab. In a light
 \* theme these would go from dark to light.
 \*/

 --jp-inverse-layout-color0: #111111;
 --jp-inverse-layout-color1: var(--md-grey-900);
 --jp-inverse-layout-color2: var(--md-grey-800);
 --jp-inverse-layout-color3: var(--md-grey-700);
 --jp-inverse-layout-color4: var(--md-grey-600);

 /\* Brand/accent \*/

 --jp-brand-color0: var(--md-blue-900);
 --jp-brand-color1: var(--md-blue-700);
 --jp-brand-color2: var(--md-blue-300);
 --jp-brand-color3: var(--md-blue-100);
 --jp-brand-color4: var(--md-blue-50);

 --jp-accent-color0: var(--md-green-900);
 --jp-accent-color1: var(--md-green-700);
 --jp-accent-color2: var(--md-green-300);
 --jp-accent-color3: var(--md-green-100);

 /\* State colors (warn, error, success, info) \*/

 --jp-warn-color0: var(--md-orange-900);
 --jp-warn-color1: var(--md-orange-700);
 --jp-warn-color2: var(--md-orange-300);
 --jp-warn-color3: var(--md-orange-100);

 --jp-error-color0: var(--md-red-900);
 --jp-error-color1: var(--md-red-700);
 --jp-error-color2: var(--md-red-300);
 --jp-error-color3: var(--md-red-100);

 --jp-success-color0: var(--md-green-900);
 --jp-success-color1: var(--md-green-700);
 --jp-success-color2: var(--md-green-300);
 --jp-success-color3: var(--md-green-100);

 --jp-info-color0: var(--md-cyan-900);
 --jp-info-color1: var(--md-cyan-700);
 --jp-info-color2: var(--md-cyan-300);
 --jp-info-color3: var(--md-cyan-100);

 /\* Cell specific styles \*/

 --jp-cell-padding: 5px;

 --jp-cell-collapser-width: 8px;
 --jp-cell-collapser-min-height: 20px;
 --jp-cell-collapser-not-active-hover-opacity: 0.6;

 --jp-cell-editor-background: var(--md-grey-100);
 --jp-cell-editor-border-color: var(--md-grey-300);
 --jp-cell-editor-box-shadow: inset 0 0 2px var(--md-blue-300);
 --jp-cell-editor-active-background: var(--jp-layout-color0);
 --jp-cell-editor-active-border-color: var(--jp-brand-color1);

 --jp-cell-prompt-width: 64px;
 --jp-cell-prompt-font-family: var(--jp-code-font-family-default);
 --jp-cell-prompt-letter-spacing: 0px;
 --jp-cell-prompt-opacity: 1;
 --jp-cell-prompt-not-active-opacity: 0.5;
 --jp-cell-prompt-not-active-font-color: var(--md-grey-700);
 /\* A custom blend of MD grey and blue 600
 \* See https://meyerweb.com/eric/tools/color-blend/#546E7A:1E88E5:5:hex \*/
 --jp-cell-inprompt-font-color: #307fc1;
 /\* A custom blend of MD grey and orange 600
 \* https://meyerweb.com/eric/tools/color-blend/#546E7A:F4511E:5:hex \*/
 --jp-cell-outprompt-font-color: #bf5b3d;

 /\* Notebook specific styles \*/

 --jp-notebook-padding: 10px;
 --jp-notebook-select-background: var(--jp-layout-color1);
 --jp-notebook-multiselected-color: var(--md-blue-50);

 /\* The scroll padding is calculated to fill enough space at the bottom of the
 notebook to show one single-line cell (with appropriate padding) at the top
 when the notebook is scrolled all the way to the bottom. We also subtract one
 pixel so that no scrollbar appears if we have just one single-line cell in the
 notebook. This padding is to enable a 'scroll past end' feature in a notebook.
 \*/
 --jp-notebook-scroll-padding: calc(
 100% - var(--jp-code-font-size) \* var(--jp-code-line-height) -
 var(--jp-code-padding) - var(--jp-cell-padding) - 1px
 );

 /\* Rendermime styles \*/

 --jp-rendermime-error-background: #fdd;
 --jp-rendermime-table-row-background: var(--md-grey-100);
 --jp-rendermime-table-row-hover-background: var(--md-light-blue-50);

 /\* Dialog specific styles \*/

 --jp-dialog-background: rgba(0, 0, 0, 0.25);

 /\* Console specific styles \*/

 --jp-console-padding: 10px;

 /\* Toolbar specific styles \*/

 --jp-toolbar-border-color: var(--jp-border-color1);
 --jp-toolbar-micro-height: 8px;
 --jp-toolbar-background: var(--jp-layout-color1);
 --jp-toolbar-box-shadow: 0px 0px 2px 0px rgba(0, 0, 0, 0.24);
 --jp-toolbar-header-margin: 4px 4px 0px 4px;
 --jp-toolbar-active-background: var(--md-grey-300);

 /\* Statusbar specific styles \*/

 --jp-statusbar-height: 24px;

 /\* Input field styles \*/

 --jp-input-box-shadow: inset 0 0 2px var(--md-blue-300);
 --jp-input-active-background: var(--jp-layout-color1);
 --jp-input-hover-background: var(--jp-layout-color1);
 --jp-input-background: var(--md-grey-100);
 --jp-input-border-color: var(--jp-border-color1);
 --jp-input-active-border-color: var(--jp-brand-color1);
 --jp-input-active-box-shadow-color: rgba(19, 124, 189, 0.3);

 /\* General editor styles \*/

 --jp-editor-selected-background: #d9d9d9;
 --jp-editor-selected-focused-background: #d7d4f0;
 --jp-editor-cursor-color: var(--jp-ui-font-color0);

 /\* Code mirror specific styles \*/

 --jp-mirror-editor-keyword-color: #008000;
 --jp-mirror-editor-atom-color: #88f;
 --jp-mirror-editor-number-color: #080;
 --jp-mirror-editor-def-color: #00f;
 --jp-mirror-editor-variable-color: var(--md-grey-900);
 --jp-mirror-editor-variable-2-color: #05a;
 --jp-mirror-editor-variable-3-color: #085;
 --jp-mirror-editor-punctuation-color: #05a;
 --jp-mirror-editor-property-color: #05a;
 --jp-mirror-editor-operator-color: #aa22ff;
 --jp-mirror-editor-comment-color: #408080;
 --jp-mirror-editor-string-color: #ba2121;
 --jp-mirror-editor-string-2-color: #708;
 --jp-mirror-editor-meta-color: #aa22ff;
 --jp-mirror-editor-qualifier-color: #555;
 --jp-mirror-editor-builtin-color: #008000;
 --jp-mirror-editor-bracket-color: #997;
 --jp-mirror-editor-tag-color: #170;
 --jp-mirror-editor-attribute-color: #00c;
 --jp-mirror-editor-header-color: blue;
 --jp-mirror-editor-quote-color: #090;
 --jp-mirror-editor-link-color: #00c;
 --jp-mirror-editor-error-color: #f00;
 --jp-mirror-editor-hr-color: #999;

 /\* Vega extension styles \*/

 --jp-vega-background: white;

 /\* Sidebar-related styles \*/

 --jp-sidebar-min-width: 250px;

 /\* Search-related styles \*/

 --jp-search-toggle-off-opacity: 0.5;
 --jp-search-toggle-hover-opacity: 0.8;
 --jp-search-toggle-on-opacity: 1;
 --jp-search-selected-match-background-color: rgb(245, 200, 0);
 --jp-search-selected-match-color: black;
 --jp-search-unselected-match-background-color: var(
 --jp-inverse-layout-color0
 );
 --jp-search-unselected-match-color: var(--jp-ui-inverse-font-color0);

 /\* Icon colors that work well with light or dark backgrounds \*/
 --jp-icon-contrast-color0: var(--md-purple-600);
 --jp-icon-contrast-color1: var(--md-green-600);
 --jp-icon-contrast-color2: var(--md-pink-600);
 --jp-icon-contrast-color3: var(--md-blue-600);
}


/\* Force rendering true colors when outputing to pdf \*/
\* {
 -webkit-print-color-adjust: exact;
}

/\* Misc \*/
a.anchor-link {
 display: none;
}

/\* Input area styling \*/
.jp-InputArea {
 overflow: hidden;
}

.jp-InputArea-editor {
 overflow: hidden;
}

.CodeMirror.cm-s-jupyter .highlight pre {
/\* weird, but --jp-code-padding defined to be 5px but 4px horizontal padding is hardcoded for pre.CodeMirror-line \*/
 padding: var(--jp-code-padding) 4px;
 margin: 0;

 font-family: inherit;
 font-size: inherit;
 line-height: inherit;
 color: inherit;

}

.jp-OutputArea-output pre {
 line-height: inherit;
 font-family: inherit;
}

.jp-RenderedText pre {
 color: var(--jp-content-font-color1);
 font-size: var(--jp-code-font-size);
}

/\* Using table instead of flexbox so that we can use break-inside property \*/
/\* CSS rules under this comment should not be required anymore after we move to the JupyterLab 4.0 CSS \*/


.jp-CodeCell.jp-mod-outputsScrolled .jp-OutputArea-prompt {
 min-width: calc(
 var(--jp-cell-prompt-width) - var(--jp-private-cell-scrolling-output-offset)
 );
}

.jp-OutputArea-child {
 display: table;
 width: 100%;
}

.jp-OutputPrompt {
 display: table-cell;
 vertical-align: top;
 min-width: var(--jp-cell-prompt-width);
}

body[data-format='mobile'] .jp-OutputPrompt {
 display: table-row;
}

.jp-OutputArea-output {
 display: table-cell;
 width: 100%;
}

body[data-format='mobile'] .jp-OutputArea-child .jp-OutputArea-output {
 display: table-row;
}

.jp-OutputArea-output.jp-OutputArea-executeResult {
 width: 100%;
}

/\* Hiding the collapser by default \*/
.jp-Collapser {
 display: none;
}

@media print {
 .jp-Cell-inputWrapper,
 .jp-Cell-outputWrapper {
 display: block;
 }

 .jp-OutputArea-child {
 break-inside: avoid-page;
 }
}


 


 init\_mathjax = function() {
 if (window.MathJax) {
 // MathJax loaded
 MathJax.Hub.Config({
 TeX: {
 equationNumbers: {
 autoNumber: "AMS",
 useLabelIds: true
 }
 },
 tex2jax: {
 inlineMath: [ ['$','$'], ["\\(","\\)"] ],
 displayMath: [ ['$$','$$'], ["\\[","\\]"] ],
 processEscapes: true,
 processEnvironments: true
 },
 displayAlign: 'center',
 CommonHTML: {
 linebreaks: {
 automatic: true
 }
 }
 });

 MathJax.Hub.Queue(["Typeset", MathJax.Hub]);
 }
 }
 init\_mathjax();
 








## Exploratory Data Analysis with TED data[¶](#Exploratory-Data-Analysis-with-TED-data)












### What is EDA?[¶](#What-is-EDA?)

EDA stands for Exploratory Data Analysis. This analysis is essential to understand a given dataset. Usually to perform an EDA ,**we are asking**:


* What shape does the dataset have?
* How does the data look like?
* How many records?
* How many columns?
* What is the dataset about?
* What columns represent?
* What are the types for each column?


Once we understand the format, we can continue to **business questions about the dataset**:


* Is there any question given to answer over this dataset?
* What information can this dataset provide that is crucial to business?
* What dataset transformations will give us such information/answers?


**Iterate over:**


* Once an answer is given: what other questions can be asked?
* What visualization will help understand the dataset/answer this question?


-Once the visualization is rendered, what is surprising about the result?


* Did the visualization answer our question?
* Did the visualization bring anything new? What can be inferred?












Kaggle site (datasets) https://www.kaggle.com/datasets Recommended to practice EDA and others Competitions, Models,Discussions, etc












### Credit to the original creator[¶](#Credit-to-the-original-creator)

Credit to @justmarkham
https://github.com/justmarkham/pycon-2019-tutorial/blob/master/environment.yml


I wanted to recreate the jupyter notebook step by step and make it public as a learning exercise, also adding insight on some points












Dataset https://github.com/justmarkham/pycon-2019-tutorial












Pycon session reference https://www.youtube.com/watch?v=dPwLlJkSHLo












## Retrieving the dataset to work with it[¶](#Retrieving-the-dataset-to-work-with-it)

This one is a dataset containing info on several Ted Talks. Pandas has built-in features to produce plots that we will be using throughout this notebook.










In [ ]:



```
import pandas as pd
import matplotlib.pyplot as plt
%matplotlib inline
ted = pd.read\_csv('ted.csv')

```












Using pandas features to plot number of comments on the ted dataset. The ted.comments part makes reference to the column "comments" on the "ted" dataframe.










In [ ]:



```
ted.comments.plot()

```










Out[ ]:


```
<Axes: >
```






![](data:image/png;base64,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)











## Pandas version set up[¶](#Pandas-version-set-up)










In [ ]:



```
pd.\_\_version\_\_

```










Out[ ]:


```
'2.0.1'
```












## TED talks dataset shape analysis[¶](#TED-talks-dataset-shape-analysis)










In [ ]:



```
ted = pd.read\_csv('ted.csv')

```










In [ ]:



```
ted

```










Out[ ]:



 .dataframe tbody tr th:only-of-type {
 vertical-align: middle;
 }

 .dataframe tbody tr th {
 vertical-align: top;
 }

 .dataframe thead th {
 text-align: right;
 }



|  | comments | description | duration | event | film\_date | languages | main\_speaker | name | num\_speaker | published\_date | ratings | related\_talks | speaker\_occupation | tags | title | url | views |
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
| 0 | 4553 | Sir Ken Robinson makes an entertaining and pro... | 1164 | TED2006 | 1140825600 | 60 | Ken Robinson | Ken Robinson: Do schools kill creativity? | 1 | 1151367060 | [{'id': 7, 'name': 'Funny', 'count': 19645}, {... | [{'id': 865, 'hero': 'https://pe.tedcdn.com/im... | Author/educator | ['children', 'creativity', 'culture', 'dance',... | Do schools kill creativity? | https://www.ted.com/talks/ken\_robinson\_says\_sc... | 47227110 |
| 1 | 265 | With the same humor and humanity he exuded in ... | 977 | TED2006 | 1140825600 | 43 | Al Gore | Al Gore: Averting the climate crisis | 1 | 1151367060 | [{'id': 7, 'name': 'Funny', 'count': 544}, {'i... | [{'id': 243, 'hero': 'https://pe.tedcdn.com/im... | Climate advocate | ['alternative energy', 'cars', 'climate change... | Averting the climate crisis | https://www.ted.com/talks/al\_gore\_on\_averting\_... | 3200520 |
| 2 | 124 | New York Times columnist David Pogue takes aim... | 1286 | TED2006 | 1140739200 | 26 | David Pogue | David Pogue: Simplicity sells | 1 | 1151367060 | [{'id': 7, 'name': 'Funny', 'count': 964}, {'i... | [{'id': 1725, 'hero': 'https://pe.tedcdn.com/i... | Technology columnist | ['computers', 'entertainment', 'interface desi... | Simplicity sells | https://www.ted.com/talks/david\_pogue\_says\_sim... | 1636292 |
| 3 | 200 | In an emotionally charged talk, MacArthur-winn... | 1116 | TED2006 | 1140912000 | 35 | Majora Carter | Majora Carter: Greening the ghetto | 1 | 1151367060 | [{'id': 3, 'name': 'Courageous', 'count': 760}... | [{'id': 1041, 'hero': 'https://pe.tedcdn.com/i... | Activist for environmental justice | ['MacArthur grant', 'activism', 'business', 'c... | Greening the ghetto | https://www.ted.com/talks/majora\_carter\_s\_tale... | 1697550 |
| 4 | 593 | You've never seen data presented like this. Wi... | 1190 | TED2006 | 1140566400 | 48 | Hans Rosling | Hans Rosling: The best stats you've ever seen | 1 | 1151440680 | [{'id': 9, 'name': 'Ingenious', 'count': 3202}... | [{'id': 2056, 'hero': 'https://pe.tedcdn.com/i... | Global health expert; data visionary | ['Africa', 'Asia', 'Google', 'demo', 'economic... | The best stats you've ever seen | https://www.ted.com/talks/hans\_rosling\_shows\_t... | 12005869 |
| ... | ... | ... | ... | ... | ... | ... | ... | ... | ... | ... | ... | ... | ... | ... | ... | ... | ... |
| 2545 | 17 | Between 2008 and 2016, the United States depor... | 476 | TED2017 | 1496707200 | 4 | Duarte Geraldino | Duarte Geraldino: What we're missing in the de... | 1 | 1505851216 | [{'id': 3, 'name': 'Courageous', 'count': 24},... | [{'id': 2596, 'hero': 'https://pe.tedcdn.com/i... | Journalist | ['TED Residency', 'United States', 'community'... | What we're missing in the debate about immigra... | https://www.ted.com/talks/duarte\_geraldino\_wha... | 450430 |
| 2546 | 6 | How can you study Mars without a spaceship? He... | 290 | TED2017 | 1492992000 | 3 | Armando Azua-Bustos | Armando Azua-Bustos: The most Martian place on... | 1 | 1505919737 | [{'id': 22, 'name': 'Fascinating', 'count': 32... | [{'id': 2491, 'hero': 'https://pe.tedcdn.com/i... | Astrobiologist | ['Mars', 'South America', 'TED Fellows', 'astr... | The most Martian place on Earth | https://www.ted.com/talks/armando\_azua\_bustos\_... | 417470 |
| 2547 | 10 | Science fiction visions of the future show us ... | 651 | TED2017 | 1492992000 | 1 | Radhika Nagpal | Radhika Nagpal: What intelligent machines can ... | 1 | 1506006095 | [{'id': 1, 'name': 'Beautiful', 'count': 14}, ... | [{'id': 2346, 'hero': 'https://pe.tedcdn.com/i... | Robotics engineer | ['AI', 'ants', 'fish', 'future', 'innovation',... | What intelligent machines can learn from a sch... | https://www.ted.com/talks/radhika\_nagpal\_what\_... | 375647 |
| 2548 | 32 | In an unmissable talk about race and politics ... | 1100 | TEDxMileHigh | 1499472000 | 1 | Theo E.J. Wilson | Theo E.J. Wilson: A black man goes undercover ... | 1 | 1506024042 | [{'id': 11, 'name': 'Longwinded', 'count': 3},... | [{'id': 2512, 'hero': 'https://pe.tedcdn.com/i... | Public intellectual | ['Internet', 'TEDx', 'United States', 'communi... | A black man goes undercover in the alt-right | https://www.ted.com/talks/theo\_e\_j\_wilson\_a\_bl... | 419309 |
| 2549 | 8 | With more than half of the world population li... | 519 | TED2017 | 1492992000 | 1 | Karoliina Korppoo | Karoliina Korppoo: How a video game might help... | 1 | 1506092422 | [{'id': 21, 'name': 'Unconvincing', 'count': 2... | [{'id': 2682, 'hero': 'https://pe.tedcdn.com/i... | Game designer | ['cities', 'design', 'future', 'infrastructure... | How a video game might help us build better ci... | https://www.ted.com/talks/karoliina\_korppoo\_ho... | 391721 |


2550 rows × 17 columns












In [ ]:



```
ted.head()

```










Out[ ]:



 .dataframe tbody tr th:only-of-type {
 vertical-align: middle;
 }

 .dataframe tbody tr th {
 vertical-align: top;
 }

 .dataframe thead th {
 text-align: right;
 }



|  | comments | description | duration | event | film\_date | languages | main\_speaker | name | num\_speaker | published\_date | ratings | related\_talks | speaker\_occupation | tags | title | url | views |
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
| 0 | 4553 | Sir Ken Robinson makes an entertaining and pro... | 1164 | TED2006 | 1140825600 | 60 | Ken Robinson | Ken Robinson: Do schools kill creativity? | 1 | 1151367060 | [{'id': 7, 'name': 'Funny', 'count': 19645}, {... | [{'id': 865, 'hero': 'https://pe.tedcdn.com/im... | Author/educator | ['children', 'creativity', 'culture', 'dance',... | Do schools kill creativity? | https://www.ted.com/talks/ken\_robinson\_says\_sc... | 47227110 |
| 1 | 265 | With the same humor and humanity he exuded in ... | 977 | TED2006 | 1140825600 | 43 | Al Gore | Al Gore: Averting the climate crisis | 1 | 1151367060 | [{'id': 7, 'name': 'Funny', 'count': 544}, {'i... | [{'id': 243, 'hero': 'https://pe.tedcdn.com/im... | Climate advocate | ['alternative energy', 'cars', 'climate change... | Averting the climate crisis | https://www.ted.com/talks/al\_gore\_on\_averting\_... | 3200520 |
| 2 | 124 | New York Times columnist David Pogue takes aim... | 1286 | TED2006 | 1140739200 | 26 | David Pogue | David Pogue: Simplicity sells | 1 | 1151367060 | [{'id': 7, 'name': 'Funny', 'count': 964}, {'i... | [{'id': 1725, 'hero': 'https://pe.tedcdn.com/i... | Technology columnist | ['computers', 'entertainment', 'interface desi... | Simplicity sells | https://www.ted.com/talks/david\_pogue\_says\_sim... | 1636292 |
| 3 | 200 | In an emotionally charged talk, MacArthur-winn... | 1116 | TED2006 | 1140912000 | 35 | Majora Carter | Majora Carter: Greening the ghetto | 1 | 1151367060 | [{'id': 3, 'name': 'Courageous', 'count': 760}... | [{'id': 1041, 'hero': 'https://pe.tedcdn.com/i... | Activist for environmental justice | ['MacArthur grant', 'activism', 'business', 'c... | Greening the ghetto | https://www.ted.com/talks/majora\_carter\_s\_tale... | 1697550 |
| 4 | 593 | You've never seen data presented like this. Wi... | 1190 | TED2006 | 1140566400 | 48 | Hans Rosling | Hans Rosling: The best stats you've ever seen | 1 | 1151440680 | [{'id': 9, 'name': 'Ingenious', 'count': 3202}... | [{'id': 2056, 'hero': 'https://pe.tedcdn.com/i... | Global health expert; data visionary | ['Africa', 'Asia', 'Google', 'demo', 'economic... | The best stats you've ever seen | https://www.ted.com/talks/hans\_rosling\_shows\_t... | 12005869 |












In [ ]:



```
ted.shape

```










Out[ ]:


```
(2550, 17)
```










In [ ]:



```
ted.dtypes

```










Out[ ]:


```
comments               int64
description           object
duration               int64
event                 object
film_date              int64
languages              int64
main_speaker          object
name                  object
num_speaker            int64
published_date         int64
ratings               object
related_talks         object
speaker_occupation    object
tags                  object
title                 object
url                   object
views                  int64
dtype: object
```












## Object columns can hold also dictionaries, lists and structures too ( additionally for strings)[¶](#Object-columns-can-hold-also-dictionaries,-lists-and-structures-too-(-additionally-for-strings))












1. What part of this dataset contains useful info? Tell me the sum of NA records on the dataset










In [ ]:



```
ted.isna().sum()

```










Out[ ]:


```
comments              0
description           0
duration              0
event                 0
film_date             0
languages             0
main_speaker          0
name                  0
num_speaker           0
published_date        0
ratings               0
related_talks         0
speaker_occupation    6
tags                  0
title                 0
url                   0
views                 0
dtype: int64
```












## Which talks provoke the most online discussion?[¶](#Which-talks-provoke-the-most-online-discussion?)












In this case we start with a business question: "*What are the talks that are more provokative ( produce the most online discussion)*? 
So creating a new column that can tell the amount of comments related to the number of views. We are interested in talks that generate the max number of comments per view.










In [ ]:



```
ted['comments\_per\_view'] = ted.comments / ted.views

```










In [ ]:



```
ted.sort\_values('comments\_per\_view').tail()

```










Out[ ]:



 .dataframe tbody tr th:only-of-type {
 vertical-align: middle;
 }

 .dataframe tbody tr th {
 vertical-align: top;
 }

 .dataframe thead th {
 text-align: right;
 }



|  | comments | description | duration | event | film\_date | languages | main\_speaker | name | num\_speaker | published\_date | ratings | related\_talks | speaker\_occupation | tags | title | url | views | comments\_per\_view |
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
| 954 | 2492 | Janet Echelman found her true voice as an arti... | 566 | TED2011 | 1299110400 | 35 | Janet Echelman | Janet Echelman: Taking imagination seriously | 1 | 1307489760 | [{'id': 23, 'name': 'Jaw-dropping', 'count': 3... | [{'id': 453, 'hero': 'https://pe.tedcdn.com/im... | Artist | ['art', 'cities', 'culture', 'data', 'design',... | Taking imagination seriously | https://www.ted.com/talks/janet\_echelman | 1832930 | 0.001360 |
| 694 | 1502 | Filmmaker Sharmeen Obaid-Chinoy takes on a ter... | 489 | TED2010 | 1265760000 | 32 | Sharmeen Obaid-Chinoy | Sharmeen Obaid-Chinoy: Inside a school for sui... | 1 | 1274865960 | [{'id': 23, 'name': 'Jaw-dropping', 'count': 3... | [{'id': 171, 'hero': 'https://pe.tedcdn.com/im... | Filmmaker | ['TED Fellows', 'children', 'culture', 'film',... | Inside a school for suicide bombers | https://www.ted.com/talks/sharmeen\_obaid\_chino... | 1057238 | 0.001421 |
| 96 | 6404 | Richard Dawkins urges all atheists to openly s... | 1750 | TED2002 | 1012608000 | 42 | Richard Dawkins | Richard Dawkins: Militant atheism | 1 | 1176689220 | [{'id': 3, 'name': 'Courageous', 'count': 3236... | [{'id': 86, 'hero': 'https://pe.tedcdn.com/ima... | Evolutionary biologist | ['God', 'atheism', 'culture', 'religion', 'sci... | Militant atheism | https://www.ted.com/talks/richard\_dawkins\_on\_m... | 4374792 | 0.001464 |
| 803 | 834 | David Bismark demos a new system for voting th... | 422 | TEDGlobal 2010 | 1279065600 | 36 | David Bismark | David Bismark: E-voting without fraud | 1 | 1288685640 | [{'id': 25, 'name': 'OK', 'count': 111}, {'id'... | [{'id': 803, 'hero': 'https://pe.tedcdn.com/im... | Voting system designer | ['culture', 'democracy', 'design', 'global iss... | E-voting without fraud | https://www.ted.com/talks/david\_bismark\_e\_voti... | 543551 | 0.001534 |
| 744 | 649 | Hours before New York lawmakers rejected a key... | 453 | New York State Senate | 1259712000 | 0 | Diane J. Savino | Diane J. Savino: The case for same-sex marriage | 1 | 1282062180 | [{'id': 25, 'name': 'OK', 'count': 100}, {'id'... | [{'id': 217, 'hero': 'https://pe.tedcdn.com/im... | Senator | ['God', 'LGBT', 'culture', 'government', 'law'... | The case for same-sex marriage | https://www.ted.com/talks/diane\_j\_savino\_the\_c... | 292395 | 0.002220 |














Views per comment to make it more interpretable










In [ ]:



```
ted.sort\_values('comments\_per\_view').head()

```










Out[ ]:



 .dataframe tbody tr th:only-of-type {
 vertical-align: middle;
 }

 .dataframe tbody tr th {
 vertical-align: top;
 }

 .dataframe thead th {
 text-align: right;
 }



|  | comments | description | duration | event | film\_date | languages | main\_speaker | name | num\_speaker | published\_date | ratings | related\_talks | speaker\_occupation | tags | title | url | views | comments\_per\_view |
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
| 2534 | 2 | What the astronauts felt when they saw Earth f... | 725 | TEDxSkoll | 1491523200 | 1 | Benjamin Grant | Benjamin Grant: What it feels like to see Eart... | 1 | 1504814438 | [{'id': 10, 'name': 'Inspiring', 'count': 46},... | [{'id': 2511, 'hero': 'https://pe.tedcdn.com/i... | Author | ['TEDx', 'art', 'climate change', 'environment... | What it feels like to see Earth from space | https://www.ted.com/talks/benjamin\_grant\_what\_... | 646174 | 0.000003 |
| 2501 | 3 | Meet Françoise Mouly, The New Yorker's art dir... | 509 | TEDNYC | 1488931200 | 12 | Françoise Mouly | Françoise Mouly: The stories behind The New Yo... | 1 | 1501770244 | [{'id': 7, 'name': 'Funny', 'count': 10}, {'id... | [{'id': 2479, 'hero': 'https://pe.tedcdn.com/i... | Art editor | ['TEDNYC', 'art', 'creativity', 'culture', 'de... | The stories behind The New Yorker's iconic covers | https://www.ted.com/talks/francoise\_mouly\_the\_... | 839040 | 0.000004 |
| 2542 | 3 | In the century-old statues that occupy Cape To... | 795 | TEDGlobal 2017 | 1503792000 | 1 | Sethembile Msezane | Sethembile Msezane: Living sculptures that sta... | 1 | 1505488093 | [{'id': 1, 'name': 'Beautiful', 'count': 41}, ... | [{'id': 2873, 'hero': 'https://pe.tedcdn.com/i... | Artist | ['Africa', 'activism', 'art', 'community', 'hi... | Living sculptures that stand for history's truths | https://www.ted.com/talks/sethembile\_msezane\_l... | 542088 | 0.000006 |
| 2528 | 3 | Digital archaeologist Chance Coughenour is usi... | 717 | TEDxHamburg | 1465344000 | 5 | Chance Coughenour | Chance Coughenour: How your pictures can help ... | 1 | 1504209631 | [{'id': 9, 'name': 'Ingenious', 'count': 16}, ... | [{'id': 2673, 'hero': 'https://pe.tedcdn.com/i... | Digital archaeologist | ['TEDx', 'ancient world', 'archaeology', 'cons... | How your pictures can help reclaim lost history | https://www.ted.com/talks/chance\_coughenour\_ho... | 539207 | 0.000006 |
| 2494 | 7 | Jimmy Lin is developing technologies to catch ... | 730 | TED2017 | 1492992000 | 10 | Jimmy Lin | Jimmy Lin: A simple new blood test that can ca... | 1 | 1500994384 | [{'id': 1, 'name': 'Beautiful', 'count': 7}, {... | [{'id': 2498, 'hero': 'https://pe.tedcdn.com/i... | Geneticist | ['DNA', 'TED Fellows', 'biology', 'cancer', 'd... | A simple new blood test that can catch cancer ... | https://www.ted.com/talks/jimmy\_lin\_a\_simple\_n... | 1005506 | 0.000007 |












In [ ]:



```
ted['views\_per\_comment'] = ted.views/ted.comments

```










In [ ]:



```
ted.sort\_values('views\_per\_comment')

```










Out[ ]:



 .dataframe tbody tr th:only-of-type {
 vertical-align: middle;
 }

 .dataframe tbody tr th {
 vertical-align: top;
 }

 .dataframe thead th {
 text-align: right;
 }



|  | comments | description | duration | event | film\_date | languages | main\_speaker | name | num\_speaker | published\_date | ratings | related\_talks | speaker\_occupation | tags | title | url | views | comments\_per\_view | views\_per\_comment |
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
| 744 | 649 | Hours before New York lawmakers rejected a key... | 453 | New York State Senate | 1259712000 | 0 | Diane J. Savino | Diane J. Savino: The case for same-sex marriage | 1 | 1282062180 | [{'id': 25, 'name': 'OK', 'count': 100}, {'id'... | [{'id': 217, 'hero': 'https://pe.tedcdn.com/im... | Senator | ['God', 'LGBT', 'culture', 'government', 'law'... | The case for same-sex marriage | https://www.ted.com/talks/diane\_j\_savino\_the\_c... | 292395 | 0.002220 | 450.531587 |
| 803 | 834 | David Bismark demos a new system for voting th... | 422 | TEDGlobal 2010 | 1279065600 | 36 | David Bismark | David Bismark: E-voting without fraud | 1 | 1288685640 | [{'id': 25, 'name': 'OK', 'count': 111}, {'id'... | [{'id': 803, 'hero': 'https://pe.tedcdn.com/im... | Voting system designer | ['culture', 'democracy', 'design', 'global iss... | E-voting without fraud | https://www.ted.com/talks/david\_bismark\_e\_voti... | 543551 | 0.001534 | 651.739808 |
| 96 | 6404 | Richard Dawkins urges all atheists to openly s... | 1750 | TED2002 | 1012608000 | 42 | Richard Dawkins | Richard Dawkins: Militant atheism | 1 | 1176689220 | [{'id': 3, 'name': 'Courageous', 'count': 3236... | [{'id': 86, 'hero': 'https://pe.tedcdn.com/ima... | Evolutionary biologist | ['God', 'atheism', 'culture', 'religion', 'sci... | Militant atheism | https://www.ted.com/talks/richard\_dawkins\_on\_m... | 4374792 | 0.001464 | 683.134291 |
| 694 | 1502 | Filmmaker Sharmeen Obaid-Chinoy takes on a ter... | 489 | TED2010 | 1265760000 | 32 | Sharmeen Obaid-Chinoy | Sharmeen Obaid-Chinoy: Inside a school for sui... | 1 | 1274865960 | [{'id': 23, 'name': 'Jaw-dropping', 'count': 3... | [{'id': 171, 'hero': 'https://pe.tedcdn.com/im... | Filmmaker | ['TED Fellows', 'children', 'culture', 'film',... | Inside a school for suicide bombers | https://www.ted.com/talks/sharmeen\_obaid\_chino... | 1057238 | 0.001421 | 703.886818 |
| 954 | 2492 | Janet Echelman found her true voice as an arti... | 566 | TED2011 | 1299110400 | 35 | Janet Echelman | Janet Echelman: Taking imagination seriously | 1 | 1307489760 | [{'id': 23, 'name': 'Jaw-dropping', 'count': 3... | [{'id': 453, 'hero': 'https://pe.tedcdn.com/im... | Artist | ['art', 'cities', 'culture', 'data', 'design',... | Taking imagination seriously | https://www.ted.com/talks/janet\_echelman | 1832930 | 0.001360 | 735.525682 |
| ... | ... | ... | ... | ... | ... | ... | ... | ... | ... | ... | ... | ... | ... | ... | ... | ... | ... | ... | ... |
| 2494 | 7 | Jimmy Lin is developing technologies to catch ... | 730 | TED2017 | 1492992000 | 10 | Jimmy Lin | Jimmy Lin: A simple new blood test that can ca... | 1 | 1500994384 | [{'id': 1, 'name': 'Beautiful', 'count': 7}, {... | [{'id': 2498, 'hero': 'https://pe.tedcdn.com/i... | Geneticist | ['DNA', 'TED Fellows', 'biology', 'cancer', 'd... | A simple new blood test that can catch cancer ... | https://www.ted.com/talks/jimmy\_lin\_a\_simple\_n... | 1005506 | 0.000007 | 143643.714286 |
| 2528 | 3 | Digital archaeologist Chance Coughenour is usi... | 717 | TEDxHamburg | 1465344000 | 5 | Chance Coughenour | Chance Coughenour: How your pictures can help ... | 1 | 1504209631 | [{'id': 9, 'name': 'Ingenious', 'count': 16}, ... | [{'id': 2673, 'hero': 'https://pe.tedcdn.com/i... | Digital archaeologist | ['TEDx', 'ancient world', 'archaeology', 'cons... | How your pictures can help reclaim lost history | https://www.ted.com/talks/chance\_coughenour\_ho... | 539207 | 0.000006 | 179735.666667 |
| 2542 | 3 | In the century-old statues that occupy Cape To... | 795 | TEDGlobal 2017 | 1503792000 | 1 | Sethembile Msezane | Sethembile Msezane: Living sculptures that sta... | 1 | 1505488093 | [{'id': 1, 'name': 'Beautiful', 'count': 41}, ... | [{'id': 2873, 'hero': 'https://pe.tedcdn.com/i... | Artist | ['Africa', 'activism', 'art', 'community', 'hi... | Living sculptures that stand for history's truths | https://www.ted.com/talks/sethembile\_msezane\_l... | 542088 | 0.000006 | 180696.000000 |
| 2501 | 3 | Meet Françoise Mouly, The New Yorker's art dir... | 509 | TEDNYC | 1488931200 | 12 | Françoise Mouly | Françoise Mouly: The stories behind The New Yo... | 1 | 1501770244 | [{'id': 7, 'name': 'Funny', 'count': 10}, {'id... | [{'id': 2479, 'hero': 'https://pe.tedcdn.com/i... | Art editor | ['TEDNYC', 'art', 'creativity', 'culture', 'de... | The stories behind The New Yorker's iconic covers | https://www.ted.com/talks/francoise\_mouly\_the\_... | 839040 | 0.000004 | 279680.000000 |
| 2534 | 2 | What the astronauts felt when they saw Earth f... | 725 | TEDxSkoll | 1491523200 | 1 | Benjamin Grant | Benjamin Grant: What it feels like to see Eart... | 1 | 1504814438 | [{'id': 10, 'name': 'Inspiring', 'count': 46},... | [{'id': 2511, 'hero': 'https://pe.tedcdn.com/i... | Author | ['TEDx', 'art', 'climate change', 'environment... | What it feels like to see Earth from space | https://www.ted.com/talks/benjamin\_grant\_what\_... | 646174 | 0.000003 | 323087.000000 |


2550 rows × 19 columns














Checking in graphical way the comments distribution. Line plot is the first choice ( but no the best one)
X= index
Y= value of the comment












This graph doesn't have a time component, line plot is not adequate.












This plot is good, however it doesn't provide detail that we can use. We just see that there are more TED talks that have between 0-1000 comments. We need more detail to make sure this intuition is true.












## Visualization of the comment distribution[¶](#Visualization-of-the-comment-distribution)












A histogram plot is more adequate for frequency distribution










In [ ]:



```
ted.comments.plot(kind='hist')

```










Out[ ]:


```
<Axes: ylabel='Frequency'>
```






![](data:image/png;base64,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)











Vast majority is on the left of 1000, so we would need to filter to understand more












So what does this look like in detail. Let's filter the dataframe by the ones that have less than 1000










In [ ]:



```
ted[ted.comments>=1000].shape

```










Out[ ]:


```
(32, 19)
```












By removing the ted talks with more than 1000 comments we cut out information that is not relevant to the question asked. Just 32 records!












This is the distribution of the ted talks within the ones with less than 1000 comments










In [ ]:



```
ted[ted.comments<1000].comments.plot(kind='hist')

```










Out[ ]:


```
<Axes: ylabel='Frequency'>
```






![](data:image/png;base64,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hBSI7r//fj3zzDMyxoS7nha++uorjR07Vt26dXPuZtu4caPTb4zRjBkz1KNHDyUlJSk7O7vFj8/W1tYqLy9PbrdbKSkpKigoUENDQ6vXDgAA2oaQvjL78MMP9cEHH2jVqlW66KKL1L59+6D+N998MyzFff311xoyZIiuu+46rVq1Smeffbb27NmjLl26OGPmzp2r+fPna/HixcrIyND06dOVk5OjTz75RB06dJAk5eXl6cCBAyopKVFTU5PGjRunCRMmaOnSpWGpEwAAtG0hBaKUlBTdfPPN4a6lhTlz5ig9PV0LFy502r77G2rGGD399NN69NFHdeONN0qSXnnlFXk8Hq1YsUJjxozRrl27tHr1am3YsEGZmZmSpGeffVYjR47Ur371K6WlpbX6PAAAQGwLKRB9N6C0prfffls5OTn6yU9+orVr1+qcc87R3XffrfHjx0uSPv/8c/l8PmVnZzvvSU5O1uDBg1VWVqYxY8aorKxMKSkpThiSpOzsbMXFxam8vDwiwQ4AAMS2kK4hkqRjx47pj3/8o1544QUdOnRIkrR///6wXpvz2WefacGCBerTp4/ee+893XXXXbr33nu1ePFiSZLP55MkeTyeoPd5PB6nz+fzKTU1Nag/Pj5eXbt2dcacqLGxUX6/P2gDAABnrpDOEH355ZcaMWKEqqqq1NjYqH//939X586dNWfOHDU2Nqq4uDgsxQUCAWVmZjq/j3bZZZdpx44dKi4uVn5+fliOcTJFRUV6/PHHW23/AAAgtoR0hmjSpEnKzMzU119/raSkJKf95ptvVmlpadiK69Gjh/r37x/U1q9fP1VVVUmSvF6vJKm6ujpoTHV1tdPn9XpVU1MT1H/s2DHV1tY6Y040bdo01dfXO9vevXvDMh8AABCbQgpEf/rTn/Too48qISEhqL1379766quvwlKYJA0ZMkSVlZVBbbt373Z+RDYjI0NerzcohPn9fpWXlysrK0uSlJWVpbq6OlVUVDhj1qxZo0AgoMGDB5/0uImJiXK73UEbAAA4c4X0lVkgEFBzc3OL9n379qlz584/uKjj7rvvPl199dV68skn9V//9V9av369XnzxRb344ouSJJfLpcmTJ+uJJ55Qnz59nNvu09LSdNNNN0n69ozSiBEjNH78eBUXF6upqUkTJ07UmDFjuMMMAABICvEM0fDhw/X00087r10ulxoaGvTYY4+F9ec8rrjiCr311lt67bXXNGDAAM2cOVNPP/208vLynDEPPfSQ7rnnHk2YMEFXXHGFGhoatHr1aucZRJK0ZMkS9e3bV8OGDdPIkSM1dOhQJ1QBAAC4TAiPm963b59ycnJkjNGePXuUmZmpPXv2qHv37lq3bl2Lu7raOr/fr+TkZNXX17fK12e9p74b9n2ipS9m50a7BABABJ3O53dIX5mde+652rp1q5YtW6Zt27apoaFBBQUFysvLC7rIGgAAoC0IKRBJ3z7LZ+zYseGsBQAAICpCCkSvvPLK9/bfdtttIRUDAAAQDSEFokmTJgW9bmpq0jfffKOEhAR17NiRQAQAANqUkO4y+/rrr4O2hoYGVVZWaujQoXrttdfCXSMAAECrCvm3zE7Up08fzZ49u8XZIwAAgFgXtkAkfXuh9f79+8O5SwAAgFYX0jVEb7/9dtBrY4wOHDig3/72txoyZEhYCgMAAIiUkALR8Z/FOM7lcunss8/Wj370I/36178OR10AAAARE/JvmQEAAJwpwnoNEQAAQFsU0hmiKVOmnPLYefPmhXIIAACAiAkpEG3evFmbN29WU1OTLrzwQknS7t271a5dO11++eXOOJfLFZ4qAQAAWlFIgeiGG25Q586dtXjxYnXp0kXStw9rHDdunK655hrdf//9YS0SAACgNYV0DdGvf/1rFRUVOWFIkrp06aInnniCu8wAAECbE1Ig8vv9OnjwYIv2gwcP6tChQz+4KAAAgEgKKRDdfPPNGjdunN58803t27dP+/bt0//8z/+ooKBAo0aNCneNAAAArSqka4iKi4v1wAMP6Gc/+5mampq+3VF8vAoKCvTUU0+FtUAAAIDWFlIg6tixo55//nk99dRT+utf/ypJOu+889SpU6ewFgcAABAJP+jBjAcOHNCBAwfUp08fderUScaYcNUFAAAQMSEFor///e8aNmyYLrjgAo0cOVIHDhyQJBUUFHDLPQAAaHNCCkT33Xef2rdvr6qqKnXs2NFp/+lPf6rVq1eHrTgAAIBICOkaovfff1/vvfeezj333KD2Pn366MsvvwxLYQAAAJES0hmiw4cPB50ZOq62tlaJiYk/uCgAAIBICikQXXPNNXrllVec1y6XS4FAQHPnztV1110XtuIAAAAiIaSvzObOnathw4Zp48aNOnr0qB566CHt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PkN0ovr6eklS165dJUkVFRVqampSdna2M6Zv377q2bOnysrKJEllZWUaOHCgE4YkKScnR36/Xzt37jzpcRobG+X3+4M2AABw5mozgSgQCGjy5MkaMmSIBgwYIEny+XxKSEhQSkpK0FiPxyOfz+eM+W4YOt5/vO9kioqKlJyc7Gzp6elhng0AAIglbSYQFRYWaseOHVq2bFmrH2vatGmqr693tr1797b6MQEAQPTER7uAUzFx4kStXLlS69at07nnnuu0e71eHT16VHV1dUFniaqrq+X1ep0x69evD9rf8bvQjo85UWJiohITE8M8CwAAEKti+gyRMUYTJ07UW2+9pTVr1igjIyOof9CgQWrfvr1KS0udtsrKSlVVVSkrK0uSlJWVpe3bt6umpsYZU1JSIrfbrf79+0dmIgAAIKbF9BmiwsJCLV26VL///e/VuXNn55qf5ORkJSUlKTk5WQUFBZoyZYq6du0qt9ute+65R1lZWbrqqqskScOHD1f//v116623au7cufL5fHr00UdVWFjIWSAAACApxgPRggULJEn/9m//FtS+cOFC3X777ZKk3/zmN4qLi9Po0aPV2NionJwcPf/8887Ydu3aaeXKlbrrrruUlZWlTp06KT8/X7/85S8jNQ0AABDj2tRziKKF5xAhWngOEQCE7ox9DhEAAEBrIBABAADrEYgAAID1CEQAAMB6BCIAAGA9AhEAALBeTD+HCLBdW3wkA48KANAWcYYIAABYj0AEAACsRyACAADWIxABAADrEYgAAID1CEQAAMB6BCIAAGA9AhEAALAegQgAAFiPQAQAAKxHIAIAANYjEAEAAOsRiAAAgPUIRAAAwHoEIgAAYD0CEQAAsB6BCAAAWI9ABAAArEcgAgAA1iMQAQAA6xGIAACA9QhEAADAegQiAABgPQIRAACwHoEIAABYLz7aBQA4s/Se+m60SzhtX8zOjXYJAKKMM0QAAMB6BCIAAGA9AhEAALAegQgAAFiPQAQAAKxHIAIAANYjEAEAAOvxHCIA1uPZSQA4QwQAAKxHIAIAANYjEAEAAOsRiAAAgPUIRAAAwHoEIgAAYD1uuweANqgtPipA4nEBiF2cIQIAANYjEAEAAOsRiAAAgPW4hggAEDFt8donrnuyA4EIAIDv0RZDXFsU7eBp1Vdmzz33nHr37q0OHTpo8ODBWr9+fbRLAgAAMcCaQPT6669rypQpeuyxx7Rp0yZdcsklysnJUU1NTbRLAwAAUWZNIJo3b57Gjx+vcePGqX///iouLlbHjh318ssvR7s0AAAQZVZcQ3T06FFVVFRo2rRpTltcXJyys7NVVlbWYnxjY6MaGxud1/X19ZIkv9/fKvUFGr9plf0CANBWtMZn7PF9GmP+6VgrAtHf/vY3NTc3y+PxBLV7PB59+umnLcYXFRXp8ccfb9Genp7eajUCAGCz5Kdbb9+HDh1ScnLy946xIhCdrmnTpmnKlCnO60AgoNraWnXr1k0ulytsx/H7/UpPT9fevXvldrvDtl+0xFpHDmsdOax15LDWkRWu9TbG6NChQ0pLS/unY60IRN27d1e7du1UXV0d1F5dXS2v19tifGJiohITE4PaUlJSWq0+t9vNP7AIYa0jh7WOHNY6cljryArHev+zM0PHWXFRdUJCggYNGqTS0lKnLRAIqLS0VFlZWVGsDAAAxAIrzhBJ0pQpU5Sfn6/MzExdeeWVevrpp3X48GGNGzcu2qUBAIAosyYQ/fSnP9XBgwc1Y8YM+Xw+XXrppVq9enWLC60jKTExUY899liLr+cQfqx15LDWkcNaRw5rHVnRWG+XOZV70QAAAM5gVlxDBAAA8H0IRAAAwHoEIgAAYD0CEQAAsB6BKIqee+459e7dWx06dNDgwYO1fv36aJfUphQVFemKK65Q586dlZqaqptuukmVlZVBY44cOaLCwkJ169ZNZ511lkaPHt3iAZ1VVVXKzc1Vx44dlZqaqgcffFDHjh2L5FTanNmzZ8vlcmny5MlOG2sdPl999ZXGjh2rbt26KSkpSQMHDtTGjRudfmOMZsyYoR49eigpKUnZ2dnas2dP0D5qa2uVl5cnt9utlJQUFRQUqKGhIdJTiWnNzc2aPn26MjIylJSUpPPOO08zZ84M+t0r1jp069at0w033KC0tDS5XC6tWLEiqD9ca7tt2zZdc8016tChg9LT0zV37tzQCjaIimXLlpmEhATz8ssvm507d5rx48eblJQUU11dHe3S2oycnByzcOFCs2PHDrNlyxYzcuRI07NnT9PQ0OCMufPOO016eropLS01GzduNFdddZW5+uqrnf5jx46ZAQMGmOzsbLN582bzhz/8wXTv3t1MmzYtGlNqE9avX2969+5tLr74YjNp0iSnnbUOj9raWtOrVy9z++23m/LycvPZZ5+Z9957z/zlL39xxsyePdskJyebFStWmK1bt5r/+I//MBkZGeYf//iHM2bEiBHmkksuMR9//LH505/+ZM4//3xzyy23RGNKMWvWrFmmW7duZuXKlebzzz83y5cvN2eddZZ55plnnDGsdej+8Ic/mEceecS8+eabRpJ56623gvrDsbb19fXG4/GYvLw8s2PHDvPaa6+ZpKQk88ILL5x2vQSiKLnyyitNYWGh87q5udmkpaWZoqKiKFbVttXU1BhJZu3atcYYY+rq6kz79u3N8uXLnTG7du0ykkxZWZkx5tt/sHFxccbn8zljFixYYNxut2lsbIzsBNqAQ4cOmT59+piSkhLzr//6r04gYq3D5+GHHzZDhw79//YHAgHj9XrNU0895bTV1dWZxMRE89prrxljjPnkk0+MJLNhwwZnzKpVq4zL5TJfffVV6xXfxuTm5po77rgjqG3UqFEmLy/PGMNah9OJgShca/v888+bLl26BP0f8vDDD5sLL7zwtGvkK7MoOHr0qCoqKpSdne20xcXFKTs7W2VlZVGsrG2rr6+XJHXt2lWSVFFRoaampqB17tu3r3r27Omsc1lZmQYOHBj0gM6cnBz5/X7t3LkzgtW3DYWFhcrNzQ1aU4m1Dqe3335bmZmZ+slPfqLU1FRddtll+t3vfuf0f/755/L5fEFrnZycrMGDBwetdUpKijIzM50x2dnZiouLU3l5eeQmE+OuvvpqlZaWavfu3ZKkrVu36sMPP9T1118vibVuTeFa27KyMl177bVKSEhwxuTk5KiyslJff/31adVkzZOqY8nf/vY3NTc3t3hKtsfj0aeffhqlqtq2QCCgyZMna8iQIRowYIAkyefzKSEhocUP83o8Hvl8PmfMyf4ejvfh/yxbtkybNm3Shg0bWvSx1uHz2WefacGCBZoyZYr++7//Wxs2bNC9996rhIQE5efnO2t1srX87lqnpqYG9cfHx6tr166s9XdMnTpVfr9fffv2Vbt27dTc3KxZs2YpLy9PkljrVhSutfX5fMrIyGixj+N9Xbp0OeWaCEQ4IxQWFmrHjh368MMPo13KGWnv3r2aNGmSSkpK1KFDh2iXc0YLBALKzMzUk08+KUm67LLLtGPHDhUXFys/Pz/K1Z1Z3njjDS1ZskRLly7VRRddpC1btmjy5MlKS0tjrS3EV2ZR0L17d7Vr167FHTjV1dXyer1RqqrtmjhxolauXKkPPvhA5557rtPu9Xp19OhR1dXVBY3/7jp7vd6T/j0c78O3KioqVFNTo8svv1zx8fGKj4/X2rVrNX/+fMXHx8vj8bDWYdKjRw/1798/qK1fv36qqqqS9H9r9X3/f3i9XtXU1AT1Hzt2TLW1taz1dzz44IOaOnWqxowZo4EDB+rWW2/Vfffdp6KiIkmsdWsK19qG8/8VAlEUJCQkaNCgQSotLXXaAoGASktLlZWVFcXK2hZjjCZOnKi33npLa9asaXHadNCgQWrfvn3QOldWVqqqqspZ56ysLG3fvj3oH11JSYncbneLDyWbDRs2TNu3b9eWLVucLTMzU3l5ec6fWevwGDJkSIvHR+zevVu9evWSJGVkZMjr9Qattd/vV3l5edBa19XVqaKiwhmzZs0aBQIBDR48OAKzaBu++eYbxcUFfwy2a9dOgUBAEmvdmsK1tllZWVq3bp2ampqcMSUlJbrwwgtP6+sySdx2Hy3Lli0ziYmJZtGiReaTTz4xEyZMMCkpKUF34OD73XXXXSY5Odn87//+rzlw4ICzffPNN86YO++80/Ts2dOsWbPGbNy40WRlZZmsrCyn//it4MOHDzdbtmwxq1evNmeffTa3gp+C795lZgxrHS7r16838fHxZtasWWbPnj1myZIlpmPHjubVV191xsyePdukpKSY3//+92bbtm3mxhtvPOntypdddpkpLy83H374oenTpw+3gp8gPz/fnHPOOc5t92+++abp3r27eeihh5wxrHXoDh06ZDZv3mw2b95sJJl58+aZzZs3my+//NIYE561raurMx6Px9x6661mx44dZtmyZaZjx47cdt/WPPvss6Znz54mISHBXHnllebjjz+OdkltiqSTbgsXLnTG/OMf/zB333236dKli+nYsaO5+eabzYEDB4L288UXX5jrr7/eJCUlme7du5v777/fNDU1RXg2bc+JgYi1Dp933nnHDBgwwCQmJpq+ffuaF198Mag/EAiY6dOnG4/HYxITE82wYcNMZWVl0Ji///3v5pZbbjFnnXWWcbvdZty4cebQoUORnEbM8/v9ZtKkSaZnz56mQ4cO5l/+5V/MI488EnQLN2sdug8++OCk/0fn5+cbY8K3tlu3bjVDhw41iYmJ5pxzzjGzZ88OqV6XMd95JCcAAICFuIYIAABYj0AEAACsRyACAADWIxABAADrEYgAAID1CEQAAMB6BCIAAGA9AhEAALAegQgAAFiPQAQAAKxHIAIAANYjEAEAAOv9P+30NKPWZQ84AAAAAElFTkSuQmCC)











Same result using query:










In [ ]:



```
ted.query('comments<1000 ').comments.plot(kind='hist')

```










Out[ ]:


```
<Axes: ylabel='Frequency'>
```






![](data:image/png;base64,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hBSI7r//fj3zzDMyxoS7nha++uorjR07Vt26dXPuZtu4caPTb4zRjBkz1KNHDyUlJSk7O7vFj8/W1tYqLy9PbrdbKSkpKigoUENDQ6vXDgAA2oaQvjL78MMP9cEHH2jVqlW66KKL1L59+6D+N998MyzFff311xoyZIiuu+46rVq1Smeffbb27NmjLl26OGPmzp2r+fPna/HixcrIyND06dOVk5OjTz75RB06dJAk5eXl6cCBAyopKVFTU5PGjRunCRMmaOnSpWGpEwAAtG0hBaKUlBTdfPPN4a6lhTlz5ig9PV0LFy502r77G2rGGD399NN69NFHdeONN0qSXnnlFXk8Hq1YsUJjxozRrl27tHr1am3YsEGZmZmSpGeffVYjR47Ur371K6WlpbX6PAAAQGwLKRB9N6C0prfffls5OTn6yU9+orVr1+qcc87R3XffrfHjx0uSPv/8c/l8PmVnZzvvSU5O1uDBg1VWVqYxY8aorKxMKSkpThiSpOzsbMXFxam8vDwiwQ4AAMS2kK4hkqRjx47pj3/8o1544QUdOnRIkrR///6wXpvz2WefacGCBerTp4/ee+893XXXXbr33nu1ePFiSZLP55MkeTyeoPd5PB6nz+fzKTU1Nag/Pj5eXbt2dcacqLGxUX6/P2gDAABnrpDOEH355ZcaMWKEqqqq1NjYqH//939X586dNWfOHDU2Nqq4uDgsxQUCAWVmZjq/j3bZZZdpx44dKi4uVn5+fliOcTJFRUV6/PHHW23/AAAgtoR0hmjSpEnKzMzU119/raSkJKf95ptvVmlpadiK69Gjh/r37x/U1q9fP1VVVUmSvF6vJKm6ujpoTHV1tdPn9XpVU1MT1H/s2DHV1tY6Y040bdo01dfXO9vevXvDMh8AABCbQgpEf/rTn/Too48qISEhqL1379766quvwlKYJA0ZMkSVlZVBbbt373Z+RDYjI0NerzcohPn9fpWXlysrK0uSlJWVpbq6OlVUVDhj1qxZo0AgoMGDB5/0uImJiXK73UEbAAA4c4X0lVkgEFBzc3OL9n379qlz584/uKjj7rvvPl199dV68skn9V//9V9av369XnzxRb344ouSJJfLpcmTJ+uJJ55Qnz59nNvu09LSdNNNN0n69ozSiBEjNH78eBUXF6upqUkTJ07UmDFjuMMMAABICvEM0fDhw/X00087r10ulxoaGvTYY4+F9ec8rrjiCr311lt67bXXNGDAAM2cOVNPP/208vLynDEPPfSQ7rnnHk2YMEFXXHGFGhoatHr1aucZRJK0ZMkS9e3bV8OGDdPIkSM1dOhQJ1QBAAC4TAiPm963b59ycnJkjNGePXuUmZmpPXv2qHv37lq3bl2Lu7raOr/fr+TkZNXX17fK12e9p74b9n2ipS9m50a7BABABJ3O53dIX5mde+652rp1q5YtW6Zt27apoaFBBQUFysvLC7rIGgAAoC0IKRBJ3z7LZ+zYseGsBQAAICpCCkSvvPLK9/bfdtttIRUDAAAQDSEFokmTJgW9bmpq0jfffKOEhAR17NiRQAQAANqUkO4y+/rrr4O2hoYGVVZWaujQoXrttdfCXSMAAECrCvm3zE7Up08fzZ49u8XZIwAAgFgXtkAkfXuh9f79+8O5SwAAgFYX0jVEb7/9dtBrY4wOHDig3/72txoyZEhYCgMAAIiUkALR8Z/FOM7lcunss8/Wj370I/36178OR10AAAARE/JvmQEAAJwpwnoNEQAAQFsU0hmiKVOmnPLYefPmhXIIAACAiAkpEG3evFmbN29WU1OTLrzwQknS7t271a5dO11++eXOOJfLFZ4qAQAAWlFIgeiGG25Q586dtXjxYnXp0kXStw9rHDdunK655hrdf//9YS0SAACgNYV0DdGvf/1rFRUVOWFIkrp06aInnniCu8wAAECbE1Ig8vv9OnjwYIv2gwcP6tChQz+4KAAAgEgKKRDdfPPNGjdunN58803t27dP+/bt0//8z/+ooKBAo0aNCneNAAAArSqka4iKi4v1wAMP6Gc/+5mampq+3VF8vAoKCvTUU0+FtUAAAIDWFlIg6tixo55//nk99dRT+utf/ypJOu+889SpU6ewFgcAABAJP+jBjAcOHNCBAwfUp08fderUScaYcNUFAAAQMSEFor///e8aNmyYLrjgAo0cOVIHDhyQJBUUFHDLPQAAaHNCCkT33Xef2rdvr6qqKnXs2NFp/+lPf6rVq1eHrTgAAIBICOkaovfff1/vvfeezj333KD2Pn366MsvvwxLYQAAAJES0hmiw4cPB50ZOq62tlaJiYk/uCgAAIBICikQXXPNNXrllVec1y6XS4FAQHPnztV1110XtuIAAAAiIaSvzObOnathw4Zp48aNOnr0qB566CHt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PkN0ovr6eklS165dJUkVFRVqampSdna2M6Zv377q2bOnysrKJEllZWUaOHCgE4YkKScnR36/Xzt37jzpcRobG+X3+4M2AABw5mozgSgQCGjy5MkaMmSIBgwYIEny+XxKSEhQSkpK0FiPxyOfz+eM+W4YOt5/vO9kioqKlJyc7Gzp6elhng0AAIglbSYQFRYWaseOHVq2bFmrH2vatGmqr693tr1797b6MQEAQPTER7uAUzFx4kStXLlS69at07nnnuu0e71eHT16VHV1dUFniaqrq+X1ep0x69evD9rf8bvQjo85UWJiohITE8M8CwAAEKti+gyRMUYTJ07UW2+9pTVr1igjIyOof9CgQWrfvr1KS0udtsrKSlVVVSkrK0uSlJWVpe3bt6umpsYZU1JSIrfbrf79+0dmIgAAIKbF9BmiwsJCLV26VL///e/VuXNn55qf5ORkJSUlKTk5WQUFBZoyZYq6du0qt9ute+65R1lZWbrqqqskScOHD1f//v116623au7cufL5fHr00UdVWFjIWSAAACApxgPRggULJEn/9m//FtS+cOFC3X777ZKk3/zmN4qLi9Po0aPV2NionJwcPf/8887Ydu3aaeXKlbrrrruUlZWlTp06KT8/X7/85S8jNQ0AABDj2tRziKKF5xAhWngOEQCE7ox9DhEAAEBrIBABAADrEYgAAID1CEQAAMB6BCIAAGA9AhEAALBeTD+HCLBdW3wkA48KANAWcYYIAABYj0AEAACsRyACAADWIxABAADrEYgAAID1CEQAAMB6BCIAAGA9AhEAALAegQgAAFiPQAQAAKxHIAIAANYjEAEAAOsRiAAAgPUIRAAAwHoEIgAAYD0CEQAAsB6BCAAAWI9ABAAArEcgAgAA1iMQAQAA6xGIAACA9QhEAADAegQiAABgPQIRAACwHoEIAABYLz7aBQA4s/Se+m60SzhtX8zOjXYJAKKMM0QAAMB6BCIAAGA9AhEAALAegQgAAFiPQAQAAKxHIAIAANYjEAEAAOvxHCIA1uPZSQA4QwQAAKxHIAIAANYjEAEAAOsRiAAAgPUIRAAAwHoEIgAAYD1uuweANqgtPipA4nEBiF2cIQIAANYjEAEAAOsRiAAAgPW4hggAEDFt8donrnuyA4EIAIDv0RZDXFsU7eBp1Vdmzz33nHr37q0OHTpo8ODBWr9+fbRL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rS3EV2ZR0L17d7Vr167FHTjV1dXyer1RqqrtmjhxolauXKkPPvhA5557rtPu9Xp19OhR1dXVBY3/7jp7vd6T/j0c78O3KioqVFNTo8svv1zx8fGKj4/X2rVrNX/+fMXHx8vj8bDWYdKjRw/1798/qK1fv36qqqqS9H9r9X3/f3i9XtXU1AT1Hzt2TLW1taz1dzz44IOaOnWqxowZo4EDB+rWW2/Vfffdp6KiIkmsdWsK19qG8/8VAlEUJCQkaNCgQSotLXXaAoGASktLlZWVFcXK2hZjjCZOnKi33npLa9asaXHadNCgQWrfvn3QOldWVqqqqspZ56ysLG3fvj3oH11JSYncbneLDyWbDRs2TNu3b9eWLVucLTMzU3l5ec6fWevwGDJkSIvHR+zevVu9evWSJGVkZMjr9Qattd/vV3l5edBa19XVqaKiwhmzZs0aBQIBDR48OAKzaBu++eYbxcUFfwy2a9dOgUBAEmvdmsK1tllZWVq3bp2ampqcMSUlJbrwwgtP6+sySdx2Hy3Lli0ziYmJZtGiReaTTz4xEyZMMCkpKUF34OD73XXXXSY5Odn87//+rzlw4ICzffPNN86YO++80/Ts2dOsWbPGbNy40WRlZZmsrCyn//it4MOHDzdbtmwxq1evNmeffTa3gp+C795lZgxrHS7r16838fHxZtasWWbPnj1myZIlpmPHjubVV191xsyePdukpKSY3//+92bbtm3mxhtvPOntypdddpkpLy83H374oenTpw+3gp8gPz/fnHPOOc5t92+++abp3r27eeihh5wxrHXoDh06ZDZv3mw2b95sJJl58+aZzZs3my+//NIYE561raurMx6Px9x6661mx44dZtmyZaZjx47cdt/WPPvss6Znz54mISHBXHnllebjjz+OdkltiqSTbgsXLnTG/OMf/zB333236dKli+nYsaO5+eabzYEDB4L288UXX5jrr7/eJCUlme7du5v777/fNDU1RXg2bc+JgYi1Dp933nnHDBgwwCQmJpq+ffuaF198Mag/EAiY6dOnG4/HYxITE82wYcNMZWVl0Ji///3v5pZbbjFnnXWWcbvdZty4cebQoUORnEbM8/v9ZtKkSaZnz56mQ4cO5l/+5V/MI488EnQLN2sdug8++OCk/0fn5+cbY8K3tlu3bjVDhw41iYmJ5pxzzjGzZ88OqV6XMd95JCcAAICFuIYIAABYj0AEAACsRyACAADWIxABAADrEYgAAID1CEQAAMB6BCIAAGA9AhEAALAegQgAAFiPQAQAAKxHIAIAANYjEAEAAOv9P+30NKPWZQ84AAAAAElFTkSuQmCC)











Same result but using loc:










In [ ]:



```
ted.loc[ ted.comments<1000,'comments' ].plot(kind='hist')

```










Out[ ]:


```
<Axes: ylabel='Frequency'>
```






![](data:image/png;base64,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hBSI7r//fj3zzDMyxoS7nha++uorjR07Vt26dXPuZtu4caPTb4zRjBkz1KNHDyUlJSk7O7vFj8/W1tYqLy9PbrdbKSkpKigoUENDQ6vXDgAA2oaQvjL78MMP9cEHH2jVqlW66KKL1L59+6D+N998MyzFff311xoyZIiuu+46rVq1Smeffbb27NmjLl26OGPmzp2r+fPna/HixcrIyND06dOVk5OjTz75RB06dJAk5eXl6cCBAyopKVFTU5PGjRunCRMmaOnSpWGpEwAAtG0hBaKUlBTdfPPN4a6lhTlz5ig9PV0LFy502r77G2rGGD399NN69NFHdeONN0qSXnnlFXk8Hq1YsUJjxozRrl27tHr1am3YsEGZmZmSpGeffVYjR47Ur371K6WlpbX6PAAAQGwLKRB9N6C0prfffls5OTn6yU9+orVr1+qcc87R3XffrfHjx0uSPv/8c/l8PmVnZzvvSU5O1uDBg1VWVqYxY8aorKxMKSkpThiSpOzsbMXFxam8vDwiwQ4AAMS2kK4hkqRjx47pj3/8o1544QUdOnRIkrR///6wXpvz2WefacGCBerTp4/ee+893XXXXbr33nu1ePFiSZLP55MkeTyeoPd5PB6nz+fzKTU1Nag/Pj5eXbt2dcacqLGxUX6/P2gDAABnrpDOEH355ZcaMWKEqqqq1NjYqH//939X586dNWfOHDU2Nqq4uDgsxQUCAWVmZjq/j3bZZZdpx44dKi4uVn5+fliOcTJFRUV6/PHHW23/AAAgtoR0hmjSpEnKzMzU119/raSkJKf95ptvVmlpadiK69Gjh/r37x/U1q9fP1VVVUmSvF6vJKm6ujpoTHV1tdPn9XpVU1MT1H/s2DHV1tY6Y040bdo01dfXO9vevXvDMh8AABCbQgpEf/rTn/Too48qISEhqL1379766quvwlKYJA0ZMkSVlZVBbbt373Z+RDYjI0NerzcohPn9fpWXlysrK0uSlJWVpbq6OlVUVDhj1qxZo0AgoMGDB5/0uImJiXK73UEbAAA4c4X0lVkgEFBzc3OL9n379qlz584/uKjj7rvvPl199dV68skn9V//9V9av369XnzxRb344ouSJJfLpcmTJ+uJJ55Qnz59nNvu09LSdNNNN0n69ozSiBEjNH78eBUXF6upqUkTJ07UmDFjuMMMAABICvEM0fDhw/X00087r10ulxoaGvTYY4+F9ec8rrjiCr311lt67bXXNGDAAM2cOVNPP/208vLynDEPPfSQ7rnnHk2YMEFXXHGFGhoatHr1aucZRJK0ZMkS9e3bV8OGDdPIkSM1dOhQJ1QBAAC4TAiPm963b59ycnJkjNGePXuUmZmpPXv2qHv37lq3bl2Lu7raOr/fr+TkZNXX17fK12e9p74b9n2ipS9m50a7BABABJ3O53dIX5mde+652rp1q5YtW6Zt27apoaFBBQUFysvLC7rIGgAAoC0IKRBJ3z7LZ+zYseGsBQAAICpCCkSvvPLK9/bfdtttIRUDAAAQDSEFokmTJgW9bmpq0jfffKOEhAR17NiRQAQAANqUkO4y+/rrr4O2hoYGVVZWaujQoXrttdfCXSMAAECrCvm3zE7Up08fzZ49u8XZIwAAgFgXtkAkfXuh9f79+8O5SwAAgFYX0jVEb7/9dtBrY4wOHDig3/72txoyZEhYCgMAAIiUkALR8Z/FOM7lcunss8/Wj370I/36178OR10AAAARE/JvmQEAAJwpwnoNEQAAQFsU0hmiKVOmnPLYefPmhXIIAACAiAkpEG3evFmbN29WU1OTLrzwQknS7t271a5dO11++eXOOJfLFZ4qAQAAWlFIgeiGG25Q586dtXjxYnXp0kXStw9rHDdunK655hrdf//9YS0SAACgNYV0DdGvf/1rFRUVOWFIkrp06aInnniCu8wAAECbE1Ig8vv9OnjwYIv2gwcP6tChQz+4KAAAgEgKKRDdfPPNGjdunN58803t27dP+/bt0//8z/+ooKBAo0aNCneNAAAArSqka4iKi4v1wAMP6Gc/+5mampq+3VF8vAoKCvTUU0+FtUAAAIDWFlIg6tixo55//nk99dRT+utf/ypJOu+889SpU6ewFgcAABAJP+jBjAcOHNCBAwfUp08fderUScaYcNUFAAAQMSEFor///e8aNmyYLrjgAo0cOVIHDhyQJBUUFHDLPQAAaHNCCkT33Xef2rdvr6qqKnXs2NFp/+lPf6rVq1eHrTgAAIBICOkaovfff1/vvfeezj333KD2Pn366MsvvwxLYQAAAJES0hmiw4cPB50ZOq62tlaJiYk/uCgAAIBICikQXXPNNXrllVec1y6XS4FAQHPnztV1110XtuIAAAAiIaSvzObOnathw4Zp48aNOnr0qB566CHt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PkN0ovr6eklS165dJUkVFRVqampSdna2M6Zv377q2bOnysrKJEllZWUaOHCgE4YkKScnR36/Xzt37jzpcRobG+X3+4M2AABw5mozgSgQCGjy5MkaMmSIBgwYIEny+XxKSEhQSkpK0FiPxyOfz+eM+W4YOt5/vO9kioqKlJyc7Gzp6elhng0AAIglbSYQFRYWaseOHVq2bFmrH2vatGmqr693tr1797b6MQEAQPTER7uAUzFx4kStXLlS69at07nnnuu0e71eHT16VHV1dUFniaqrq+X1ep0x69evD9rf8bvQjo85UWJiohITE8M8CwAAEKti+gyRMUYTJ07UW2+9pTVr1igjIyOof9CgQWrfvr1KS0udtsrKSlVVVSkrK0uSlJWVpe3bt6umpsYZU1JSIrfbrf79+0dmIgAAIKbF9BmiwsJCLV26VL///e/VuXNn55qf5ORkJSUlKTk5WQUFBZoyZYq6du0qt9ute+65R1lZWbrqqqskScOHD1f//v116623au7cufL5fHr00UdVWFjIWSAAACApxgPRggULJEn/9m//FtS+cOFC3X777ZKk3/zmN4qLi9Po0aPV2NionJwcPf/8887Ydu3aaeXKlbrrrruUlZWlTp06KT8/X7/85S8jNQ0AABDj2tRziKKF5xAhWngOEQCE7ox9DhEAAEBrIBABAADrEYgAAID1CEQAAMB6BCIAAGA9AhEAALBeTD+HCLBdW3wkA48KANAWcYYIAABYj0AEAACsRyACAADWIxABAADrEYgAAID1CEQAAMB6BCIAAGA9AhEAALAegQgAAFiPQAQAAKxHIAIAANYjEAEAAOsRiAAAgPUIRAAAwHoEIgAAYD0CEQAAsB6BCAAAWI9ABAAArEcgAgAA1iMQAQAA6xGIAACA9QhEAADAegQiAABgPQIRAACwHoEIAABYLz7aBQA4s/Se+m60SzhtX8zOjXYJAKKMM0QAAMB6BCIAAGA9AhEAALAegQgAAFiPQAQAAKxHIAIAANYjEAEAAOvxHCIA1uPZSQA4QwQAAKxHIAIAANYjEAEAAOsRiAAAgPUIRAAAwHoEIgAAYD1uuweANqgtPipA4nEBiF2cIQIAANYjEAEAAOsRiAAAgPW4hggAEDFt8donrnuyA4EIAIDv0RZDXFsU7eBp1Vdmzz33nHr37q0OHTpo8ODBWr9+fbRL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rS3EV2ZR0L17d7Vr167FHTjV1dXyer1RqqrtmjhxolauXKkPPvhA5557rtPu9Xp19OhR1dXVBY3/7jp7vd6T/j0c78O3KioqVFNTo8svv1zx8fGKj4/X2rVrNX/+fMXHx8vj8bDWYdKjRw/1798/qK1fv36qqqqS9H9r9X3/f3i9XtXU1AT1Hzt2TLW1taz1dzz44IOaOnWqxowZo4EDB+rWW2/Vfffdp6KiIkmsdWsK19qG8/8VAlEUJCQkaNCgQSotLXXaAoGASktLlZWVFcXK2hZjjCZOnKi33npLa9asaXHadNCgQWrfvn3QOldWVqqqqspZ56ysLG3fvj3oH11JSYncbneLDyWbDRs2TNu3b9eWLVucLTMzU3l5ec6fWevwGDJkSIvHR+zevVu9evWSJGVkZMjr9Qattd/vV3l5edBa19XVqaKiwhmzZs0aBQIBDR48OAKzaBu++eYbxcUFfwy2a9dOgUBAEmvdmsK1tllZWVq3bp2ampqcMSUlJbrwwgtP6+sySdx2Hy3Lli0ziYmJZtGiReaTTz4xEyZMMCkpKUF34OD73XXXXSY5Odn87//+rzlw4ICzffPNN86YO++80/Ts2dOsWbPGbNy40WRlZZmsrCyn//it4MOHDzdbtmwxq1evNmeffTa3gp+C795lZgxrHS7r16838fHxZtasWWbPnj1myZIlpmPHjubVV191xsyePdukpKSY3//+92bbtm3mxhtvPOntypdddpkpLy83H374oenTpw+3gp8gPz/fnHPOOc5t92+++abp3r27eeihh5wxrHXoDh06ZDZv3mw2b95sJJl58+aZzZs3my+//NIYE561raurMx6Px9x6661mx44dZtmyZaZjx47cdt/WPPvss6Znz54mISHBXHnllebjjz+OdkltiqSTbgsXLnTG/OMf/zB333236dKli+nYsaO5+eabzYEDB4L288UXX5jrr7/eJCUlme7du5v777/fNDU1RXg2bc+JgYi1Dp933nnHDBgwwCQmJpq+ffuaF198Mag/EAiY6dOnG4/HYxITE82wYcNMZWVl0Ji///3v5pZbbjFnnXWWcbvdZty4cebQoUORnEbM8/v9ZtKkSaZnz56mQ4cO5l/+5V/MI488EnQLN2sdug8++OCk/0fn5+cbY8K3tlu3bjVDhw41iYmJ5pxzzjGzZ88OqV6XMd95JCcAAICFuIYIAABYj0AEAACsRyACAADWIxABAADrEYgAAID1CEQAAMB6BCIAAGA9AhEAALAegQgAAFiPQAQAAKxHIAIAANYjEAEAAOv9P+30NKPWZQ84AAAAAElFTkSuQmCC)











Changing the number of bins:












## Plot the number of talks that took place each year[¶](#Plot-the-number-of-talks-that-took-place-each-year)










In [ ]:



```
ted.dtypes

```










Out[ ]:


```
comments                int64
description            object
duration                int64
event                  object
film_date               int64
languages               int64
main_speaker           object
name                   object
num_speaker             int64
published_date          int64
ratings                object
related_talks          object
speaker_occupation     object
tags                   object
title                  object
url                    object
views                   int64
comments_per_view     float64
views_per_comment     float64
dtype: object
```










In [ ]:



```
ted

```










Out[ ]:



 .dataframe tbody tr th:only-of-type {
 vertical-align: middle;
 }

 .dataframe tbody tr th {
 vertical-align: top;
 }

 .dataframe thead th {
 text-align: right;
 }



|  | comments | description | duration | event | film\_date | languages | main\_speaker | name | num\_speaker | published\_date | ratings | related\_talks | speaker\_occupation | tags | title | url | views | comments\_per\_view | views\_per\_comment |
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
| 0 | 4553 | Sir Ken Robinson makes an entertaining and pro... | 1164 | TED2006 | 1140825600 | 60 | Ken Robinson | Ken Robinson: Do schools kill creativity? | 1 | 1151367060 | [{'id': 7, 'name': 'Funny', 'count': 19645}, {... | [{'id': 865, 'hero': 'https://pe.tedcdn.com/im... | Author/educator | ['children', 'creativity', 'culture', 'dance',... | Do schools kill creativity? | https://www.ted.com/talks/ken\_robinson\_says\_sc... | 47227110 | 0.000096 | 10372.745443 |
| 1 | 265 | With the same humor and humanity he exuded in ... | 977 | TED2006 | 1140825600 | 43 | Al Gore | Al Gore: Averting the climate crisis | 1 | 1151367060 | [{'id': 7, 'name': 'Funny', 'count': 544}, {'i... | [{'id': 243, 'hero': 'https://pe.tedcdn.com/im... | Climate advocate | ['alternative energy', 'cars', 'climate change... | Averting the climate crisis | https://www.ted.com/talks/al\_gore\_on\_averting\_... | 3200520 | 0.000083 | 12077.433962 |
| 2 | 124 | New York Times columnist David Pogue takes aim... | 1286 | TED2006 | 1140739200 | 26 | David Pogue | David Pogue: Simplicity sells | 1 | 1151367060 | [{'id': 7, 'name': 'Funny', 'count': 964}, {'i... | [{'id': 1725, 'hero': 'https://pe.tedcdn.com/i... | Technology columnist | ['computers', 'entertainment', 'interface desi... | Simplicity sells | https://www.ted.com/talks/david\_pogue\_says\_sim... | 1636292 | 0.000076 | 13195.903226 |
| 3 | 200 | In an emotionally charged talk, MacArthur-winn... | 1116 | TED2006 | 1140912000 | 35 | Majora Carter | Majora Carter: Greening the ghetto | 1 | 1151367060 | [{'id': 3, 'name': 'Courageous', 'count': 760}... | [{'id': 1041, 'hero': 'https://pe.tedcdn.com/i... | Activist for environmental justice | ['MacArthur grant', 'activism', 'business', 'c... | Greening the ghetto | https://www.ted.com/talks/majora\_carter\_s\_tale... | 1697550 | 0.000118 | 8487.750000 |
| 4 | 593 | You've never seen data presented like this. Wi... | 1190 | TED2006 | 1140566400 | 48 | Hans Rosling | Hans Rosling: The best stats you've ever seen | 1 | 1151440680 | [{'id': 9, 'name': 'Ingenious', 'count': 3202}... | [{'id': 2056, 'hero': 'https://pe.tedcdn.com/i... | Global health expert; data visionary | ['Africa', 'Asia', 'Google', 'demo', 'economic... | The best stats you've ever seen | https://www.ted.com/talks/hans\_rosling\_shows\_t... | 12005869 | 0.000049 | 20245.984823 |
| ... | ... | ... | ... | ... | ... | ... | ... | ... | ... | ... | ... | ... | ... | ... | ... | ... | ... | ... | ... |
| 2545 | 17 | Between 2008 and 2016, the United States depor... | 476 | TED2017 | 1496707200 | 4 | Duarte Geraldino | Duarte Geraldino: What we're missing in the de... | 1 | 1505851216 | [{'id': 3, 'name': 'Courageous', 'count': 24},... | [{'id': 2596, 'hero': 'https://pe.tedcdn.com/i... | Journalist | ['TED Residency', 'United States', 'community'... | What we're missing in the debate about immigra... | https://www.ted.com/talks/duarte\_geraldino\_wha... | 450430 | 0.000038 | 26495.882353 |
| 2546 | 6 | How can you study Mars without a spaceship? He... | 290 | TED2017 | 1492992000 | 3 | Armando Azua-Bustos | Armando Azua-Bustos: The most Martian place on... | 1 | 1505919737 | [{'id': 22, 'name': 'Fascinating', 'count': 32... | [{'id': 2491, 'hero': 'https://pe.tedcdn.com/i... | Astrobiologist | ['Mars', 'South America', 'TED Fellows', 'astr... | The most Martian place on Earth | https://www.ted.com/talks/armando\_azua\_bustos\_... | 417470 | 0.000014 | 69578.333333 |
| 2547 | 10 | Science fiction visions of the future show us ... | 651 | TED2017 | 1492992000 | 1 | Radhika Nagpal | Radhika Nagpal: What intelligent machines can ... | 1 | 1506006095 | [{'id': 1, 'name': 'Beautiful', 'count': 14}, ... | [{'id': 2346, 'hero': 'https://pe.tedcdn.com/i... | Robotics engineer | ['AI', 'ants', 'fish', 'future', 'innovation',... | What intelligent machines can learn from a sch... | https://www.ted.com/talks/radhika\_nagpal\_what\_... | 375647 | 0.000027 | 37564.700000 |
| 2548 | 32 | In an unmissable talk about race and politics ... | 1100 | TEDxMileHigh | 1499472000 | 1 | Theo E.J. Wilson | Theo E.J. Wilson: A black man goes undercover ... | 1 | 1506024042 | [{'id': 11, 'name': 'Longwinded', 'count': 3},... | [{'id': 2512, 'hero': 'https://pe.tedcdn.com/i... | Public intellectual | ['Internet', 'TEDx', 'United States', 'communi... | A black man goes undercover in the alt-right | https://www.ted.com/talks/theo\_e\_j\_wilson\_a\_bl... | 419309 | 0.000076 | 13103.406250 |
| 2549 | 8 | With more than half of the world population li... | 519 | TED2017 | 1492992000 | 1 | Karoliina Korppoo | Karoliina Korppoo: How a video game might help... | 1 | 1506092422 | [{'id': 21, 'name': 'Unconvincing', 'count': 2... | [{'id': 2682, 'hero': 'https://pe.tedcdn.com/i... | Game designer | ['cities', 'design', 'future', 'infrastructure... | How a video game might help us build better ci... | https://www.ted.com/talks/karoliina\_korppoo\_ho... | 391721 | 0.000020 | 48965.125000 |


2550 rows × 19 columns














## Displaying by column[¶](#Displaying-by-column)










In [ ]:



```
ted.published\_date

```










Out[ ]:


```
0       1151367060
1       1151367060
2       1151367060
3       1151367060
4       1151440680
           ...    
2545    1505851216
2546    1505919737
2547    1506006095
2548    1506024042
2549    1506092422
Name: published_date, Length: 2550, dtype: int64
```












1. Showing a sample of 30 elements of the column "event" to check if it contains the year










In [ ]:



```
ted.event.sample(30)

```










Out[ ]:


```
493                     TED2009
1556             TEDGlobal 2013
929                 TEDxCaltech
292                     TED2002
1150             TEDGlobal 2011
2126       TEDxAmoskeagMillyard
768                  TED@Cannes
752         Mission Blue Voyage
307                     TED2006
510              TEDGlobal 2009
2435             TEDxSanQuentin
819                 TEDxMidwest
2105              TEDWomen 2015
84                      TED2005
129              TEDGlobal 2007
170                     TED2007
218              TEDGlobal 2007
912                     TED2011
2022            TEDGlobalLondon
1746             TEDActive 2014
1818       TEDSalon Berlin 2014
1309             TEDGlobal 2012
1883           TEDxBeaconStreet
1492                    TED2013
1245                 TEDxSummit
932                     TED2011
2015                    TED2015
911            TEDxToronto 2010
1902    TED@State Street London
1069           TEDxBoulder 2011
Name: event, dtype: object
```












Unfortunately the date is not in date format, but as a timestamp, we require converting to date.










In [ ]:



```
ted.film\_date

```










Out[ ]:


```
0       1140825600
1       1140825600
2       1140739200
3       1140912000
4       1140566400
           ...    
2545    1496707200
2546    1492992000
2547    1492992000
2548    1499472000
2549    1492992000
Name: film_date, Length: 2550, dtype: int64
```












## Using datetime transformations[¶](#Using-datetime-transformations)










In [ ]:



```
pd.to\_datetime(ted.published\_date)

```










Out[ ]:


```
0      1970-01-01 00:00:01.151367060
1      1970-01-01 00:00:01.151367060
2      1970-01-01 00:00:01.151367060
3      1970-01-01 00:00:01.151367060
4      1970-01-01 00:00:01.151440680
                    ...             
2545   1970-01-01 00:00:01.505851216
2546   1970-01-01 00:00:01.505919737
2547   1970-01-01 00:00:01.506006095
2548   1970-01-01 00:00:01.506024042
2549   1970-01-01 00:00:01.506092422
Name: published_date, Length: 2550, dtype: datetime64[ns]
```










In [ ]:



```
pd.to\_datetime(ted.published\_date, unit='s')

```










Out[ ]:


```
0      2006-06-27 00:11:00
1      2006-06-27 00:11:00
2      2006-06-27 00:11:00
3      2006-06-27 00:11:00
4      2006-06-27 20:38:00
               ...        
2545   2017-09-19 20:00:16
2546   2017-09-20 15:02:17
2547   2017-09-21 15:01:35
2548   2017-09-21 20:00:42
2549   2017-09-22 15:00:22
Name: published_date, Length: 2550, dtype: datetime64[ns]
```












The unit parameter is crucial for the conversion to be correct.










In [ ]:



```
ted['film\_datetime']= pd.to\_datetime(ted.published\_date, unit='s')

```












Reviewing that the data makes sense comparing with event name










In [ ]:



```
ted.film\_datetime

```










Out[ ]:


```
0      2006-06-27 00:11:00
1      2006-06-27 00:11:00
2      2006-06-27 00:11:00
3      2006-06-27 00:11:00
4      2006-06-27 20:38:00
               ...        
2545   2017-09-19 20:00:16
2546   2017-09-20 15:02:17
2547   2017-09-21 15:01:35
2548   2017-09-21 20:00:42
2549   2017-09-22 15:00:22
Name: film_datetime, Length: 2550, dtype: datetime64[ns]
```










In [ ]:



```
ted[['event','film\_datetime']].sample(25)

```










Out[ ]:



 .dataframe tbody tr th:only-of-type {
 vertical-align: middle;
 }

 .dataframe tbody tr th {
 vertical-align: top;
 }

 .dataframe thead th {
 text-align: right;
 }



|  | event | film\_datetime |
| --- | --- | --- |
| 1693 | TED Fellows Retreat 2013 | 2014-03-06 16:01:23 |
| 1985 | TED2015 | 2015-05-28 15:21:08 |
| 1136 | TEDxCanberra | 2012-02-07 16:08:24 |
| 283 | TED2008 | 2008-09-02 01:00:00 |
| 1784 | TEDGlobal 2013 | 2014-07-09 14:51:35 |
| 94 | TED2003 | 2007-04-14 21:40:00 |
| 1551 | TEDxCERN | 2013-07-22 15:12:18 |
| 1314 | TEDxHousesOfParliament | 2012-08-12 15:13:23 |
| 250 | TED2008 | 2008-06-30 10:52:00 |
| 2122 | TEDWomen 2015 | 2016-01-21 15:49:36 |
| 2246 | TEDSummit | 2016-07-13 15:00:19 |
| 2182 | TED2015 | 2016-04-12 14:41:40 |
| 2036 | TEDGlobal 2014 | 2015-08-31 14:57:59 |
| 697 | TEDxNYED | 2010-05-31 11:13:00 |
| 529 | TEDxUSC | 2009-10-06 01:00:00 |
| 1994 | TED2015 | 2015-06-11 15:37:45 |
| 2044 | TED2015 | 2015-09-14 15:32:00 |
| 943 | TED2011 | 2011-05-24 14:54:00 |
| 1471 | TED2013 | 2013-04-04 14:56:21 |
| 2178 | TED2016 | 2016-04-07 15:03:12 |
| 1623 | TEDCity2.0 | 2013-11-13 15:59:49 |
| 2155 | TEDGlobal>Geneva | 2016-03-08 16:05:54 |
| 2543 | TED2017 | 2017-09-18 15:14:47 |
| 2506 | TEDxMileHigh | 2017-08-10 14:37:43 |
| 2113 | TEDxMarin | 2016-01-07 16:40:18 |














Some of the records don't match exactly, however the most part do. We take it as we have the right info for the film date.










In [ ]:



```
ted.dtypes

```










Out[ ]:


```
comments                       int64
description                   object
duration                       int64
event                         object
film_date                      int64
languages                      int64
main_speaker                  object
name                          object
num_speaker                    int64
published_date                 int64
ratings                       object
related_talks                 object
speaker_occupation            object
tags                          object
title                         object
url                           object
views                          int64
comments_per_view            float64
views_per_comment            float64
film_datetime         datetime64[ns]
dtype: object
```












film\_datetime has datetime64[ns] . This allows us to use a namespace "dt" with Pandas. For example:










In [ ]:



```
ted.film\_datetime.dt.year

```










Out[ ]:


```
0       2006
1       2006
2       2006
3       2006
4       2006
        ... 
2545    2017
2546    2017
2547    2017
2548    2017
2549    2017
Name: film_datetime, Length: 2550, dtype: int32
```












From that point on, we can use agregations like "value\_counts()". Below a sentence that can bring the year and the number of values that contain that year on the dataset.










In [ ]:



```
ted.film\_datetime.dt.year.value\_counts()

```










Out[ ]:


```
film_datetime
2012    306
2011    261
2010    257
2013    244
2016    243
2014    240
2009    222
2015    220
2017    197
2008    188
2007    122
2006     50
Name: count, dtype: int64
```












We can build a plot just calling it at the end of the sentence.










In [ ]:



```
ted.film\_datetime.dt.year.value\_counts().plot()

```










Out[ ]:


```
<Axes: xlabel='film_datetime'>
```






![](data:image/png;base64,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OjYRXRkDChH5Rb9+/bBr1y5Mnz7ds2znzp1e62zfvh1LlizBxIkTATgHn168eNFrHZVKBbvd7rVs+PDhOHnyJHr27HnF4ze3nS8MHz4c//rXv5CQkACdTufz/RORE7t4iMgvnn76aXz44YdYtmwZfvzxR7zyyis4evSo1zq9evXCxx9/jOPHj2PXrl2YNm0aIiMjvdbJysrChg0bUFJSgkuXLgEAXn75ZfzjH//AwoULcfToURw/fhyffPIJXnrppRa384Vp06aha9euuPPOO/H999/j7Nmz2Lx5M375y196BtIS0dVjQCEiv7j33nvxm9/8Bi+88AKys7Nx/vx5zJkzx2udDz74AJcuXcLw4cPx0EMP4Ze//CUSEhK81vnjH/+I9evXIz09HcOGDQMA5ObmYt26dfjvf/+LESNGYNSoUVi8eDEyMzNb3M4XtFottm7dioyMDEyePBn9+vXzTKFmiwqR78iEEELqIoiIiIgaYgsKERERBR0GFCLqkAEDBnhN8234am6GCxFRe7CLh4g65Pz587Barc1+5r69PRFRRzGgEBERUdBhFw8REREFHQYUIiIiCjoMKERERBR0GFCIiIgo6DCgEBERUdBhQCEiIqKgw4BCREREQYcBhYiIiILO/wdh5dzA8Ps+ZAAAAABJRU5ErkJggg==)











What can be concluded from the plot?












Not much since the data is not ordered. Pandas will show them by default in the order in which they appear.










In [ ]:



```
ted.film\_datetime.dt.year.value\_counts().sort\_index().plot()

```










Out[ ]:


```
<Axes: xlabel='film_datetime'>
```






![](data:image/png;base64,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dwwRERFxYRbDMAyzQ1RWTk4OQUFBZGdnO/Rwj4iIiNhPZb6/damKiIiIOB0VFBEREXE6KigiIiLidFRQRERExOmooIiIiIjTUUERERERp6OCIiIiIk5HBUVEREScjgqKiIiIOB0VFBEREXE6dp+LpzpcuDt/Tk6OyUlERETkSl343r6SWXZcsqDk5uYCEB0dbXISERERqazc3FyCgoIuuYxLThZotVpJSUkhICAAi8Vi18/OyckhOjqapKQkTURYBdqP9qH9aB/aj/ah/WgftXk/GoZBbm4ukZGRuLld+iwTlxxBcXNzIyoqyqHrCAwMrHW/OI6g/Wgf2o/2of1oH9qP9lFb9+PlRk4u0EmyIiIi4nRUUERERMTpqKD8D29vb1588UW8vb3NjuLStB/tQ/vRPrQf7UP70T60H6+MS54kKyIiIjWbRlBERETE6aigiIiIiNNRQRERERGnU+MKyvTp0+nWrRsBAQGEhoZy6623cuDAgQrLFBYWMmnSJOrVq4e/vz8jRowgPT29wjKJiYkMHToUPz8/QkNDmTp1KqWlpRWWKSoq4s9//jMxMTF4e3sTGxvLRx995PBtrA7VuR/nz59Px44d8fPzIyIigvvuu48zZ844fBurg73242OPPUbXrl3x9vamU6dOF13Xzp076dOnDz4+PkRHR/P66687arOqXXXtx1WrVnHLLbcQERFBnTp16NSpE/Pnz3fkplWr6vx9vODw4cMEBAQQHBxs560xT3XuR8MwePPNN2nRogXe3t40bNiQv/3tb47aNKdS4wrK6tWrmTRpEhs3bmTZsmWUlJQwcOBA8vPzbcs8+eSTLF68mIULF7J69WpSUlIYPny47fWysjKGDh1KcXExGzZsYO7cucyZM4cXXnihwrruuOMOli9fzqxZszhw4ACfffYZLVu2rLZtdaTq2o/r169nzJgxTJgwgT179rBw4UI2b97MxIkTq3V7HcUe+/GC++67jzvvvPOi68nJyWHgwIHExMSQkJDAG2+8wUsvvcS//vUvh21bdaqu/bhhwwY6dOjAV199xc6dOxk/fjxjxoxhyZIlDtu26lRd+/GCkpIS7r77bvr06WP3bTFTde7Hxx9/nP/85z+8+eab7N+/n++++47u3bs7ZLucjlHDZWRkGICxevVqwzAMIysry/D09DQWLlxoW2bfvn0GYMTHxxuG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PXdhm/Py8ujatSvz58//zWc1aNCgUusWkd+ngiIiDtG6dWs2bdrEmDFjbM9t3LixwjLr169n5syZDBkyBCg/+fT06dMVlvH09KSsrKzCc126dOHAgQM0a9bsd9d/sffZQ5cuXfjiiy8IDQ0lMDDQ7p8vIuV0iEdEHOLxxx/no48+Yvbs2Rw8eJAXX3yRPXv2VFimefPmzJs3j3379rFp0yZGjRqFr69vhWViY2NZvnw5aWlpnD17FoAXXniBjz/+mJdffpk9e/awb98+Pv/8c5577rlLvs8eRo0aRf369bnllltYu3Ytx44dY9WqVTz22GO2E2lFpOpUUETEIe68806ef/55nnnmGbp27cqJEyd4+OGHKywza9Yszp49S5cuXRg9ejSPPfYYoaGhFZZ56623WLZsGdHR0XTu3BmAQYMGsWTJEn766Se6detGz549mTFjBjExMZd8nz34+fmxZs0aGjVqxPDhw2ndurXtEmqNqIjYj8UwDMPsECIiIiK/phEUERERcToqKCJyVdq2bVvhMt9fPy52hYuISGXoEI+IXJUTJ05QUlJy0dcu3N5eRORqqaCIiIiI09EhHhEREXE6KigiIiLidFRQRERExOmooIiIiIjTUUERERERp6OCIiIiIk5HBUVEREScjgqKiIiIOJ3/Dym5uaHBmQWrAAAAAElFTkSuQmCC)











It makes more sense.










In [ ]:



```
ted.film\_datetime.dt.day\_of\_year

```










Out[ ]:


```
0       178
1       178
2       178
3       178
4       178
       ... 
2545    262
2546    263
2547    264
2548    264
2549    265
Name: film_datetime, Length: 2550, dtype: int32
```












Other namespaces by the type of the column










In [ ]:



```
ted.event.str.lower()

```










Out[ ]:


```
0            ted2006
1            ted2006
2            ted2006
3            ted2006
4            ted2006
            ...     
2545         ted2017
2546         ted2017
2547         ted2017
2548    tedxmilehigh
2549         ted2017
Name: event, Length: 2550, dtype: object
```












Is the number of talks in steep decline?










In [ ]:



```
ted[ted.film\_datetime.dt.year =='2017'].value\_counts()

```










Out[ ]:


```
Series([], Name: count, dtype: int64)
```










In [ ]:



```
ted[ted.film\_datetime.dt.year==2017].film\_datetime.dt.year.value\_counts()

```










Out[ ]:


```
film_datetime
2017    197
Name: count, dtype: int64
```










In [ ]:



```
ted[ted.film\_datetime.dt.year==2016].film\_datetime.dt.year.value\_counts()

```










Out[ ]:


```
film_datetime
2016    243
Name: count, dtype: int64
```












Are TED talks on steep decline on 2017? No, maybe the dataset is missing data from 2017 an onwards.


**Sometimes it is convenient to removing data from the dataset so the conclusions are relevant**












## What were the "best" events in TED history to attend?[¶](#What-were-the-%22best%22-events-in-TED-history-to-attend?)












# Exercise 1.[¶](#Exercise-1.)












1. How can we measure event/talk quality?


Let's use number of views for a talk as a measure of quality. The event with the greatest number of views in its talks is the best event.


**We have to consider that an event is a aggregation of talks.**












## Using aggregations with Pandas[¶](#Using-aggregations-with-Pandas)

* groupby over a column
* For each category you can call an aggregate function ( 'mean' in this case)
* You can later sort by value or sort by index












The code shown below means to sort the events which talks have the least amount of views (mean).










In [ ]:



```
ted.groupby('event').views.mean().sort\_values().head()

```










Out[ ]:


```
event
The Do Lectures           112321.0
TEDxIslay                 120274.0
TEDxWaterloo              138812.0
AORN Congress             149818.0
TEDxNASA@SiliconValley    155895.0
Name: views, dtype: float64
```












The code shown below means to sort the events which talks have the highest amount views (mean).












1. Group by event


2.For each event
3.Aggregation = mean
4.Column = views










In [ ]:



```
ted.groupby('event').views.mean().sort\_values().tail()

```










Out[ ]:


```
event
TEDxNorrkoping        6569493.0
TEDxCreativeCoast     8444981.0
TEDxBloomington       9484259.5
TEDxHouston          16140250.5
TEDxPuget Sound      34309432.0
Name: views, dtype: float64
```












However we would like to detail more: maybe an event had a few successful talks












TEDExPugetSound looks like a great event, but let's break it down to see the talks per event. We need to group by two columns:


1. We need 2 different aggregations












## Using multiple aggregation functions[¶](#Using-multiple-aggregation-functions)










In [ ]:



```
ted.groupby('event').views.agg(['count','mean']).sort\_values('mean').tail()

```










Out[ ]:



 .dataframe tbody tr th:only-of-type {
 vertical-align: middle;
 }

 .dataframe tbody tr th {
 vertical-align: top;
 }

 .dataframe thead th {
 text-align: right;
 }



|  | count | mean |
| --- | --- | --- |
| event |  |  |
| TEDxNorrkoping | 1 | 6569493.0 |
| TEDxCreativeCoast | 1 | 8444981.0 |
| TEDxBloomington | 2 | 9484259.5 |
| TEDxHouston | 2 | 16140250.5 |
| TEDxPuget Sound | 1 | 34309432.0 |














We see TEDxPuget Sound had just one talk (or at least one that was published), and maybe that one was a really good one.


Adding 'sum' to the agg functions, to see **what events had the most total number of views**










In [ ]:



```
ted.groupby('event').views.agg(['count','mean','sum']).sort\_values('sum').tail()

```










Out[ ]:



 .dataframe tbody tr th:only-of-type {
 vertical-align: middle;
 }

 .dataframe tbody tr th {
 vertical-align: top;
 }

 .dataframe thead th {
 text-align: right;
 }



|  | count | mean | sum |
| --- | --- | --- | --- |
| event |  |  |  |
| TED2006 | 45 | 3.274345e+06 | 147345533 |
| TED2015 | 75 | 2.011017e+06 | 150826305 |
| TEDGlobal 2013 | 66 | 2.584163e+06 | 170554736 |
| TED2014 | 84 | 2.072874e+06 | 174121423 |
| TED2013 | 77 | 2.302700e+06 | 177307937 |














## Conclusions[¶](#Conclusions)

1. Think about how to use data creatively
2. Think about the disavantages of your approach.
3. Using small sample sizes










In [ ]:



```
 

```












## Unpack ratings data[¶](#Unpack-ratings-data)












Ratings data is in a stringified json format, so it needs "unpacking" in a way that we can work with this data.










In [ ]:



```
ted.ratings.head()

```










Out[ ]:


```
0    [{'id': 7, 'name': 'Funny', 'count': 19645}, {...
1    [{'id': 7, 'name': 'Funny', 'count': 544}, {'i...
2    [{'id': 7, 'name': 'Funny', 'count': 964}, {'i...
3    [{'id': 3, 'name': 'Courageous', 'count': 760}...
4    [{'id': 9, 'name': 'Ingenious', 'count': 3202}...
Name: ratings, dtype: object
```












## Evaluate a string in a given object format and return as the object it is formatted like[¶](#Evaluate-a-string-in-a-given-object-format-and-return-as-the-object-it-is-formatted-like)










In [ ]:



```
import ast

```












This library can be used to describe a stringified list and retrieve it as a list object










In [ ]:



```
ast.literal\_eval('[1,2,3]')

```










Out[ ]:


```
[1, 2, 3]
```










In [ ]:



```
ted.ratings

```










Out[ ]:


```
0       [{'id': 7, 'name': 'Funny', 'count': 19645}, {...
1       [{'id': 7, 'name': 'Funny', 'count': 544}, {'i...
2       [{'id': 7, 'name': 'Funny', 'count': 964}, {'i...
3       [{'id': 3, 'name': 'Courageous', 'count': 760}...
4       [{'id': 9, 'name': 'Ingenious', 'count': 3202}...
                              ...                        
2545    [{'id': 3, 'name': 'Courageous', 'count': 24},...
2546    [{'id': 22, 'name': 'Fascinating', 'count': 32...
2547    [{'id': 1, 'name': 'Beautiful', 'count': 14}, ...
2548    [{'id': 11, 'name': 'Longwinded', 'count': 3},...
2549    [{'id': 21, 'name': 'Unconvincing', 'count': 2...
Name: ratings, Length: 2550, dtype: object
```










In [ ]:



```
type(ted.ratings)

```










Out[ ]:


```
pandas.core.series.Series
```










In [ ]:



```
type(ted.ratings[0])

```










Out[ ]:


```
str
```










In [ ]:



```
ast.literal\_eval(ted.ratings[0])

```










Out[ ]:


```
[{'id': 7, 'name': 'Funny', 'count': 19645},
 {'id': 1, 'name': 'Beautiful', 'count': 4573},
 {'id': 9, 'name': 'Ingenious', 'count': 6073},
 {'id': 3, 'name': 'Courageous', 'count': 3253},
 {'id': 11, 'name': 'Longwinded', 'count': 387},
 {'id': 2, 'name': 'Confusing', 'count': 242},
 {'id': 8, 'name': 'Informative', 'count': 7346},
 {'id': 22, 'name': 'Fascinating', 'count': 10581},
 {'id': 21, 'name': 'Unconvincing', 'count': 300},
 {'id': 24, 'name': 'Persuasive', 'count': 10704},
 {'id': 23, 'name': 'Jaw-dropping', 'count': 4439},
 {'id': 25, 'name': 'OK', 'count': 1174},
 {'id': 26, 'name': 'Obnoxious', 'count': 209},
 {'id': 10, 'name': 'Inspiring', 'count': 24924}]
```










In [ ]:



```
type(ast.literal\_eval(ted.ratings[0]))

```










Out[ ]:


```
list
```












Creating a function to encapsulate this










In [ ]:



```
def  str\_to\_list(ratings\_list):
    return ast.literal\_eval(ratings\_list)

```












So that we can apply this function to this field on the dataframe










In [ ]:



```
ted ['ratings\_list']=ted.ratings.apply( lambda x: ast.literal\_eval(x))

```










In [ ]:



```
ted.ratings\_list

```










Out[ ]:


```
0       [{'id': 7, 'name': 'Funny', 'count': 19645}, {...
1       [{'id': 7, 'name': 'Funny', 'count': 544}, {'i...
2       [{'id': 7, 'name': 'Funny', 'count': 964}, {'i...
3       [{'id': 3, 'name': 'Courageous', 'count': 760}...
4       [{'id': 9, 'name': 'Ingenious', 'count': 3202}...
                              ...                        
2545    [{'id': 3, 'name': 'Courageous', 'count': 24},...
2546    [{'id': 22, 'name': 'Fascinating', 'count': 32...
2547    [{'id': 1, 'name': 'Beautiful', 'count': 14}, ...
2548    [{'id': 11, 'name': 'Longwinded', 'count': 3},...
2549    [{'id': 21, 'name': 'Unconvincing', 'count': 2...
Name: ratings_list, Length: 2550, dtype: object
```










In [ ]:



```
type(ted.ratings\_list)

```










Out[ ]:


```
pandas.core.series.Series
```










In [ ]:



```
type(ted.ratings\_list[0])

```










Out[ ]:


```
list
```












## Map vs apply[¶](#Map-vs-apply)

1. Map seems to have a subset of apply


2.Use apply anytime it's necessary
3. Don't use apply when there is a built-in function that can do the same: usually built-in pandas functions are more reliable , performant, documented and tested.
4. Map is a better wrap for performance. However you don't always care about performance and sometimes they are equivalent (like for a small number of values).
5.Use apply last, rather than fast.
6. Apply is confusing because:


* There is a series apply method
* There is a dataframe apply method
* There is a series map method
* There is a dataframe applymap method


Use it with care!












We added a column that is a series of lists, cotaining the ratings for the talks ( instead of series of stringified lists)












## Count the number of ratings received by each talk and store it in a column called num\_ratings[¶](#Count-the-number-of-ratings-received-by-each-talk-and-store-it-in-a-column-called-num_ratings)












1. For each talk, calculate the percentage of ratings that were negative
2. For each talk, calculate the average number of ratings it received per day since it was published.










In [ ]:



```
ted.ratings\_list[1]

```










Out[ ]:


```
[{'id': 7, 'name': 'Funny', 'count': 544},
 {'id': 3, 'name': 'Courageous', 'count': 139},
 {'id': 2, 'name': 'Confusing', 'count': 62},
 {'id': 1, 'name': 'Beautiful', 'count': 58},
 {'id': 21, 'name': 'Unconvincing', 'count': 258},
 {'id': 11, 'name': 'Longwinded', 'count': 113},
 {'id': 8, 'name': 'Informative', 'count': 443},
 {'id': 10, 'name': 'Inspiring', 'count': 413},
 {'id': 22, 'name': 'Fascinating', 'count': 132},
 {'id': 9, 'name': 'Ingenious', 'count': 56},
 {'id': 24, 'name': 'Persuasive', 'count': 268},
 {'id': 23, 'name': 'Jaw-dropping', 'count': 116},
 {'id': 26, 'name': 'Obnoxious', 'count': 131},
 {'id': 25, 'name': 'OK', 'count': 203}]
```










In [ ]:



```
def get\_num\_ratings(list\_of\_dicts):
    num = 0
    for d in list\_of\_dicts:
        num = num + d['count']
    return num

```










In [ ]:



```
get\_num\_ratings(ted.ratings\_list[1])

```










Out[ ]:


```
2936
```










In [ ]:



```
ted['num\_ratings'] = ted.ratings\_list.apply(get\_num\_ratings)

```










In [ ]:



```
ted.num\_ratings

```










Out[ ]:


```
0       93850
1        2936
2        2824
3        3728
4       25620
        ...  
2545      192
2546      151
2547      136
2548      583
2549      142
Name: num_ratings, Length: 2550, dtype: int64
```










In [ ]:



```
ted.num\_ratings.describe()

```










Out[ ]:


```
count     2550.000000
mean      2436.408235
std       4226.795631
min         68.000000
25%        870.750000
50%       1452.500000
75%       2506.750000
max      93850.000000
Name: num_ratings, dtype: float64
```












Another way to do this ( Using lambdas in one go!)










In [ ]:



```
pd.DataFrame(ted.ratings\_list[0])['count'].sum()

```










Out[ ]:


```
93850
```










In [ ]:



```
ted['another\_num\_ratings'] = ted.ratings\_list.apply( lambda x: pd.DataFrame(x)['count'].sum())

```










In [ ]:



```
ted.another\_num\_ratings

```










Out[ ]:


```
0       93850
1        2936
2        2824
3        3728
4       25620
        ...  
2545      192
2546      151
2547      136
2548      583
2549      142
Name: another_num_ratings, Length: 2550, dtype: int64
```










In [ ]:



```
ted.another\_num\_ratings.describe()

```










Out[ ]:


```
count     2550.000000
mean      2436.408235
std       4226.795631
min         68.000000
25%        870.750000
50%       1452.500000
75%       2506.750000
max      93850.000000
Name: another_num_ratings, dtype: float64
```












## Conclusions[¶](#Conclusions)

1. Write one-liners as much as you can and check your work as you go
2. Lambda is best for simple functions












## Which occupations deliver the funniest TED talks on average?[¶](#Which-occupations-deliver-the-funniest-TED-talks-on-average?)












## Step 1: Count the number of funny ratings[¶](#Step-1:-Count-the-number-of-funny-ratings)










In [ ]:



```
ted.ratings\_list.head()

```










Out[ ]:


```
0    [{'id': 7, 'name': 'Funny', 'count': 19645}, {...
1    [{'id': 7, 'name': 'Funny', 'count': 544}, {'i...
2    [{'id': 7, 'name': 'Funny', 'count': 964}, {'i...
3    [{'id': 3, 'name': 'Courageous', 'count': 760}...
4    [{'id': 9, 'name': 'Ingenious', 'count': 3202}...
Name: ratings_list, dtype: object
```












1. Does every rating contain a "Funny" score?










In [ ]:



```
ted.ratings.str.contains('Funny').value\_counts()

```










Out[ ]:


```
ratings
True    2550
Name: count, dtype: int64
```










In [ ]:



```
def get\_funny\_ratings(list\_of\_dicts):
    for d in list\_of\_dicts:
        if d['name']=='Funny':
            return d['count']
        
        

```










In [ ]:



```
ted['funny\_ratings'] = ted.ratings\_list.apply(get\_funny\_ratings)

```










In [ ]:



```
ted.funny\_ratings

```










Out[ ]:


```
0       19645
1         544
2         964
3          59
4        1390
        ...  
2545        1
2546       20
2547        1
2548       63
2549        0
Name: funny_ratings, Length: 2550, dtype: int64
```










In [ ]:



```
ted.funny\_ratings.describe()

```










Out[ ]:


```
count     2550.000000
mean       154.468627
std        589.137728
min          0.000000
25%          8.000000
50%         21.000000
75%         92.000000
max      19645.000000
Name: funny_ratings, dtype: float64
```










In [ ]:



```
ted['funny\_rate'] = ted.funny\_ratings / ted.num\_ratings

```










In [ ]:



```
ted.funny\_rate

```










Out[ ]:


```
0       0.209323
1       0.185286
2       0.341360
3       0.015826
4       0.054254
          ...   
2545    0.005208
2546    0.132450
2547    0.007353
2548    0.108062
2549    0.000000
Name: funny_rate, Length: 2550, dtype: float64
```










In [ ]:



```
ted.funny\_rate.describe()

```










Out[ ]:


```
count    2550.000000
mean        0.050361
std         0.087779
min         0.000000
25%         0.005922
50%         0.014981
75%         0.047736
max         0.702076
Name: funny_rate, dtype: float64
```












How to verify that this measure makes sense? Sorting about the "Funny" rating for each talk in the listings would make sense.










In [ ]:



```
ted.sort\_values('funny\_rate').speaker\_occupation.tail(20)

```










Out[ ]:


```
1849                       Science humorist
337                                Comedian
124     Performance poet, multimedia artist
315                                  Expert
1168             Social energy entrepreneur
1468                          Ornithologist
595                  Comedian, voice artist
1534                         Cartoon editor
97                                 Satirist
2297                          Actor, writer
568                                Comedian
675                          Data scientist
21                     Humorist, web artist
194                                Jugglers
2273                    Comedian and writer
2114                    Comedian and writer
173                                Investor
747                                Comedian
1398                               Comedian
685             Actor, comedian, playwright
Name: speaker_occupation, dtype: object
```










In [ ]:



```
ted.sort\_values('funny\_rate').speaker\_occupation.head(20)

```










Out[ ]:


```
2549               Game designer
1612                   Biologist
612                     Sculptor
998               Penguin expert
593                     Engineer
284               Space activist
1041         Biomedical engineer
1618      Spinal cord researcher
2132    Computational geneticist
442                     Sculptor
426              Author, thinker
458                     Educator
2437      Environmental engineer
1491             Photojournalist
1893     Forensic anthropologist
783             Marine biologist
195                    Kenyan MP
772             HIV/AIDS fighter
788            Building activist
936                Neuroengineer
Name: speaker_occupation, dtype: object
```












## Step 3: Analyze the funny rate by occupation[¶](#Step-3:-Analyze-the-funny-rate-by-occupation)












Using group by , used by speaker would give us the funny rate by occupation










In [ ]:



```
ted.groupby('speaker\_occupation').funny\_rate.mean().sort\_values().tail(20)

```










Out[ ]:


```
speaker_occupation
Cartoonist                       0.369335
YouTube trends manager           0.404886
Entrepreneur, Lego enthusiast    0.409814
First aid instructor             0.413043
Expert                           0.415295
Philosopher-comic                0.415871
Marketing expert                 0.434353
Pranksters                       0.437240
African grey parrot              0.441525
Comedian + Designer              0.463068
Science humorist                 0.468405
Social energy entrepreneur       0.502117
Comedian, voice artist           0.503542
Cartoon editor                   0.511628
Satirist                         0.512383
Comedian                         0.512457
Actor, writer                    0.515152
Actor, comedian, playwright      0.558107
Jugglers                         0.566828
Comedian and writer              0.602085
Name: funny_rate, dtype: float64
```










In [ ]:



```
ted.speaker\_occupation.describe()

```










Out[ ]:


```
count       2544
unique      1458
top       Writer
freq          45
Name: speaker_occupation, dtype: object
```












The problem with this calculation is that these occupations have a small sample size. 
1458 are unique values, so there is a lot of occupations that are unique












## Focus on occupations that are well-represented in the data[¶](#Focus-on-occupations-that-are-well-represented-in-the-data)












1. Generate a list of the most represented occupations










In [ ]:



```
occupation\_counts = ted.speaker\_occupation.value\_counts()

```










In [ ]:



```
top\_occupations = occupation\_counts [occupation\_counts>= 5].index

```










In [ ]:



```
top\_occupations

```










Out[ ]:


```
Index(['Writer', 'Artist', 'Designer', 'Journalist', 'Entrepreneur',
       'Architect', 'Inventor', 'Psychologist', 'Photographer', 'Filmmaker',
       'Economist', 'Author', 'Neuroscientist', 'Educator', 'Roboticist',
       'Philosopher', 'Biologist', 'Physicist', 'Musician', 'Marine biologist',
       'Activist', 'Global health expert; data visionary', 'Technologist',
       'Graphic designer', 'Historian', 'Philanthropist', 'Astronomer',
       'Behavioral economist', 'Oceanographer', 'Singer/songwriter', 'Poet',
       'Futurist', 'Engineer', 'Computer scientist', 'Social psychologist',
       'Novelist', 'Mathematician', 'Astrophysicist', 'Social entrepreneur',
       'Photojournalist', 'Writer, activist', 'Evolutionary biologist',
       'Legal activist', 'Climate advocate', 'Techno-illusionist',
       'Singer-songwriter', 'Comedian', 'Performance poet, multimedia artist',
       'Reporter', 'Paleontologist', 'Chemist', 'Cartoonist',
       'Investor and advocate for moral leadership', 'Violinist',
       'Tech visionary', 'Producer', 'Sound consultant', 'Game designer',
       'Physician', 'Surgeon', 'Sculptor', 'Researcher', 'Science writer',
       'Data scientist', 'Musician, activist', 'Social Media Theorist',
       'Environmentalist, futurist', 'Chef'],
      dtype='object', name='speaker_occupation')
```










In [ ]:



```
type(top\_occupations)

```










Out[ ]:


```
pandas.core.indexes.base.Index
```










In [ ]:



```
ted\_top\_occupations = ted[ted['speaker\_occupation'].isin(top\_occupations)]

```










In [ ]:



```
ted\_top\_occupations.shape

```










Out[ ]:


```
(786, 25)
```










In [ ]:



```
ted\_top\_occupations.describe()

```










Out[ ]:



 .dataframe tbody tr th:only-of-type {
 vertical-align: middle;
 }

 .dataframe tbody tr th {
 vertical-align: top;
 }

 .dataframe thead th {
 text-align: right;
 }



|  | comments | duration | film\_date | languages | num\_speaker | published\_date | views | comments\_per\_view | views\_per\_comment | film\_datetime | num\_ratings | another\_num\_ratings | funny\_ratings | funny\_rate |
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
| count | 786.000000 | 786.000000 | 7.860000e+02 | 786.000000 | 786.000000 | 7.860000e+02 | 7.860000e+02 | 786.000000 | 786.000000 | 786 | 786.000000 | 786.000000 | 786.000000 | 786.000000 |
| mean | 205.409669 | 826.286260 | 1.301029e+09 | 27.815522 | 1.034351 | 1.326715e+09 | 1.712339e+06 | 0.000154 | 14206.494098 | 2012-01-16 11:49:37.044529152 | 2525.507634 | 2525.507634 | 165.482188 | 0.053808 |
| min | 2.000000 | 135.000000 | 4.265316e+08 | 0.000000 | 1.000000 | 1.151367e+09 | 5.044300e+04 | 0.000003 | 683.134291 | 2006-06-27 00:11:00 | 142.000000 | 142.000000 | 0.000000 | 0.000000 |
| 25% | 63.000000 | 541.500000 | 1.233965e+09 | 23.000000 | 1.000000 | 1.251356e+09 | 7.192218e+05 | 0.000059 | 5540.287089 | 2009-08-27 07:00:00 | 918.000000 | 918.000000 | 8.000000 | 0.006463 |
| 50% | 124.000000 | 848.000000 | 1.310558e+09 | 28.000000 | 1.000000 | 1.323102e+09 | 1.123634e+06 | 0.000106 | 9473.250007 | 2011-12-05 16:19:41 | 1490.000000 | 1490.000000 | 26.000000 | 0.017125 |
| 75% | 224.750000 | 1063.000000 | 1.394950e+09 | 34.000000 | 1.000000 | 1.401073e+09 | 1.759730e+06 | 0.000180 | 16808.135662 | 2014-05-26 02:54:11.500000 | 2640.000000 | 2640.000000 | 110.000000 | 0.055667 |
| max | 6404.000000 | 3955.000000 | 1.503792e+09 | 72.000000 | 4.000000 | 1.506092e+09 | 4.315540e+07 | 0.001464 | 323087.000000 | 2017-09-22 15:00:22 | 65968.000000 | 65968.000000 | 7315.000000 | 0.669927 |
| std | 339.003617 | 404.903481 | 1.274605e+08 | 10.260198 | 0.202130 | 9.433474e+07 | 2.509243e+06 | 0.000170 | 18131.368966 | NaN | 3904.029024 | 3904.029024 | 482.137463 | 0.089033 |












In [ ]:



```
ted\_top\_occupations.groupby('speaker\_occupation').funny\_rate.mean().sort\_values().tail(20)

```










Out[ ]:


```
speaker_occupation
Science writer                          0.055993
Designer                                0.059287
Writer                                  0.060745
Game designer                           0.062317
Reporter                                0.066250
Evolutionary biologist                  0.069157
Novelist                                0.070876
Entrepreneur                            0.073295
Author                                  0.075508
Artist                                  0.078939
Global health expert; data visionary    0.090306
Poet                                    0.107398
Graphic designer                        0.135718
Techno-illusionist                      0.152171
Cartoonist                              0.162120
Data scientist                          0.184076
Producer                                0.202531
Singer/songwriter                       0.252205
Performance poet, multimedia artist     0.306468
Comedian                                0.512457
Name: funny_rate, dtype: float64
```






















## Conclusions[¶](#Conclusions)

1. Check your assumptions about your data
2. Check whether your results make sense.
3. Check the type of pandas operations: they are usually DataFrame or Series.
4. Watch out for small sample sizes.
5. Consider the impact of missing data: this is NOT showing any errors :)












# Pandas Tips and Tricks[¶](#Pandas-Tips-and-Tricks)












**Credits**: From the video of same author https://youtu.be/RlIiVeig3hc












1. Show Pandas Versions (and from its dependencies)










In [ ]:



```
pd.show\_versions()

```













```

INSTALLED VERSIONS
------------------
commit           : 37ea63d540fd27274cad6585082c91b1283f963d
python           : 3.9.6.final.0
python-bits      : 64
OS               : Darwin
OS-release       : 22.4.0
Version          : Darwin Kernel Version 22.4.0: Mon Mar  6 20:59:28 PST 2023; root:xnu-8796.101.5~3/RELEASE_ARM64_T6000
machine          : arm64
processor        : arm
byteorder        : little
LC_ALL           : None
LANG             : None
LOCALE           : None.UTF-8

pandas           : 2.0.1
numpy            : 1.23.3
pytz             : 2022.2.1
dateutil         : 2.8.2
setuptools       : 58.0.4
pip              : 21.2.4
Cython           : None
pytest           : None
hypothesis       : None
sphinx           : None
blosc            : None
feather          : None
xlsxwriter       : None
lxml.etree       : 4.9.1
html5lib         : None
pymysql          : None
psycopg2         : None
jinja2           : 3.1.2
IPython          : 8.13.2
pandas_datareader: None
bs4              : 4.11.1
bottleneck       : None
brotli           : None
fastparquet      : None
fsspec           : None
gcsfs            : None
matplotlib       : 3.7.1
numba            : None
numexpr          : None
odfpy            : None
openpyxl         : None
pandas_gbq       : None
pyarrow          : None
pyreadstat       : None
pyxlsb           : None
s3fs             : None
scipy            : None
snappy           : None
sqlalchemy       : None
tables           : None
tabulate         : None
xarray           : None
xlrd             : None
zstandard        : None
tzdata           : 2023.3
qtpy             : 2.2.0
pyqt5            : None

```












2. Generate a sample Data Frame












What we do manually:










In [ ]:



```
df = pd.DataFrame({'col one':[100,200],'col two':[300,400]})

```










In [ ]:



```
df

```










Out[ ]:



 .dataframe tbody tr th:only-of-type {
 vertical-align: middle;
 }

 .dataframe tbody tr th {
 vertical-align: top;
 }

 .dataframe thead th {
 text-align: right;
 }



|  | col one | col two |
| --- | --- | --- |
| 0 | 100 | 300 |
| 1 | 200 | 400 |














Easier, using numpy:










In [ ]:



```
import numpy as np

```












Parameters are: rows,columns










In [ ]:



```
pd.DataFrame(np.random.rand(4,8))

```










Out[ ]:



 .dataframe tbody tr th:only-of-type {
 vertical-align: middle;
 }

 .dataframe tbody tr th {
 vertical-align: top;
 }

 .dataframe thead th {
 text-align: right;
 }



|  | 0 | 1 | 2 | 3 | 4 | 5 | 6 | 7 |
| --- | --- | --- | --- | --- | --- | --- | --- | --- |
| 0 | 0.570378 | 0.367411 | 0.865880 | 0.437038 | 0.354206 | 0.412463 | 0.330390 | 0.722543 |
| 1 | 0.167644 | 0.677556 | 0.615086 | 0.454293 | 0.614237 | 0.409272 | 0.704607 | 0.045908 |
| 2 | 0.285340 | 0.438551 | 0.402809 | 0.296770 | 0.996599 | 0.989184 | 0.386614 | 0.050287 |
| 3 | 0.283214 | 0.040261 | 0.310578 | 0.272318 | 0.544209 | 0.575619 | 0.861728 | 0.279068 |














Giving it the header for each column (as a list)










In [ ]:



```
pd.DataFrame(np.random.rand(4,8), columns=list('abcdefgh'))

```










Out[ ]:



 .dataframe tbody tr th:only-of-type {
 vertical-align: middle;
 }

 .dataframe tbody tr th {
 vertical-align: top;
 }

 .dataframe thead th {
 text-align: right;
 }



|  | a | b | c | d | e | f | g | h |
| --- | --- | --- | --- | --- | --- | --- | --- | --- |
| 0 | 0.034104 | 0.075956 | 0.334785 | 0.442860 | 0.179954 | 0.607041 | 0.558778 | 0.288265 |
| 1 | 0.650791 | 0.718474 | 0.694375 | 0.901698 | 0.437911 | 0.848726 | 0.272597 | 0.982334 |
| 2 | 0.344147 | 0.791109 | 0.560324 | 0.882701 | 0.282536 | 0.992830 | 0.900864 | 0.334858 |
| 3 | 0.645883 | 0.584075 | 0.442720 | 0.289285 | 0.273389 | 0.024719 | 0.316358 | 0.203573 |














3. Renaming columns












# Pandas AI[¶](#Pandas-AI)










In [ ]:



```
pip install pandasai

```













```
Defaulting to user installation because normal site-packages is not writeable
Requirement already satisfied: pandasai in /Users/sandralancheros/Library/Python/3.9/lib/python/site-packages (0.2.11)
Requirement already satisfied: openai<0.28.0,>=0.27.5 in /Users/sandralancheros/Library/Python/3.9/lib/python/site-packages (from pandasai) (0.27.6)
Requirement already satisfied: ipython<9.0.0,>=8.13.1 in /Users/sandralancheros/Library/Python/3.9/lib/python/site-packages (from pandasai) (8.13.2)
Requirement already satisfied: astor<0.9.0,>=0.8.1 in /Users/sandralancheros/Library/Python/3.9/lib/python/site-packages (from pandasai) (0.8.1)
Requirement already satisfied: python-dotenv<2.0.0,>=1.0.0 in /Users/sandralancheros/Library/Python/3.9/lib/python/site-packages (from pandasai) (1.0.0)
Requirement already satisfied: pandas<3.0.0,>=2.0.1 in /Users/sandralancheros/Library/Python/3.9/lib/python/site-packages (from pandasai) (2.0.1)
Requirement already satisfied: matplotlib<4.0.0,>=3.7.1 in /Users/sandralancheros/Library/Python/3.9/lib/python/site-packages (from pandasai) (3.7.1)
Requirement already satisfied: prompt-toolkit!=3.0.37,<3.1.0,>=3.0.30 in /Users/sandralancheros/Library/Python/3.9/lib/python/site-packages (from ipython<9.0.0,>=8.13.1->pandasai) (3.0.31)
Requirement already satisfied: pexpect>4.3 in /Users/sandralancheros/Library/Python/3.9/lib/python/site-packages (from ipython<9.0.0,>=8.13.1->pandasai) (4.8.0)
Requirement already satisfied: matplotlib-inline in /Users/sandralancheros/Library/Python/3.9/lib/python/site-packages (from ipython<9.0.0,>=8.13.1->pandasai) (0.1.6)
Requirement already satisfied: appnope in /Users/sandralancheros/Library/Python/3.9/lib/python/site-packages (from ipython<9.0.0,>=8.13.1->pandasai) (0.1.3)
Requirement already satisfied: stack-data in /Users/sandralancheros/Library/Python/3.9/lib/python/site-packages (from ipython<9.0.0,>=8.13.1->pandasai) (0.5.1)
Requirement already satisfied: backcall in /Users/sandralancheros/Library/Python/3.9/lib/python/site-packages (from ipython<9.0.0,>=8.13.1->pandasai) (0.2.0)
Requirement already satisfied: decorator in /Users/sandralancheros/Library/Python/3.9/lib/python/site-packages (from ipython<9.0.0,>=8.13.1->pandasai) (5.1.1)
Requirement already satisfied: traitlets>=5 in /Users/sandralancheros/Library/Python/3.9/lib/python/site-packages (from ipython<9.0.0,>=8.13.1->pandasai) (5.4.0)
Requirement already satisfied: pickleshare in /Users/sandralancheros/Library/Python/3.9/lib/python/site-packages (from ipython<9.0.0,>=8.13.1->pandasai) (0.7.5)
Requirement already satisfied: typing-extensions in /Users/sandralancheros/Library/Python/3.9/lib/python/site-packages (from ipython<9.0.0,>=8.13.1->pandasai) (4.5.0)
Requirement already satisfied: pygments>=2.4.0 in /Users/sandralancheros/Library/Python/3.9/lib/python/site-packages (from ipython<9.0.0,>=8.13.1->pandasai) (2.13.0)
Requirement already satisfied: jedi>=0.16 in /Users/sandralancheros/Library/Python/3.9/lib/python/site-packages (from ipython<9.0.0,>=8.13.1->pandasai) (0.18.1)
Requirement already satisfied: parso<0.9.0,>=0.8.0 in /Users/sandralancheros/Library/Python/3.9/lib/python/site-packages (from jedi>=0.16->ipython<9.0.0,>=8.13.1->pandasai) (0.8.3)
Requirement already satisfied: pyparsing>=2.3.1 in /Users/sandralancheros/Library/Python/3.9/lib/python/site-packages (from matplotlib<4.0.0,>=3.7.1->pandasai) (3.0.9)
Requirement already satisfied: packaging>=20.0 in /Users/sandralancheros/Library/Python/3.9/lib/python/site-packages (from matplotlib<4.0.0,>=3.7.1->pandasai) (21.3)
Requirement already satisfied: kiwisolver>=1.0.1 in /Users/sandralancheros/Library/Python/3.9/lib/python/site-packages (from matplotlib<4.0.0,>=3.7.1->pandasai) (1.4.4)
Requirement already satisfied: python-dateutil>=2.7 in /Users/sandralancheros/Library/Python/3.9/lib/python/site-packages (from matplotlib<4.0.0,>=3.7.1->pandasai) (2.8.2)
Requirement already satisfied: pillow>=6.2.0 in /Users/sandralancheros/Library/Python/3.9/lib/python/site-packages (from matplotlib<4.0.0,>=3.7.1->pandasai) (9.2.0)
Requirement already satisfied: contourpy>=1.0.1 in /Users/sandralancheros/Library/Python/3.9/lib/python/site-packages (from matplotlib<4.0.0,>=3.7.1->pandasai) (1.0.5)
Requirement already satisfied: numpy>=1.20 in /Users/sandralancheros/Library/Python/3.9/lib/python/site-packages (from matplotlib<4.0.0,>=3.7.1->pandasai) (1.23.3)
Requirement already satisfied: cycler>=0.10 in /Users/sandralancheros/Library/Python/3.9/lib/python/site-packages (from matplotlib<4.0.0,>=3.7.1->pandasai) (0.11.0)
Requirement already satisfied: fonttools>=4.22.0 in /Users/sandralancheros/Library/Python/3.9/lib/python/site-packages (from matplotlib<4.0.0,>=3.7.1->pandasai) (4.37.3)
Requirement already satisfied: importlib-resources>=3.2.0 in /Users/sandralancheros/Library/Python/3.9/lib/python/site-packages (from matplotlib<4.0.0,>=3.7.1->pandasai) (5.12.0)
Requirement already satisfied: zipp>=3.1.0 in /Users/sandralancheros/Library/Python/3.9/lib/python/site-packages (from importlib-resources>=3.2.0->matplotlib<4.0.0,>=3.7.1->pandasai) (3.8.1)
Requirement already satisfied: aiohttp in /Users/sandralancheros/Library/Python/3.9/lib/python/site-packages (from openai<0.28.0,>=0.27.5->pandasai) (3.8.4)
Requirement already satisfied: tqdm in /Users/sandralancheros/Library/Python/3.9/lib/python/site-packages (from openai<0.28.0,>=0.27.5->pandasai) (4.64.1)
Requirement already satisfied: requests>=2.20 in /Users/sandralancheros/Library/Python/3.9/lib/python/site-packages (from openai<0.28.0,>=0.27.5->pandasai) (2.28.1)
Requirement already satisfied: tzdata>=2022.1 in /Users/sandralancheros/Library/Python/3.9/lib/python/site-packages (from pandas<3.0.0,>=2.0.1->pandasai) (2023.3)
Requirement already satisfied: pytz>=2020.1 in /Users/sandralancheros/Library/Python/3.9/lib/python/site-packages (from pandas<3.0.0,>=2.0.1->pandasai) (2022.2.1)
Requirement already satisfied: ptyprocess>=0.5 in /Users/sandralancheros/Library/Python/3.9/lib/python/site-packages (from pexpect>4.3->ipython<9.0.0,>=8.13.1->pandasai) (0.7.0)
Requirement already satisfied: wcwidth in /Users/sandralancheros/Library/Python/3.9/lib/python/site-packages (from prompt-toolkit!=3.0.37,<3.1.0,>=3.0.30->ipython<9.0.0,>=8.13.1->pandasai) (0.2.5)
Requirement already satisfied: six>=1.5 in /Library/Developer/CommandLineTools/Library/Frameworks/Python3.framework/Versions/3.9/lib/python3.9/site-packages (from python-dateutil>=2.7->matplotlib<4.0.0,>=3.7.1->pandasai) (1.15.0)
Requirement already satisfied: idna<4,>=2.5 in /Users/sandralancheros/Library/Python/3.9/lib/python/site-packages (from requests>=2.20->openai<0.28.0,>=0.27.5->pandasai) (3.4)
Requirement already satisfied: certifi>=2017.4.17 in /Users/sandralancheros/Library/Python/3.9/lib/python/site-packages (from requests>=2.20->openai<0.28.0,>=0.27.5->pandasai) (2022.9.24)
Requirement already satisfied: charset-normalizer<3,>=2 in /Users/sandralancheros/Library/Python/3.9/lib/python/site-packages (from requests>=2.20->openai<0.28.0,>=0.27.5->pandasai) (2.1.1)
Requirement already satisfied: urllib3<1.27,>=1.21.1 in /Users/sandralancheros/Library/Python/3.9/lib/python/site-packages (from requests>=2.20->openai<0.28.0,>=0.27.5->pandasai) (1.26.12)
Requirement already satisfied: multidict<7.0,>=4.5 in /Users/sandralancheros/Library/Python/3.9/lib/python/site-packages (from aiohttp->openai<0.28.0,>=0.27.5->pandasai) (6.0.4)
Requirement already satisfied: aiosignal>=1.1.2 in /Users/sandralancheros/Library/Python/3.9/lib/python/site-packages (from aiohttp->openai<0.28.0,>=0.27.5->pandasai) (1.3.1)
Requirement already satisfied: async-timeout<5.0,>=4.0.0a3 in /Users/sandralancheros/Library/Python/3.9/lib/python/site-packages (from aiohttp->openai<0.28.0,>=0.27.5->pandasai) (4.0.2)
Requirement already satisfied: yarl<2.0,>=1.0 in /Users/sandralancheros/Library/Python/3.9/lib/python/site-packages (from aiohttp->openai<0.28.0,>=0.27.5->pandasai) (1.9.2)
Requirement already satisfied: attrs>=17.3.0 in /Users/sandralancheros/Library/Python/3.9/lib/python/site-packages (from aiohttp->openai<0.28.0,>=0.27.5->pandasai) (22.1.0)
Requirement already satisfied: frozenlist>=1.1.1 in /Users/sandralancheros/Library/Python/3.9/lib/python/site-packages (from aiohttp->openai<0.28.0,>=0.27.5->pandasai) (1.3.3)
Requirement already satisfied: executing in /Users/sandralancheros/Library/Python/3.9/lib/python/site-packages (from stack-data->ipython<9.0.0,>=8.13.1->pandasai) (1.1.0)
Requirement already satisfied: pure-eval in /Users/sandralancheros/Library/Python/3.9/lib/python/site-packages (from stack-data->ipython<9.0.0,>=8.13.1->pandasai) (0.2.2)
Requirement already satisfied: asttokens in /Users/sandralancheros/Library/Python/3.9/lib/python/site-packages (from stack-data->ipython<9.0.0,>=8.13.1->pandasai) (2.0.8)
WARNING: You are using pip version 21.2.4; however, version 23.1.2 is available.
You should consider upgrading via the '/Library/Developer/CommandLineTools/usr/bin/python3 -m pip install --upgrade pip' command.
Note: you may need to restart the kernel to use updated packages.

```










In [ ]:



```
from pandasai import PandasAI

```










In [ ]:



```
 

```










In [ ]:



```
{
    "tags": [
        "hide-cell"
    ]
}

```










Out[ ]:


```
{'tags': ['hide-cell']}
```










In [ ]:



```
# Instantiate a LLM
from pandasai.llm.openai import OpenAI
llm = OpenAI(api\_token="API\_KEY")

```










In [ ]:



```
df = pd.DataFrame({
    "country": ["United States", "United Kingdom", "France", "Germany", "Italy", "Spain", "Canada", "Australia", "Japan", "China"],
    "gdp": [19294482071552, 2891615567872, 2411255037952, 3435817336832, 1745433788416, 1181205135360, 1607402389504, 1490967855104, 4380756541440, 14631844184064],
    "happiness\_index": [6.94, 7.16, 6.66, 7.07, 6.38, 6.4, 7.23, 7.22, 5.87, 5.12]
})

```










In [ ]:



```
pandas\_ai = PandasAI(llm, conversational=False)
pandas\_ai.run(df, prompt='Which are the 5 happiest countries?')

```










Out[ ]:


```
'6            Canada\n7         Australia\n1    United Kingdom\n3           Germany\n0     United States\nName: country, dtype: object\n'
```










In [ ]:



```
pandas\_ai.run(
    df,
    "Plot the histogram of countries showing for each the gdp, using different colors for each bar",
)

```












![](data:image/png;base64,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NgBAPiz4qaPi+NRx5fObewkBAADLo7AAAADLo7AAAADLo7AAAADLo7AAAADLo7AAAADLo7AAAADLo7AAAADLo7AAAADLo7AAAADLo7AAAADLo7AAAADLo7AAAADLo7AAAADLo7AAAADLo7AAAADLo7AAAADLo7AAAADLo7AAAADLo7AAAADLo7AAAADLo7AAAADLo7AAAADLo7AAAADLo7AAAADLo7AAAADLo7AAAADLo7AAAADLo7AAAADLo7AAAADLo7AAAADLo7AAAADLo7AAAADLo7AAAADLc7mwrF+/Xr1791ZgYKBsNptWrlxZ4PYrVqxQ165dVb16dfn6+qp9+/b65ptvnLZ58cUXZbPZnB4333yzq9EAAEAp5XJhyczMVPPmzTVr1qxCbb9+/Xp17dpVX331lbZv36477rhDvXv31s6dO522a9y4sU6fPu14bNiwwdVoAACglCrj6gt69OihHj16FHr76dOnOz1/9dVX9emnn+rzzz9Xy5Yt/xekTBkFBAS4GgcAANwASnwMS05OjtLT01W1alWn5YcOHVJgYKBCQkL00EMPKTExMd99ZGVlKS0tzekBAABKrxIvLG+88YYyMjJ0//33O5aFh4drwYIFio2N1TvvvKNjx47ptttuU3p6ep77mDJliux2u+MRFBRUUvEBAIAJbIZhGNf9YptNn3zyifr27Vuo7ZcsWaKhQ4fq008/VURERL7bpaSkqE6dOpo2bZoGDx6ca31WVpaysrIcz9PS0hQUFKTU1FT5+vq6/D6uyWYr+n3+Vdf/1wYAsDgLfuqoOD510tLSZLfbC/X57fIYluu1dOlSDRkyRB999FGBZUWSKleurPr16+vw4cN5rvf29pa3t3dxxAQAABZUIqeEPvjgA0VFRemDDz5Qr169rrl9RkaGjhw5opo1a5ZAOgAAYHUuH2HJyMhwOvJx7NgxJSQkqGrVqqpdu7bGjRunkydPatGiRZKunAYaOHCgZsyYofDwcCUlJUmSypUrJ7vdLkl65pln1Lt3b9WpU0enTp3SxIkT5enpqf79+xfFewQAAG7O5SMs27ZtU8uWLR2XJEdHR6tly5aKiYmRJJ0+fdrpCp85c+bo999/1/Dhw1WzZk3HY9SoUY5tfv75Z/Xv318NGjTQ/fffr2rVqmnz5s2qXr36X31/AACgFPhLg26twpVBO9eFQbcAgBJkwU8d0wfdci8hAABgeRQWAABgeRQWAABgeRQWAABgeRQWAABgeRQWAABgeRQWAABgeRQWAABgeRQWAABgeRQWAABgeRQWAABgeRQWAABgeRQWAABgeRQWAABgeRQWAABgeRQWAABgeRQWAABgeRQWAABgeRQWAABgeRQWAABgeRQWAABgeRQWAABgeRQWAABgeRQWAABgeRQWAABgeRQWAABgeRQWAABgeRQWAABgeRQWAABgeRQWAABgeRQWAABgeRQWAABgeRQWAABgeRQWAABgeRQWAABgeS4XlvXr16t3794KDAyUzWbTypUrr/matWvXqlWrVvL29lZoaKgWLFiQa5tZs2apbt268vHxUXh4uLZs2eJqNAAAUEq5XFgyMzPVvHlzzZo1q1DbHzt2TL169dIdd9yhhIQEPfXUUxoyZIi++eYbxzbLli1TdHS0Jk6cqB07dqh58+aKjIzUmTNnXI0HAABKIZthGMZ1v9hm0yeffKK+ffvmu83YsWP15Zdf6scff3Qse/DBB5WSkqLY2FhJUnh4uG655Ra9/fbbkqScnBwFBQXpySef1HPPPZdrn1lZWcrKynI8T0tLU1BQkFJTU+Xr63u9byd/NlvR7/Ovuv6/NgCAxVnwU0fF8amTlpYmu91eqM/vYh/DEh8fr4iICKdlkZGRio+PlyRdunRJ27dvd9rGw8NDERERjm3+bMqUKbLb7Y5HUFBQ8b0BAABgumIvLElJSfL393da5u/vr7S0NP322286d+6csrOz89wmKSkpz32OGzdOqampjseJEyeKLT8AADBfGbMDXA9vb295e3ubHQMAAJSQYi8sAQEBSk5OdlqWnJwsX19flStXTp6envL09Mxzm4CAgOKOBwAA3ECxnxJq37694uLinJatWrVK7du3lyR5eXmpdevWTtvk5OQoLi7OsQ0AALixuVxYMjIylJCQoISEBElXLltOSEhQYmKipCvjSwYMGODY/h//+IeOHj2qZ599Vvv379e///1vffjhh3r66acd20RHR+u9997TwoULtW/fPg0bNkyZmZmKior6i28PAACUBi6fEtq2bZvuuOMOx/Po6GhJ0sCBA7VgwQKdPn3aUV4kKTg4WF9++aWefvppzZgxQzfddJPmzp2ryMhIxzYPPPCAzp49q5iYGCUlJalFixaKjY3NNRAXAADc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XcePHy/xPAW51jihP7LSmKGr7rzzTn322Wdq2bKloqKi9PTTT2v58uXatm2bS6dEzTB9+nQ999xzevfdd1W3bl2z4xQpTgkVE09PT50+fTrXwNvz58+rRo0aljrf/EfTpk3ThAkTNGLECMeg1Q0bNmjWrFmaPHmyZSb/ys/8+fM1YsQIjRkzRnfeeackKS4uTm+++aamT5+uoUOHmpwwt+Dg4HzX2Ww2y9+szN2upoiJidHcuXM1evRojR8/Xi+88IKOHz+ulStXKiYmxrIF8fbbb5ePj48WL14sf39/SVcGWA4YMEAXL17MNebMTJMmTSr0thMnTizGJNcnJydHOTk5KlPmyu/0S5cu1aZNmxQWFqbHH3/c0jclrVKlin799Vf9/vvvKl++fK5fgKxayAuDwlJMPDw8lJSUlKuwnDp1SvXq1dNvv/1mUrKCBQcHa9KkSRowYIDT8oULF+rFF190i7k03nnnHb3yyis6deqUJKlu3bp68cUXc70n/HV/vJpizpw5ua6meOWVV8yOmEu9evU0c+ZM9erVy2neoZkzZ2rz5s1asmSJ2RHzdPjwYfXr189xF3hJOnHihMLCwrRy5UqFhoaanBBWsHDhwgLXDxw4sISSFD0KSxGbOXOmJOnpp5/Wyy+/rIoVKzrWZWdna/369Tp+/LhlJ47z8fHRjz/+mOuH36FDh9S0aVNdvHjRpGSuO3v2rMqVK+f0d4CidfPNN2vixInq37+/03xDV6+mePvtt82OmEuFChW0b98+1a5dWzVr1tSXX36pVq1a6ejRo2rZsqXjHj1WZBiGVq1apf3790uSGjZsqIiICLcaZ+YufvnlF82bN88xNqhRo0aKiopS1apVTU5242IMSxF76623JF35wTJ79mx5eno61nl5ealu3bqaPXu2WfGuKTQ0VB9++KGef/55p+XLli2z1A3sCsOq9w7Ky88//6zPPvssz9Mq06ZNMynVtSUmJurWW2+VJJUrV07p6emSrszP0q5dO0sWFne9J4905RRht27d1K1bN7OjFJo7jhlav3697r77bvn6+qpNmzaSrvwy+tJLL+nzzz/X7bffbnJCZ2lpafL19XX8uSBXt3NHFJYidvWUyR133KEVK1aoSpUqJidyzaRJk/TAAw9o/fr1jjEsGzduVFxcnD788EOT012bO06aFBcXp7vvvlshISHav3+/mjRpouPHj8swDLVq1crseAVyx6sp+vXrp7i4OIWHh+vJJ5/Uww8/rHnz5ikxMdHyY7QyMzO1bt26PD/4rTr2ZtKkSQWOGbKi4cOH6/7779c777zj+KUzOztbTzzxhIYPH649e/aYnNBZlSpVHGMmK1eunOcRN8Mw3OIGtgXhlBBy2b59u9566y3HodCGDRtq9OjRatmypcnJrq1Hjx5KTEzUiBEj8pw0qU+fPiYly1/btm3Vo0cPTZo0yXFapUaNGnrooYfUvXt3DRs2zOyI+RoyZIiCgoI0ceJEzZo1S2PGjFGHDh0cV1PMmzfP7IjX5C735Nm5c6d69uypX3/9VZmZmapatarOnTun8uXLq0aNGpYdnO2OY4bKlSunhIQENWjQwGn5gQMH1KJFC8uNQVy3bp06dOigMmXKXHPwdadOnUooVdGjsBQjdz3M787ccdKkP/4Qr1KlijZs2KDGjRtr165d6tOnj+UuWf0jd76awt107txZ9evX1+zZs2W327Vr1y6VLVtWDz/8sEaNGmXZy23dccxQhw4dNGbMmFwzDa9cuVKvvfaaNm/ebE6wGxynhIqJOx3md+VGjFY//+mOkyZVqFDBUWhr1qypI0eOqHHjxpJk2cnurvr5558dV6xI0oMPPqgHH3xQhmHoxIkTql27tonp8nfgwAH961//cjqK+OSTT+b6jdpKEhIS9O6778rDw0Oenp7KyspSSEiIpk6dqoEDB1q2sLjjmKGRI0dq1KhROnz4sNq1aydJ2rx5s2bNmqXXXntNu3fvdmzbrFkzs2LmKyUlRVu2bMnzZqpufbWkgWJxyy23GDExMYZhGEbFihWNI0eOGOnp6cbdd99t/Pvf/zY5nTObzWZ4eHgU6mF133zzjdGtWzfj2LFjZkcptD59+hhz5swxDMMwRo8ebYSGhhqTJ082WrVqZXTp0sXkdAXz8PAwkpOTcy0/d+6cZb9fli9fbpQpU8Zo166d8fTTTxtPP/200b59e6NMmTLG8uXLzY6XLz8/P+PgwYOGYRhGWFiYERsbaxiGYezbt88oX768mdEKNHbsWOOVV14xDMMwli5dapQpU8YIDQ01vLy8jLFjx5qcLm82m63Ah4eHh+O/VvPZZ58ZlSpVMmw2m2G3243KlSs7HlWqVDE73l/CKaFi4k6H+f94zvP48eN67rnnNGjQIKf7lSxcuFBTpkyx/DX87jhp0tGjR5WRkaFmzZopMzNTo0ePdpxWmTZtmurUqWN2xHx5eHgoOTk51xVZP/30kxo1aqTMzEyTkuWvXr16euihh/TSSy85LZ84caL+85//6MiRIyYlK1i3bt00aNAg/f3vf9fQoUO1e/dujRw5UosXL9Yvv/yiH374weyIhbJ582bH97dVxwz99NNPhd7Wav8+69evr549e+rVV19V+fLlzY5TpCgsxSQgIEBr1qxRw4YN1ahRI7322mu6++67tWvXLnXo0EEZGRlmR8xTly5dNGTIEPXv399p+ZIlSzRnzhytXbvWnGCFVJonTbKS6OhoSdKMGTM0dOhQpx+M2dnZ+uGHH+Tp6amNGzeaFTFf5cuX1+7du/Oca6h58+b69ddfTUpWsG3btik9PV133HGHzpw5owEDBjg++OfPn6/mzZubHTGXy5cv6/HHH9eECRMKnNEZRadChQras2ePZW9F8lcwhqWYtGvXThs2bFDDhg3Vs2dPjR49Wnv27NGKFSsc50StKD4+Ps95Ytq0aaMhQ4aYkMg17l5IMjIycp1ztuK4oasTHxqGoT179jgNrvXy8lLz5s31zDPPmBWvQJ07d9b333+fq7Bs2LBBt912m0mpru3qfCCSVKNGDcXGxpqYpnDKli2rjz/+WBMmTDA7ynXZu3dvnhdN3H333SYlurbIyEht27atVBYWjrAUE3c9zN+gQQP16dNHU6dOdVr+7LPP6tNPP9WBAwdMSua6ixcv5vpBY8UP/2PHjmnEiBFau3at00zChhvMmxAVFaWZM2eqUqVKZkcptNmzZysmJkb333+/04DKjz76SJMmTVJgYKBjWyt/MLmLgQMHqkWLFpaf4+aPjh49qn79+mnPnj2y2Wy57lxvtX+Tn332mePPZ8+e1UsvvaSoqKg8b6bqzt/TFBY4+eqrr3TvvfcqNDRU4eHhkqQtW7bo0KFD+vjjj9WzZ0+TExYsMzNTY8eO1Ycffqjz58/nWm+1HzTSlUsoDcPQqFGj5O/vn2vuGCvOm1DYK1JWrFhRzElc5+HhUajtrFYW3XFSREmaPHmy3nzzTXXp0kWtW7dWhQoVnNZbccK73r17y9PTU3PnzlVwcLC2bNmi8+fPa/To0XrjjTcsdyTOXb+nXUVhKSYhISHaunWrqlWr5rQ8JSXFMQeBVZ04cULvvPOO0/1K/vGPfzhdvmpVw4cP15o1a/Tyyy/rkUce0axZs3Ty5Em9++67eu211/TQQw+ZHTGXihUravv27Za+pPbPoqKiCrXd+++/X8xJbhzuOCmi5J53I/fz89Pq1avVrFkz2e12bdmyRQ0aNNDq1as1evRoy94LrtQz4cqkG4LNZsvzcs+kpCTDy8vLhEQ3hqCgIGPNmjWGYRhGpUqVjEOHDhmGYRiLFi0yevToYWKy/HXu3NlYtWqV2TFKvU2bNhmff/6507KFCxcadevWNapXr24MHTrUuHjxoknprq1ixYrGzp07zY5xQ6hcubJx9OhRwzAMIyQkxFi9erVhGIZx+PBho1y5cmZGy1dcXJzRsGFDIzU1Nde6lJQUo1GjRsb69etNSFZ0GHRbxP54LvGbb76R3W53PM/OzlZcXJzq1q1rQrLC+eOESH9ks9nk4+Oj2rVrW3ayJ+nKZctXB5v5+vo6LmPu2LGjZae4nzt3rv7xj3/o5MmTatKkSa5zzlacmModvfTSS+rcubPuuusuSdKePXs0ePBgDRo0SA0bNtQ///lPBQYG6sUXXzQ3aD7ccVJE6crX/Zlnnsl1ie1vv/2mf/7zn5a8n1CTJk20a9cuBQcHKzw8XFOnTpWXl5fmzJlj2cGs06dP19ChQ/Mcp2e32/X4449r2rRpljud5RKzG1Np8+eJhf748PLyMurXr5/rtzwr+eMkcn98L1cf3t7exoABA4zffvvN7Kh5atq0qbF27VrDMAyjS5cuxujRow3DMIwZM2YYtWrVMjNavuLj443g4GC3mZjKXQUEBBhbt251PH/++eeNDh06OJ5/+OGHRsOGDc2IVijuOCmiYbjn5IKxsbHGxx9/bBiGYRw8eNBo0KCBYbPZDD8/P+O7774zOV3eateubezduzff9fv27TOCgoJKMFHR4whLEbt6SWpwcLC2bt0qPz8/kxO55pNPPtHYsWM1ZswYtW3bVtKVQbdvvvmmJk6cqN9//13PPfecxo8frzfeeMPktLlFRUVp165d6tSpk5577jn17t1bb7/9ti5fvmzZ+zc9+uijatmypT744IM8B92iaPzyyy/y9/d3PF+3bp169OjheH7LLbfoxIkTZkQrlAceeEC//vqr6tWr5zaTIkr/u9rtz3bt2qWqVauakOjaIiMjHX8OCwvT/v37deHCBVWpUsWy/z6Tk5NzfU/8UZkyZXT27NkSTFT0KCzF5NixY2ZHuC6vvPKKZsyY4fQPtmnTprrppps0YcIEbdmyRRUqVHCMlreaP146GRERof3792v79u0KDQ217KmVn376SZ999lmueUFQtPz9/XXs2DEFBQXp0qVL2rFjhyZNmuRYn56eXuAPfLNNnz7d7AguufrhbrPZVL9+facP+uzsbGVkZOgf//iHiQlzK8zVb2XKlFFAQIC6du1qqZl6a9WqpR9//DHfnyO7d+9WzZo1SzhV0aKwFLH4+HidP3/ecZ5ckhYtWqSJEycqMzNTffv21b/+9S/LjgPZs2dPnnPE1KlTR3v27JEktWjRQqdPny7paNd0+fJlde/eXbNnz1ZYWJikK7mtOufNVXfeead27dpFYSlmPXv21HPPPafXX39dK1euVPny5Z3O5+/evVv16tUzMWHB3G1SxOnTp8swDD366KOaNGmS03g+Ly8v1a1b13H7D6v4Y8b85OTk6NChQ5o7d66eeeaZXLd4MEvPnj01YcIEde/eXT4+Pk7rfvvtN02cONHpc8kdcVlzEevRo4c6d+6ssWPHSrpSAFq1auU0sO/xxx+37MC+li1bqnnz5pozZ45j9tLLly9r6NCh2rVrl3bu3KmNGzfq4YcftuRRpOrVqzsm6HMXc+bM0eTJk/Xoo4+WuomerOTcuXO65557tGHDBlWsWFELFy5Uv379HOu7dOmidu3a6ZVXXjExZeG4y6SI0pVTbx06dFCZMqXr9+MvvvhCTzzxhBITE82OIunKKaFWrVrJ09NTI0aMcEyTsH//fs2aNUvZ2dnasWOH02lRt2PuEJrSx90H9m3cuNGoVq2aUb16daNLly5Gly5djBo1ahjVqlUz4uPjDcO4conw1KlTTU6at6eeesqyd4DNz7XuCouilZKSYvz++++5lp8/f97IysoyIVHhZGRkGMOHDzeqV6/uVndS3759u7F7927H85UrVxp9+vQxxo0bZ+mv97X88ssvRr9+/cyO4eT48eNGjx49cl000aNHD8dl2u6MIyxFzMfHR4cOHXJMstaxY0f16NFDL7zwgqQrd0Nu2rSp0tPTzYxZoPT0dP33v//VwYMHJV2Zrv/vf/+7W0y//uSTT2rRokUKCwvLc1ZNqw68Ba7FHSdFlK4MZn7uued077336ujRo2rUqJHuuecebd26Vb169XK7sTnu4JdfftHhw4dlGIbCwsJUpUoVsyMVCQpLEatTp44WL16s22+/XZcuXVLlypX1+eefq0uXLpKunCLq1KmTZUf0u6ujR4+qbt26jq9zXmw2m1avXl2Cqa7t8uXLKleunBISEtSkSROz48DCateurUWLFqlz587y9fXVjh07FBoaqsWLF+uDDz7QV199ZXbEPNntdu3YsUP16tXT66+/rtWrV+ubb77Rxo0b9eCDD1r6yixYS+k6qWgB7j6wT5IOHTqkNWvW6MyZM7nuHGzFSZ6kK5cenj59WmvWrJF05RLQmTNnWv58bdmyZVW7dm23vr8HSoY7ToooXbms+erPke+++84x8DMoKEjnzp0zMxrcDIWliL388su655571KlTJ8fAvquDVyVp/vz56tatm4kJC/bee+9p2LBh8vPzU0BAgNOliDabzbKF5c8HCr/++mtlZmaalMY1L7zwgp5//nktXrzYsvNSwHwhISE6duyYateurZtvvlkffvih2rZtq88//1yVK1c2O16+2rRpo8mTJysiIkLr1q3TO++8I+nK1A9W/4UC1sIpoWKSmpqqihUrytPT02n5hQsXVLFiRacSYyV16tTRE0884bjKyV14eHgoKSlJNWrUkCRVqlRJu3btsuw02n/UsmVLHT58WJcvX1adOnVyjbvZsWOHSclgJW+99ZY8PT01cuRIfffdd+rdu7cMw9ClS5f01ltvadSoUWZHzNPu3bv10EMPKTExUdHR0Zo4caKkK+PNzp8/ryVLlpicEO6CwgInvr6+SkhIcIsP+j/y9PRUUlKSqlevLulKYdm9e3eBd4q1ij9OXpaXqz/ggT/66aeftH37doWFhalp06Zmx3HZxYsX5enpaenJ+mAtFBY4GTx4sG655RbLzUB5LR4eHurRo4djQr7PP/9cd955Z66jFStWrDAjHnDdVq9erREjRmjz5s255lpJTU3VrbfeqtmzZ7v3Te2AQmAMC5yEhoZqwoQJ2rx5c56TmI0cOdKkZAX78yygDz/8sElJrk9KSoqWL1+uI0eOaMyYMapatapjkqdatWqZHQ8mcve78Hp4eBR4/x0GnKOwOMICJwWdQrHZbDp69GgJprkx7N69WxEREbLb7Tp+/LgOHDigkJAQjR8/XomJiVq0aJHZEWGiOnXqKDY2Vg0bNsxz/f79+9WtWzfLzLj6Z59++qnT88uXL2vnzp1auHChJk2apMGDB5uUDO6GwgKYLCIiQq1atdLUqVOdBgtv2rRJf//733X8+HGzI8JEPj4+Bd7U7vDhw2ratKl+++23Ek721yxZskTLli3LVWiA/HBKqAh99tlnhd6W+8Pgqq1bt+rdd9/NtbxWrVpKSkoyIRGspLTehbddu3Z67LHHzI4BN0JhKUJ9+/Z1em6z2ZzmB/nz7dWtIjo6Wi+//LIqVKig6OjoArdlavui5+3trbS0tFzLDx486LjqCTeu0ngX3t9++00zZ85kfBZcQmEpQn+cFfa7777T2LFj9eqrrzpuoR4fH6/x48fr1VdfNStinnbu3KnLly87/oySdffdd+ull17Shx9+KOlKsU1MTNTYsWN17733mpwOZhs/frxWrFih+vXr53sX3qv3KrOiKlWqOP2yZhiG0tPTVa5cOf33v/81MRncDWNYikmTJk00e/ZsdezY0Wn5999/r8cee0z79u0zKdn1S09Pd4sbILqb1NRU/e1vf9O2bduUnp6uwMBAJSUlqV27dvr6669zXZqNG89PP/2kYcOG6ZtvvnEctbXZbIqMjNSsWbMsPd/QwoULnZ57eHioevXqCg8P18mTJ7mHFgqNwlJMypUrp61bt+b6x7h7926Fh4dbboDcW2+9paeffjrf9enp6erevbs2btxYgqluLBs3btSuXbuUkZGhVq1aKSIiwuxIsJjScBfe9PR0ffDBB5o3b562bdtmqdPjsDYKSzG5/fbb5ePjo8WLFzvul5GcnKwBAwbo4sWLWrdunckJnZUrV07vvvuuBgwYkGtdRkaGIiMjdf78ee3fv9+EdKXTb7/9pri4OMf4g3HjxikrK8uxvkyZMnrppZdyjVsA3NH69es1b948ffzxxwoMDNQ999yje++9V7fccovZ0eAmGMNSTObPn69+/fqpdu3aCgoKkiSdOHFCYWFhWrlypbnh8rB48WI98sgjqly5stMVTJmZmerevbvOnj1ruZLl7hYuXKgvv/zSUVjefvttNW7cWOXKlZN0ZYxCzZo1CzzyBVhZUlKSFixYoHnz5iktLU3333+/srKytHLlSjVq1MjseHAzHGEpRoZhaNWqVY6jEg0bNlRERESBsz6aae7cuRo1apS+/PJLde7c2VFWkpKStG7dOgUGBpodsVS57bbb9Oyzz6p3796Sct+w8T//+Y9mzZql+Ph4M2MC16V3795av369evXqpYceekjdu3d33Dto165dFBa4jCMsxchms6lbt266/fbb5e3tbdmictWQIUN04cIF9enTR59++qliYmJ06tQpykoxuTrh11U+Pj7y8PBwPG/btq2GDx9uRjTgL/v66681cuRIDRs2TGFhYWbHQSngce1NcD1ycnL08ssvq1atWqpYsaKOHTsmSZowYYLmzZtncrr8Pfvssxo2bJi6dOmikydPau3atbrpppvMjlUqpaSkOI1ZOXv2rOrWret4npOT47QecCcbNmxQenq6WrdurfDwcL399ts6d+6c2bHgxigsxWTy5MlasGCBpk6dKi8vL8fyJk2aaO7cuSYmy9s999zjeBw8eFBly5aVn5+fRo0a5bQOReemm27Sjz/+mO/63bt3Uxbhttq1a6f33ntPp0+f1uOPP66lS5cqMDBQOTk5WrVqldLT082OCDfDGJZiEhoaqnfffVddunRxGpuwf/9+tW/fXr/88ovZEZ1ERUUVarv333+/mJPcOEaNGqXvvvtO27dvz3MG0zZt2igiIkIzZswwKSFQtA4cOKB58+Zp8eLFSklJUdeuXV26pQlubBSWYlKuXDnt379fderUcSose/fuVdu2bZWRkWF2RJgsOTlZLVq0kJeXl0aMGKH69etLuvJD/e2339bvv/+unTt3Oi6LB0qL7Oxsff7555o/fz6FBYXGoNti0qhRI33//feqU6eO0/Lly5erZcuWJqWClfj7+2vTpk0aNmyYnnvuOacZTLt27ap///vflBWUSp6enurbt2+u+68BBaGwFJOYmBgNHDhQJ0+eVE5OjlasWKEDBw5o0aJF+uKLL8yOB4sIDg5WbGysLly4oMOHD0u6cjqxatWqJicDAGvhlFAx+v777/XSSy85TbceExOjbt26mR0NAAC3QmEBAACWx2XNxSQkJETnz5/PtTwlJcUxkykAACgcxrAUk+PHj+d5F9KsrCydPHnShET5c2WU/h/vMwQAQEmhsBSxP374f/PNN7Lb7Y7n2dnZiouLc5rN1Ar+PFLfZrPpj2cK/3hLAW4FDwAwA2NYitjVe8H8+UNfksqWLau6devqzTffdNyh12q+++47jR07Vq+++qrat28vSYqPj9f48eP16quvqmvXriYnBADciCgsxSQ4OFhbt26Vn5+f2VFc0qRJE82ePVsdO3Z0Wv7999/rscce0759+0xKBgC4kXFKqJhcvdmhuzly5IgqV66ca7ndbtfx48dLPA8AABJHWIrUzJkz9dhjj8nHx0czZ84scNuRI0eWUCrX3H777fLx8dHixYsds6wmJydrwIABunjxotatW2dyQgDAjYjCUoSCg4O1bds2VatWTcHBwfluZ7PZdPTo0RJMVniHDx9Wv379dPDgQQUFBUmSTpw4obCwMK1cuVKhoaEmJwQA3IgoLMjFMAytWrVK+/fvlyQ1bNhQERERTlcLAQBQkigsyNfFixfl7e1NUQEAmI5Bt8UkOztbCxYsUFxcnM6cOaOcnByn9atXrzYpWcFycnL0yiuvaPbs2UpOTtbBgwcVEhKiCRMmqG7duho8eLDZEQEANyCm5i8mo0aN0qhRo5Sdna0mTZqoefPmTg+rmjx5shYsWKCpU6fKy8vLsbxJkyaaO3euickAADcyTgkVEz8/Py1atEg9e/Y0O4pLQkND9e6776pLly6qVKmSdu3apZCQEO3fv1/t27fXL7/8YnZEAMANiCMsxcTLy8str6g5efJknrlzcnJ0+fJlExIBAEBhKTajR4/WjBkzck3Pb3WNGjXS999/n2v58uXL1bJlSxMSAQDAoNtis2HDBq1Zs0Zff/21GjdurLJlyzqtX7FihUnJChYTE6OBAwfq5MmTysnJ0YoVK3TgwAEtWrRIX3zxhdnxAAA3KMawFJOoqKgC17///vsllMR133//vV566SXt2rVLGRkZatWqlWJiYtStWzezowEAblAUFgAAYHmMYYGTkJAQnT9/PtfylJQUhYSEmJAIAADGsBS5KlWq5DkzrN1uV/369fXMM8+oa9euJiQrnOPHjys7OzvX8qysLJ08edKERAAAUFiK3PTp0/NcnpKSou3bt+uuu+7S8uXL1bt375INdg2fffaZ48/ffPON7Ha743l2drbi4uJUt25dE5IBAMAYlhI3bdo0LV++XJs2bTI7ihMPjytnB202W65LscuWLau6devqzTff1F133WVGPADADY7CUsIOHjyodu3a6cKFC2ZHyVNwcLC2bt0qPz8/s6MAAODAKaESlpWV5XSPHqs5duyY2REAAMiFwlLC5s2bpxYtWpgdw8nMmTP12GOPycfHRzNnzixw25EjR5ZQKgAA/odTQkUsOjo6z+WpqanasWOHDh48qPXr16t169YlnCx/wcHB2rZtm6pVq6bg4OB8t7PZbDp69GgJJgMA4AoKSxG744478lzu6+urBg0aaNiwYQWWAgAAkBuFBQAAWB5jWOAkOztbCxYsUFxcnM6cOaOcnByn9atXrzYpGQDgRkZhgZNRo0ZpwYIF6tWrl5o0aZLnrL0AAJQ0TgnBiZ+fnxYtWqSePXuaHQUAAAdufggnXl5eCg0NNTsGAABOKCxwMnr0aM2YMSPX9PwAAJiJU0Jw0q9fP61Zs0ZVq1ZV48aNVbZsWaf1K1asMCkZAOBGxqBbOKlcubL69etndgwAAJxwhAUAAFgeY1gAAIDlcUoIkqQqVarkOeeK3W5X/fr19cwzz6hr164mJAMAgFNC+P8WLlyY5/KUlBRt375dy5Yt0/Lly9W7d+8STgYAAIUFhTRt2jQtX75cmzZtMjsKAOAGRGFBoRw8eFDt2rXThQsXzI4CALgBMegWhZKVlSUvLy+zYwAAblAUFhTKvHnz1KJFC7NjAABuUFwlBElSdHR0nstTU1O1Y8cOHTx4UOvXry/hVAAAXEFhgSRp586deS739fVV165dtWLFCgUHB5dwKgAArmDQLQAAsDzGsAAAAMujsAAAAMujsAAAAMujsAAAAMujsAAAAMujsAAAAMujsAAAAMujsAAAAMv7f1chxJiGo1adAAAAAElFTkSuQmCC)



Out[ ]:


```
''
```









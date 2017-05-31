# Sublime Text setting

install Sublime Text package control

[package control](https://packagecontrol.io/installation)

-
### 常用插件
- Babel
- ES6-Toolkit（ES6代码提示)
- DocBlokr（代码注释/** -> tab）
- sass
- HTML-CSS-JS Prettify （格式化）
- jsfmt
- CSScomb （css属性顺序格式化）
- SublimeTmpl（template）
- JavaScript & NodeJS Snippets (js代码提示)
- emmet

---
### react环境搭建
- React ES6 Snippets
- React and React Router Snippets
- emmet（html -> tab; js -> command+e)
<pre>
//配置
//打开菜单 preferences -> Key bindings - Users
[{
    "keys": ["super+e"],
    "command": "expand_abbreviation_by_tab",
    "context": [{
        "operand": "source.js",
        "operator": "equal",
        "match_all": true,
        "key": "selector"
    },
    {
        "match_all": true,
        "key": "selection_empty"
    }, 
    {
        "operator": "equal",
        "operand": false,
        "match_all": true,
        "key": "has_next_field"
    },
    {
        "operand": false,
        "operator": "equal",
        "match_all": true,
        "key": "auto_complete_visible"
    }, {
        "match_all": true,
        "key": "is_abbreviation"
    }]
}]
</pre>

- jsfmt
<pre>
//配置
//打开菜单Preferences -> Package Settings -> Sublime JSFMAT -> Settings - User，将下面代码贴进去保存。
{
    "autoformat": false,
    "extensions": ["js", "sublime-settings"],
    "options": {
        "preset": "jquery",
        "indent": {
            "value": "    "
        },
        // plugins included
        "plugins": [
            // "esformatter-quotes",
            // "esformatter-semicolons",
            // "esformatter-braces",
            // "esformatter-dot-notation"
        ]
    },
    "options-JSON": {
        "plugins": [
            "esformatter-quotes"
        ],
        "quotes": {
            "type": "double"
        }
    },
    "alert-errors": true,
    "node-path": "node",
    "ignore-selection": false
}
</pre>
<pre>
//快捷键设置 Preferences -> Key Bindings - User
{"keys":["ctrl+q"],"command":"format_javascript"}
</pre>
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
- jsformat
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

- jsformat
<pre>
//配置
//打开菜单Preferences -> Package Settings -> JsFormat -> Settings - User，将下面代码贴进去保存。
{
    "e4x": true,
    // jsformat options
    "format_on_save": true,
}
</pre>
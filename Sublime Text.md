# Sublime Text setting

install Sublime Text package control

[package control](https://packagecontrol.io/installation)

-

command + shift + p  install

- ES6-Toolkit（ES6代码提示)
- DocBlokr（代码注释/** -> tab）
- sass
- HTML-CSS-JS Prettify （格式化）
- SublimeTmpl（template）
- emmet（html -> tab; js -> command+e)
<pre>
//配置
//打开菜单Preferences -> Package Settings -> Emmet -> Key Bindings - User
[{
    "keys": ["tab"],
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
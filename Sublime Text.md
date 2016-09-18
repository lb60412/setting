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
{
    "keys": ["super+e"],
    "command": "expand_abbreviation_by_tab",
    // put comma-separated syntax selectors for which 
    // you want to expandEmmet abbreviations into "operand" key 
    // instead of SCOPE_SELECTOR.
    // Examples: source.js, text.html - source
    "context": [{
            "operand": "source.js",
            "operator": "equal",
            "match_all": true,
            "key": "selector"
        },
        // run only if there's no selected text
        {
            "match_all": true,
            "key": "selection_empty"
        },
        // don't work if there are active tabstops
        {
            "operator": "equal",
            "operand": false,
            "match_all": true,
            "key": "has_next_field"
        },
        // don't work if completion popup is visible and you
        // want to insert completion with Tab. If you want to
        // expand Emmet with Tab even if popup is visible -- 
        // remove this section
        {
            "operand": false,
            "operator": "equal",
            "match_all": true,
            "key": "auto_complete_visible"
        }, {
            "match_all": true,
            "key": "is_abbreviation"
        }
    ]
}
</pre>

- jsformat
<pre>
{
    "e4x": true,
    // jsformat options
    "format_on_save": true,
}
</pre>
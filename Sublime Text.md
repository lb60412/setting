# Sublime Text setting

install Sublime Text package control

[package control](https://packagecontrol.io/installation)

-

### 常用插件

* Babel
* ES6-Toolkit（ES6 代码提示)
* DocBlokr（代码注释/\*\* -> tab）
* sass
* HTML-CSS-JS Prettify （格式化）
* JsPrettier
* CSScomb （css 属性顺序格式化）
* SublimeTmpl（template）
* JavaScript & NodeJS Snippets (js 代码提示)
* emmet

---

### react 环境搭建

* React ES6 Snippets
* React and React Router Snippets
* emmet（html -> tab; js -> command+e)
<pre>
//配置
//打开菜单 preferences -> Key bindings - Users
[
	{
		"keys": ["super+e"],
		"command": "expand_abbreviation_by_tab",
		"context": [
			{
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
			},
			{
				"match_all": true,
				"key": "is_abbreviation"
			}
		]
	}
]
</pre>

* JsPrettier
 <pre>// 安装
 $ npm install -g prettier
 // Sublime 安装 JsPrettier
 // 配置
 // 打开菜单 Preferences -> Package Settings -> JsPrettier -> Settings - User，将下面代码贴进去保存。
{
    "auto_format_on_save": true,
    "prettier_options":
    {
        "printWidth": 80,
        "singleQuote": true,
        "trailingComma": "none",
        "bracketSpacing": true,
        "jsxBracketSameLine": false,
        "parser": "babylon",
        "semi": false,
        "requirePragma": false,
        "proseWrap": "preserve",
        "arrowParens": "avoid"
    }
}
</pre>

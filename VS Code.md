### VUE 环境搭建

* Babel ES6/ES7
* Babel JavaScript
* Node.js Modules Intellisense
* Prettier
* Vetur
  <pre>
//配置
{
  "window.zoomLevel": 2,
  "editor.tabSize": 2,
  "editor.formatOnSave": true, // 保存自动格式化
  "extensions.ignoreRecommendations": true,
  "prettier.semi": false, // 分号
  "prettier.singleQuote": true, // 单引号
  "prettier.stylelintIntegration": true, // 格式化 style
  "vetur.format.defaultFormatter.html": "js-beautify-html",
  "vetur.format.defaultFormatterOptions": { // 格式化 HTML
    "js-beautify-html": {
      "wrap_attributes": "force"
    }
  },
}
  </pre>

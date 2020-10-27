# vue3-admin

## 目标
- 熟练使用git
- 使用vue3, 学会vue3相关语法(比vue2多一些api, 其他基本类似)
- 学会typescript的使用
- 学会封装一些基本的api

## src中各个文件夹用途
assets: 存放图片资源
components: 存放通用的组件
router: 存放路由配置文件
store: 存放状态管理文件
utils: 存放封装的工具函数
views: 存放单页应用的页面级文件

## vue开发风格指南
[点击](https://v3.vuejs.org/style-guide/#multi-word-component-names-essential)

## 开发工具

> vscode 配置

```json
{
  "workbench.iconTheme": "vscode-icons",
  "vsicons.associations.folders": [
    { "icon": "api", "extensions": ["apis", "api"] },
    { "icon": "redux", "extensions": ["store"] },
    {
      "icon": "route",
      "extensions": ["route", "routes", "_route", "_routes", "routers", "router"]
    },
    { "icon": "middleware", "extensions": ["middleware", "middlewares", "hook", "hooks"] }
  ],
  "todo-tree.tree.showScanModeButton": false,
  "workbench.tree.indent": 12,
  "window.menuBarVisibility": "toggle",
  "editor.tabSize": 2,
  "editor.fontFamily": "'JetBrains Mono', Consolas,'Courier New'",
  "editor.fontWeight": "300",
  "editor.dragAndDrop": false,
  "editor.foldingStrategy": "indentation",
  "editor.glyphMargin": false,
  "editor.hover.delay": 300,
  "editor.overviewRulerBorder": false,
  "editor.renderLineHighlight": "all",
  "editor.scrollBeyondLastLine": true,
  "editor.wordWrapColumn": 100,
  "editor.wordWrap": "wordWrapColumn",
  "editor.cursorBlinking": "phase",
  "editor.fontLigatures": true,
  "editor.minimap.maxColumn": 80,
  "editor.minimap.renderCharacters": false,
  "editor.minimap.showSlider": "always",
  "editor.suggest.statusBar.visible": true,
  "files.trimTrailingWhitespace": true,
  "workbench.startupEditor": "none",
  "workbench.editor.labelFormat": "short",
  "breadcrumbs.enabled": false,
  "workbench.editor.limit.enabled": true,
  "workbench.editor.limit.perEditorGroup": true,
  "window.titleSeparator": " 🦄 ",
  "explorer.openEditors.visible": 6,
  "explorer.sortOrder": "type",
  "[typescriptreact]": {
    "editor.defaultFormatter": "esbenp.prettier-vscode"
  },
  "[javascript]": {
    "editor.defaultFormatter": "esbenp.prettier-vscode"
  },
  "prettier.printWidth": 100, // 超过最大值换行
  "prettier.tabWidth": 2, // 缩进字节数
  "prettier.useTabs": false, // 缩进不使用tab，使用空格
  "prettier.semi": false, // 句尾不加分号
  "prettier.singleQuote": true, // 使用单引号代替双引号
  "prettier.bracketSpacing": true, // 在对象，数组括号与文字之间加空格 "{ foo: bar }"
  "prettier.jsxBracketSameLine": false, // 在jsx中把'>' 是否单独放一行
  "prettier.jsxSingleQuote": true, // 在jsx中使用单引号代替双引号
  "bracketPairColorizer.consecutivePairColors": [
    "()",
    "[]",
    "{}",
    ["cadetblue", "Orchid", "LightSkyBlue"],
    "Red"
  ],
  "todo-tree.highlights.customHighlight": {
    "TODO": {
      "icon": "dashboard",
      "type": "text",
      "foreground": "white",
      "background": "green",
      "iconColour": "cadetblue",
      "gutterIcon": false
    },
    "BUG": {
      "icon": "alert",
      "iconColour": "red",
      "background": "red",
      "foreground": "white",
      "type": "text"
    }
  },
  "[html]": {
    "editor.defaultFormatter": "esbenp.prettier-vscode"
  },
  "[typescript]": {
    "editor.defaultFormatter": "esbenp.prettier-vscode"
  },
  "prettier.trailingComma": "none",
  "git.enableSmartCommit": true,
  "git.confirmSync": false,
  "git.autofetch": true,
  "workbench.list.openMode": "doubleClick",
  "window.doubleClickIconToClose": true,
  "window.zoomLevel": 0,
  "workbench.colorTheme": "One Dark Pro",
  "terminal.integrated.fontFamily": "'JetBrains Mono', Consolas,'Courier New'",
  "workbench.colorCustomizations": {
    "[One Dark Pro]": {}
  },
  "workbench.list.smoothScrolling": true,
  "[jsonc]": {
    "editor.defaultFormatter": "esbenp.prettier-vscode"
  },
  "terminal.integrated.macOptionClickForcesSelection": true,
  "[vue]": {
    "editor.defaultFormatter": "esbenp.prettier-vscode"
  },
  "[markdown]": {
    "editor.wordWrap": "on",
    "editor.quickSuggestions": true,
    "editor.defaultFormatter": "fcrespo82.markdown-table-formatter"
  },
  "leetcode.endpoint": "leetcode-cn",
  "leetcode.workspaceFolder": "C:\\Users\\WHJ12037\\.leetcode",
  "explorer.confirmDragAndDrop": false,
  "explorer.compactFolders": false,
  "explorer.confirmDelete": false,
  "vsicons.dontShowNewVersionMessage": true,
  "[json]": {
    "editor.defaultFormatter": "esbenp.prettier-vscode"
  },
  "vetur.validation.template": false,
  "go.formatTool": "goreturns",
  "go.docsTool": "gogetdoc",
"go.autocompleteUnimportedPackages": true,
  "go.testFlags": ["-v", "-count=1"],
  "go.useCodeSnippetsOnFunctionSuggest": false,
  "go.useLanguageServer": true,
  "typescript.format.semicolons": "remove",
  "javascript.format.semicolons": "remove",
  "typescript.preferences.importModuleSpecifierEnding": "minimal",
  "path-autocomplete.pathMappings": {
    "@": "${folder}/src"
  },
  "jsannotations.hideInvalidAnnotation": false,
  "editor.suggestSelection": "first",
  "vsintellicode.modify.editor.suggestSelection": "automaticallyOverrodeDefaultValue",
  "editor.tokenColorCustomizations": {
    "textMateRules": [
      {
        "name": "jetbrains mono italic",
        "settings": {
          "fontStyle": "italic"
        },
        "scope": [
          "comment",
          "constant",
          "keyword",
          "entity.name.type.class",
          "storage.modifier",
          "storage.type.class.js",
        ]
      }
    ]
  },
  "debug.console.fontFamily": "'JetBrains Mono', Consolas,'Courier New'",
  "[javascriptreact]": {
    "editor.defaultFormatter": "esbenp.prettier-vscode"
  },
  "gitlens.views.repositories.files.layout": "list"
}
```

> vscode 插件

1. Gitlens
2. Path Autocomplete
3. Prettier
4. Todo Tree
5. Vetur
6. Visual Studio IntelliCode
7. vscode-icons


> vscode 字体

[JetBrains Mono](https://www.jetbrains.com/lp/mono/)
# Awesome Angular Pack

A collection of useful, stable and best rated angular/typescript extensions, which build a productive IDE. If you are also a dotnetcore developer check out the [Awesome Dotnetcore Pack](https://marketplace.visualstudio.com/items?itemName=salbert.awesome-dotnetcore-pack), which reuses packages that offer support for both environments.

## Angular

- [VSCode Angular TypeScript & Html Snippets](https://marketplace.visualstudio.com/items?itemName=Mikael.Angular-BeastCode)
  Visual Studio Code TypeScript and Html snippets and code examples for Angular 2,4,5 & 6. All code snippets are based on and follow the [Angular style guide](https://angular.io/docs/ts/latest/guide/style-guide.html).

- [Angular Schematics](https://marketplace.visualstudio.com/items?itemName=cyrilletuzi.angular-schematics)
  Angular schematics (CLI commands) from files Explorer or Command Palette.

- [Angular2 Switcher](https://marketplace.visualstudio.com/items?itemName=infinity1207.angular2-switcher)
  Easily navigate to typescript(.ts)|template(.html)|style(.scss/.sass/.less/.css) in angular2 project.

- [Angular Support](https://marketplace.visualstudio.com/items?itemName=vismalietuva.vscode-angular-support)
  Very lightweight language support for angular definitions.

- [Material Icon Theme](https://marketplace.visualstudio.com/items?itemName=PKief.material-icon-theme)
  The Material Icon Theme provides lots of icons based on Material Design for Visual Studio Code. It include seperate icon for example Angular-Services, Angular-Components, Angular-Directives,....

## Typescript

- [ESLint](https://marketplace.visualstudio.com/items?itemName=dbaeumer.vscode-eslint)
  Integrates ESLint into VS Code. TSLint is deprecated. [Migration](https://code.visualstudio.com/api/advanced-topics/tslint-eslint-migration)

- [Move TS README](https://marketplace.visualstudio.com/items?itemName=stringham.move-ts)
  Supports moving typescript files and updating relative imports within the workspace.

- [Paste JSON as Code](https://marketplace.visualstudio.com/items?itemName=quicktype.quicktype)

- [Todo Tree](https://marketplace.visualstudio.com/items?itemName=Gruntfuggly.todo-tree)
  Show TODO, FIXME, etc. comment tags in a tree view

- [Comment TS](https://marketplace.visualstudio.com/items?itemName=salbert.comment-ts)
  "Comment TS" generates a template for JSDoc comments. It is adapted for TypeScript files. Typescript comes with a lot of language annotations, which should not be duplicated in the comments. Most likely this would lead to inconsistencies. If you like a todo in your generated comments:

```
"comment-ts.todoComments": true,
```

## HTML

- [IntelliSense for CSS class names in HTML](https://marketplace.visualstudio.com/items?itemName=Zignd.html-css-class-completion)
  CSS class name completion for the HTML class attribute based on the definitions found in your workspace.

- [Auto Rename Tag](https://marketplace.visualstudio.com/items?itemName=formulahendry.auto-rename-tag)
  Automatically rename paired HTML/XML tag, same as Visual Studio IDE does.

## NPM

- [Node npm](https://marketplace.visualstudio.com/items?itemName=eg2.vscode-npm-script)
  This extension validates the installed modules against the dependencies defined in the package.json.

- [Version Lens](https://marketplace.visualstudio.com/items?itemName=pflannery.vscode-versionlens)
  Shows package version information for npm, jspm, bower, dub and dotnet core in the Visual Studio Code editor.

## Code formatting

- [Prettier formatter for Visual Studio Code](https://marketplace.visualstudio.com/items?itemName=esbenp.prettier-vscode)
  VS Code package to format your JavaScript / TypeScript / CSS using Prettier. Configure your preferences in a ".prettierrc" file:

```
{
   "printWidth": 150,
   "singleQuote": true,
   "arrowParens": "always"
}
```

- [EditorConfig](https://marketplace.visualstudio.com/items?itemName=EditorConfig.EditorConfig)
  This plugin attempts to override user/workspace settings with settings found in .editorconfig files. No additional or vscode-specific files are required. As with any EditorConfig plugin, if root=true is not specified, EditorConfig will continue to look for an .editorconfig file outside of the project.

## Dev Tools

- [GitLens](https://marketplace.visualstudio.com/items?itemName=eamodio.gitlens)
  GitLens supercharges the Git capabilities built into Visual Studio Code. It helps you to visualize code authorship at a glance via Git blame annotations and code lens, seamlessly navigate and explore Git repositories, gain valuable insights via powerful comparison commands, and so much more. If you don't like the gitlens on the current line set:

```
"gitlens.currentLine.enabled": false
```

- [Path Intellisense](https://marketplace.visualstudio.com/items?itemName=christian-kohler.path-intellisense)
  Visual Studio Code plugin that autocompletes filenames.

- [Copy text](https://marketplace.visualstudio.com/items?itemName=salbert.copy-text)
  Offers more copy options: Copies text without syntax highlighting, optionally adds metainfo like document name and date.

- [Online help](https://marketplace.visualstudio.com/items?itemName=salbert.online-help)
  Offers context sensitive online help.

## Recommended Tools (not included)

- [Import cost](https://marketplace.visualstudio.com/items?itemName=wix.vscode-import-cost)
  Display import/require package size in the editor

- [Better Comments](https://marketplace.visualstudio.com/items?itemName=aaron-bond.better-comments)
  With this extension, you will be able to categorise your annotations into: Alerts, Queries, TODOs, Highlights,...
  Commented out code can also be styled to make it clear the code shouldn't be there.

- [Compodoc](https://compodoc.github.io/website/)
  Generate your Angular project documentation in seconds.

- [TypeDoc](http://typedoc.org/guides/installation/)
  A documentation generator for TypeScript projects.

- [Angular/Karma Test Explorer](https://marketplace.visualstudio.com/items?itemName=raagh.angular-karma-test-explorer&ssr=false#review-details)
  Run your Angular Tests in the Sidebar of Visual Studio Code

## Settings Tipps

- If you do not like vs code telemetry set:

```
"telemetry.enableTelemetry": false
```

- All NPM scripts to start in the explorer view:

```
"npm.enableScriptExplorer": true
```

- Organize imports on file save:

```
"[typescript]": {
    "editor.codeActionsOnSave": {
        "source.organizeImports": true
    }
}
```

- If you do not need 'open editors' and like to use the space for your project files:

```
"explorer.openEditors.visible": 0
```

- Auto save on leaving the editor:

```
"files.autoSave": "onFocusChange"
```

- Enhanced minimap performance by disabling render characters in minimap:

```
"editor.minimap.renderCharacters": false
```

- Bracket colorization

```
    "editor.bracketPairColorization.enabled": true,
    "editor.guides.bracketPairs":"active"
```

- Makes the corresponding js and source map files invisible:

```
"files.exclude": {
    "**/*.js": {
        "when": "$(basename).ts"
    },
    "**/*.js.map": true
}
```

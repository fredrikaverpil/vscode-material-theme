# Material Theme for vscode

This is a direct conversion of the excellent Material Theme by [Mattia Astorino](https://github.com/equinusocio), downloaded from the [tmTheme Editor](http://tmtheme-editor.herokuapp.com/#!/editor/theme/Material%20Theme) and [converted through Yeoman](https://code.visualstudio.com/Docs/customization/themes#_adding-a-new-theme) into a vscode extension.

## Screenshot

![Screenshot](https://cloud.githubusercontent.com/assets/994357/20610669/042cc31a-b29d-11e6-9657-87427ceb9e6a.png)


## Github source

[https://github.com/fredrikaverpil/vscode-material-theme](https://github.com/fredrikaverpil/vscode-material-theme)


## Visual Studio Marketplace

[https://marketplace.visualstudio.com/items?itemName=fredrikaverpil.vscode-material-theme](https://marketplace.visualstudio.com/items?itemName=fredrikaverpil.vscode-material-theme)


## Notes on updating the theme


#### Clone this repository

```bash
git clone https://github.com/fredrikaverpil/vscode-material-theme.git
cd vscode-material-theme
```

#### Download the latest version of the theme

```bash
curl -o themes/material-theme.tmTheme https://raw.githubusercontent.com/equinusocio/material-theme/develop/schemes/Material-Theme.tmTheme
```

#### Install and run Yo Code

Offical Yo code docs: [https://code.visualstudio.com/docs/tools/yocode](https://code.visualstudio.com/docs/tools/yocode)

Please note, this step is not needed to follow as the git repo already holds all of the data which Yo Code generates, but it's here for completeness:

```bash
npm install -g yo generator-code
yo code
```

#### Finalize update

* Bump the version number in `package.json`
* Add notes on the update in `CHANGELOG.md`
* Commit and push all changes to git repository.


#### Publish extension onto the Visual Studio Marketplace

Official vsce docs: [https://code.visualstudio.com/docs/tools/vscecli](https://code.visualstudio.com/docs/tools/vscecli)

```bash
npm install -g vsce
vsce publish
```

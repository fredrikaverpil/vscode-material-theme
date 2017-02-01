# Material Theme for vscode

[![](https://vsmarketplacebadge.apphb.com/version-short/fredrikaverpil.vscode-material-theme.svg)](https://marketplace.visualstudio.com/items?itemName=fredrikaverpil.vscode-material-theme)
[![](https://vsmarketplacebadge.apphb.com/installs-short/fredrikaverpil.vscode-material-theme.svg)](https://marketplace.visualstudio.com/items?itemName=fredrikaverpil.vscode-material-theme)
[![The MIT License](https://img.shields.io/github/license/mashape/apistatus.svg)](http://opensource.org/licenses/MIT)


This theme is directly based on the excellent Material Theme by [Mattia Astorino](https://github.com/equinusocio) without any modifications.

**Please note**: The theme is, as of writing this, not rendered as intended in vscode (1.8). The current Insider build (1.9) does render it correctly and we should enjoy this soon in the stable build of vscode.


## Screenshot

![Screenshot](https://cloud.githubusercontent.com/assets/994357/20610669/042cc31a-b29d-11e6-9657-87427ceb9e6a.png)



## Resources

* [Github source](https://github.com/fredrikaverpil/vscode-material-theme)
* [Visual Studio Marketplace page](https://marketplace.visualstudio.com/items?itemName=fredrikaverpil.vscode-material-theme)



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

#### Bump version and create update changelog

* Bump the version number in `package.json`
* Add notes on the update in `CHANGELOG.md`


#### Test extension

Official vsce docs: [https://code.visualstudio.com/docs/tools/vscecli](https://code.visualstudio.com/docs/tools/vscecli)

```bash
npm install -g vsce
vsce package  # create .vsix
code --install-extension *.vsix  # test it
mv *.vsix vsix/  # Move it into "vsix" folder
```


#### Publish to Github and Visual Studio Marketplace

```bash
git commit -am "Updated theme"
git push
```

Notes on setting up a token in the [official vsce docs](https://code.visualstudio.com/docs/tools/vscecli).

```bash
vsce publish
```

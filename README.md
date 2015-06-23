# My Dev Environment

### Xcode
* __Install:__ $`xcode-select --install`
* __Confirm install__ $`xcode-select -p`
  Should yeild /Applications/Xcode.app/Contents/Developer

### Homebrew
* __Install:__ $`ruby -e "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install)"`
* __Get installed version:__ $`brew -v`
* __Update (run before package installs):__ $`brew update`
* __Upgrade brew packages:__ $`brew upgrade`
* __Check for errors:__ $`brew doctor`
* [Homebrew site](http://brew.sh/)

### Git
* __Install:__ $`brew install git`
* __Confirm install:__ $`git --version`
* __Github for Mac download:__ [Github site](https://mac.github.com/)

### Markdown
* [Markdown basics](https://help.github.com/articles/markdown-basics/)
* [Github flavored markup (GMF)](https://help.github.com/articles/github-flavored-markdown/)
* [Language specific code highlighting](http://pygments.org/docs/lexers/) - e.g. 'bash'
* [Chrome markdown preview app](https://chrome.google.com/webstore/detail/markdown-preview/jmchmkecamhbiokiopfpnfgbidieafmd/related)
  After install, check "Allow access to file URLs" in Preferences > Extensions > Markdown Preview
Drag file into chrome

### Atom (IDE)
* __Atom download:__ [Atom site](https://atom.io/)
* [Atom package search](https://atom.io/packages)
* __Install package:__ $`apm install [package_name]`
* __Install atom packages from file:__ $`apm install --packages-file apm-package-list.txt`
* __Update atom packages file:__ $`apm list --installed --bare > apm-package-list.txt`

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
* __Add file/dir to gitignore:__ `echo venv/ >> .gitignore`

### Markdown
* [Markdown basics docs](https://help.github.com/articles/markdown-basics/)
* [Github flavored markdown (GMF) docs](https://help.github.com/articles/github-flavored-markdown/)
* [Gitbhub flavored markdown Chrome plugin](https://chrome.google.com/webstore/detail/github-flavored-markdown/faelggnmhofdamhdegcdhhemfokkfngk?hl=en)
  - In Chrome > preferences, check Allow access to file URL's to view local files
* [Language specific code highlighting docs](http://pygments.org/docs/lexers/) - e.g. 'bash'
  After install, check "Allow access to file URLs" in Preferences > Extensions > Markdown Preview
Drag file into chrome

### Atom (IDE)
* __Atom download:__ [Atom site](https://atom.io/)
* [Atom package search](https://atom.io/packages)
* __Install package:__ $`apm install [package_name]`
* __Install atom packages from file:__ $`apm install --packages-file apm-package-list.txt`
* __Update atom packages file:__ $`apm list --installed --bare > apm-package-list.txt`

### Sublime Text 3 (IDE)
* __Package control install__: Manually (https://packagecontrol.io/docs/usage)
* __Install packages__: cmd+shift+P (type 'install', 'list')
  Anaconda, SideBarEnhancements
* __Install subl command__: `sudo ln -s /Applications/Sublime\ Text.app/Contents/SharedSupport/bin/subl /usr/bin/subl`
* __Save project__: Project > Save Project As... (create PROJECT-NAME.sublime-workspace and PROJECT-NAME.sublime-project)
* __Edit project__: Edit PROJECT-NAME.sublime-project file. Include settings:
  ```json
  "settings":
  {
    "anaconda_gutter_theme": "Bright",
    "python_interpreter": "/full/path/to/project/venv/bin/python"
  }```
* __Open project with subl command line tool__: subl PROJECT-NAME.sublime-workspace
* __Preferences > Settings > User (base settings)__: Modified from [mjhea0's base settings](https://github.com/mjhea0/sublime-setup-for-python/blob/master/dotfiles/Preferences.sublime-settings)
* __Preferences > More(to create) or Browse Packages > Python.sublime-settings__: Modified from [mjhea0's Python settings](https://github.com/mjhea0/sublime-setup-for-python/blob/master/dotfiles/Python.sublime-settings)

### Pip (Python package installer)
* __Save current packages to requirements file:__ $`pip freeze > requirements.txt`
* __Publishing a package tutorial__: http://peterdowns.com/posts/first-time-with-pypi.html

### Python Virtual Environment
* __Install venv package:__ $`pip install virtualenv`
* __Create new virtual environment:__ $`virtualenv venv`
* __Enter virtual environment:__ $`source venv/bin/activate`
* __Exit virtual environment:__ $`deactivate`

# boilerplate (for HTML)
Simple node script to create a boilerplate html file.

### Installation
Install in `~/bin` to use globally (create folder if it doesn't exist and add it to your `$PATH`).

### Usage
To start a new `.html` file, type: 
```shell
$ boilerplate <htmlFileName>
```

`boilerplate` only checks if the argument has an `.html` extension (if it doesn't it will be added). It doesn't check for anything else. If the file already exists, it will be overwritten.

`boilerplate` will prompt for a page title, path to a `CSS` file, and a path to a `JS` file:
```shell
$ Enter page title (press enter to skip):
Best page ever
$ Enter path to CSS file (press enter to skip):
style.css
$ Enter path to JS file (press enter to skip):
script.js
```

Again, `boilerplate` doesn't do any file path checking.

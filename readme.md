# boilerplate (for HTML)
Simple node script to create a boilerplate html file.

### Installation
Install in `~/bin` to use globally (create folder if it doesn't exist and add it to your `$PATH`).

### Usage
To start a new `.html` file in the current directory, type: 
```shell
$ boilerplate <htmlFileName>
```

`boilerplate` checks if the argument has an `.html` extension (if not, it will be added), but **will not** check if the file already exists (always overwritten).

`boilerplate` will prompt for a page title, path to a `CSS` file, and a path to a `JS` file:
```shell
$ Enter page title (press enter to skip):
Best page ever
$ Enter path to CSS file (press enter to skip):
style.css
$ Enter path to JS file (press enter to skip):
script.js
```

If `css` and `js` files and their directories don't exist yet, they will be created recursively.

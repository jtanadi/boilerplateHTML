# boilerplate (for HTML)
Simple node script to create a boilerplate html file.

### Installation
Install in `~/bin` to use globally (create folder if it doesn't exist and add it to your `$PATH`).

### Basic usage
To start a new `.html` file in the current directory, type: 
```shell
$ boilerplate <htmlFileName>
```

`boilerplate` will add an `.html` extension to the file name if it's not there,  so `boilerplate index` and `boilerplate index.html` will both create a file called `index.html`. However, it **will not** check if the file already exists—it always overwrites (out of laziness).

`boilerplate` will prompt for a page title, path to a `css` file, and a path to a `js` file:
```shell
Enter page title (press enter to skip):
$ Best page ever
Enter path to CSS file (press enter to skip):
$ style.css
Enter path to JS file (press enter to skip):
$ script.js
```

With the paths above, the resulting html will have these `<link>` and `<script>` tags:
```html
<link rel="stylesheet" type="text/css" href="style.css" />

<!-- stuff here -->

<script type="application/javascript" src="script.js"></script>
```

### Creating files in other directories
If you prefer to have your `css` and `js` files in separate directories, just type them out, and `boilerplate` will create all folders that lead to those files for you:
```shell
Enter page title (press enter to skip):
$ Another great page
Enter path to CSS file (press enter to skip):
$ ./other_stuff/styles/main.css
Enter path to JS file (press enter to skip):
$ ./other_stuff/scripts/main.js
```

The `<link>` and `<script>` tags will look like:
```html
<link rel="stylesheet" type="text/css" href="./other_stuff/styles/main.css" />

<!-- stuff here -->

<script type="application/javascript" src="./other_stuff/scripts/main.js"></script>
```

### Skipping `css` and `js` files
If no `css` and `js` files are specified, `boilerplate` will add `<style>` and `<script>` tags inside of the html file:
```html
<html>
  <head>
    <!-- stuff here -->
    <style>
      /* CSS here */
    </style>
  </head>

  <body>
    <script>
      /* JS here */
    </script>
  </body>
</html>
```

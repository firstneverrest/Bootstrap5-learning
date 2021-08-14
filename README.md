# Bootstrap 5 Learning
Bootstrap 5 is the most famous CSS framework. Find more information in the [official website](https://getbootstrap.com/).

## Installation
1. Bootstrap CDN - easiest way to install
```html
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta http-equiv="X-UA-Compatible" content="IE=edge" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <!-- Bootstrap 5 CSS -->
    <link
      href="https://cdn.jsdelivr.net/npm/bootstrap@5.0.2/dist/css/bootstrap.min.css"
      rel="stylesheet"
      integrity="sha384-EVSTQN3/azprG1Anm3QDgpJLIm9Nao0Yz1ztcQTwFspd3yD65VohhpuuCOmLASjC"
      crossorigin="anonymous"
    />
    <title>Bootstrap 5 Learning</title>
  </head>
  <body>
    <h1>Bootstrap 5 Learning</h1>

    <!-- Bootstrap 5 JavaScript -->
    <script
      src="https://cdn.jsdelivr.net/npm/@popperjs/core@2.9.2/dist/umd/popper.min.js"
      integrity="sha384-IQsoLXl5PILFhosVNubq5LC7Qb9DXgDA9i+tQ8Zj3iwWAwPtgFTxbJ8NT4GN1R8p"
      crossorigin="anonymous"
    ></script>
    <script
      src="https://cdn.jsdelivr.net/npm/bootstrap@5.0.2/dist/js/bootstrap.min.js"
      integrity="sha384-cVKIPhGWiC2Al4u+LWgxfKTRIcfu0JTxR+EQDz/bgldoEyl4H0zUF0QKbrJ0EcQF"
      crossorigin="anonymous"
    ></script>
  </body>
</html>

```
1. CSS and JS Files - when you want to work offline
2. Source files - when you want to config Bootstrap5
3. Build Tools - npm
```
npm install bootstrap
```

## Bootstrap 5 Icons
Put this CDN below the Bootstrap CSS CDN to use Bootstrap 5 icons 
```html
<link rel="stylesheet" href="https://cdn.jsdelivr.net/npm/bootstrap-icons@1.4.1/font/bootstrap-icons.css" />
```

## Reboot
Bootstrap 5 uses Reboot which is a collection of element-specific CSS changes in a single file. Therefore, it helps create simple baseline to style CSS. Reboot has core features as following:
1.  use `rem` instead of `em`
2.  avoid `margin-top`
3.  `inherit` when possible
4.  Native `sans-serif` fonts
5.  body background `#fff`
6.  box sizing: `border-box`

## Customization
To customize some CSS properties, you need to use `npm install bootstrap` to get all files (Bootstrap CDN cannot be customized).
1. Install bootstrap with npm
2. Create sass/main.scss at the root
3. In main.scss, import bootstrap.scss to gain every styles from bootstrap
4. Then, you can start customize by overriding  
    ```scss
    // custom variables
    $primary: #ffcb3b;

    // import the functions & variables

    // import bootstrap
    @import '../node_modules/bootstrap/scss/bootstrap.scss';
    ```
5. Install "Live Sass Compiler" in vscode extension -> open settings -> type "live sass format" -> Click "Edit in settings.json" -> edit as following:

    ```json
    "liveSassCompile.settings.formats": [
          {
              "format": "compressed",
              "extensionName": ".min.css",
              "savePath": "/css"
          }
      ]
    ```
6. Open main.scss and click "Watch Sass" at the bottom of vscode
7. It will create the css with two css files
8. Link `main.min.css` file in HTML

## Resources
- [slides from Bootstrap5 LinkedIn Learning course](https://raybo.org/slides_bootstrap5/)
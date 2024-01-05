# saas

## Compiling Sass with VS Code extensions

install extention - Live saas server - glenn Marks

`CTRL + SHIFT + P -> type open settings(JSON)`

```json 
{
   ...//Add below
    "liveSassCompile.settings.formats": [
        {
            "format": "expanded", //Change to compressed if you need to minify the saas
            "extensionName": ".css",
            "savePath": null, //change the path if you would like to save it in desired location
            "savePathReplacementPairs": null
        }
    ]
}
```

Folow the folder structure format

![Alt text](image.png)


# sass partials (different files)

![Alt text](image-1.png)

@forward
@use

## Sass variables
define
$font : 'Comic Neue', cursive;

use it 

```css
@use "../utils"; //here

html {
    box-sizing: border-box;
    font-size: 100%;
}

*,
*::before,
*::after {
    box-sizing: inherit;
}


body {
    margin: 0;
    padding: 0;
    font-family: utils.$font; //here
    background-color: rgb(66, 66, 66);
    color: rgb(208, 208, 208);
}
```

breakpoints:

sass map
mixin#   l e a r n - s a s s  
 
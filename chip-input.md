# Chip Input

## Material Icon link

```html
<link href="https://fonts.googleapis.com/icon?family=Material+Icons"
      rel="stylesheet">
```

## styles.scss

```scss
@import url('https://fonts.googleapis.com/css2?family=Roboto:wght@300;400;500;700;900&display=swap');

* {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
}

body {
    height: 100vh;
    width: 100vw;
    background-color: #f8f8f9;
    font-family: 'Roboto', sans-serif;
}
```

## Commands used

To generate module : `ng g m chips`

To generate components : 
`ng g c chips --flat true --export true --skip-tests true`

### commands explanation:

 - `--export true` will add components to export array in module.

 - `--flat true` will skip creating additional folder.
 
 - `--skip-tests true` will skip unit test file creation.

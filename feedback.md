# Feedback

## styles.scss

```scss
@import url('https://fonts.googleapis.com/css2?family=Roboto:wght@300;400;500;700;900&display=swap');

* {
    margin: 0;
    padding: 0;
}

body {
    height: 100vh;
    width: 100vw;
    background-color: #83eef9;
    font-family: 'Roboto', sans-serif;
}
```

## Commands used

To generate module : `ng g m feedback`

To generate components : 
`ng g c feedback --flat true --export true`

### commands explanation:

 - `--export true` will add components to export array in module.

 - `--flat true` will skip creating additional folder.

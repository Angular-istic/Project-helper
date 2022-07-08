# Sidenav

## Font awesome link

```html
<link rel="stylesheet" href="https://pro.fontawesome.com/releases/v5.10.0/css/all.css"
    integrity="sha384-AYmEC3Yw5cVb3ZcuHtOA93w35dYTsvhLPVnYs9eStHfGJvOvKxVfELGroGkvsg+p" crossorigin="anonymous" />
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
    position: relative;
    font-family: 'Roboto', sans-serif;
}

.card {
    display: flex;
    flex-direction: column;
    border-radius: .5rem;
    background-color: #fff;
    margin: 1.25rem 0 1.25rem 0;
    box-shadow: 0 .25rem .5rem #e6edef;

    .card-head {
        padding: 1rem 1.5rem;
        border-bottom: 1px solid #edf1f7;
        font-size: 1rem;
        font-weight: 600;
    }

    .card-body {
        padding: 1rem 1.5rem; 
    }
}
```

## Commands used

### To generate components : 

`ng g c body --skip-tests true` 

`ng g c sidenav --skip-tests true` 

`ng g c dashboard --skip-tests true` 

`ng g c products --skip-tests true` 

`ng g c statistics --skip-tests true` 

`ng g c coupens --skip-tests true` 

`ng g c pages --skip-tests true` 

`ng g c media --skip-tests true` 

`ng g c settings --skip-tests true` 

# Sidenav with Multi Level Menu

## Commands used

### To generate components :

`ng g c sublevel-menu --inline-template --inline-style --flat true`

`ng g c coupen-list --module coupens`

`ng g c product-level-three-one --module products`

`ng g c product-level-three-two --module products`

### To generate modules:

`ng g m coupens --routing --flat true`

`ng g m products --routing --flat true`


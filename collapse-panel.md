# Collapse Panel


## Font awesome link

```html
<link rel="stylesheet" href="https://pro.fontawesome.com/releases/v5.10.0/css/all.css"
    integrity="sha384-AYmEC3Yw5cVb3ZcuHtOA93w35dYTsvhLPVnYs9eStHfGJvOvKxVfELGroGkvsg+p" crossorigin="anonymous" />
```

## Commands used

To generate module : `ng g m collapse-panel`

To generate components :

 - `ng g c collapse-panel --module collapse-panel --flat true --skip-tests true --export true`

 - `ng g c collapse-header --module collapse-panel --flat true --skip-tests true --export true --inline-template true --inline-style true`

 - `ng g c collapse-content --module collapse-panel --flat true --skip-tests true --export true --inline-template true --inline-style true`

### commands explanation:

 - `--module collapse-panel` will add components to collapse-panel module.

 - `--export true` will add components to export array in module.

 - `--skip-tests true` will skip `spec.ts` file creation.

 - `--flat true` will skip creating additional folder.

 - `--inline-template true` will create a component with inline template in the ts file.

 - `--inline-style true` will create a component with inline styles in the ts file.


## styles.scss

```scss
/* You can add global styles to this file, and also import other style files */
@import url('https://fonts.googleapis.com/css?family=Roboto:400,500,700,900&display=swap');

* {
    margin: 0;
}
body {
    background-color: #575ced;
    font-family: 'Roboto', sans-serif;
}
```

## collapse-panel.component.scss

```scss
.c-panel-container {
  border: 1px solid #dee2e6;
  background: #f9f9f9;
  color: #495057;
  border-radius: 6px;
  margin: 20px;
}

.c-panel-header {
  border: 1px solid #dee2e6;
  color: #343a40;
  background: #fff;
  font-weight: 700;
  border-radius: 6px;
  cursor: pointer;
  width: 100%;
}

.c-panel-header-container {
  display: flex;
  align-items: center;
  padding: 1.25rem;
}

.c-panel-header-icon {
  margin-right: 0.5rem;
}

.c-panel-header-text {
  line-height: 1;
}

.c-panel-content {
  background: #f9f9f9;
  padding: 1.25rem;
}

```

## app.component.scss

```scss
:host {
  width: 100vw;
  height: 100vh;

  .container {
    display: flex;
    flex-direction: row;
    justify-content: center;
    margin: 50px;

    h2 {
      text-align: center;
      color: #fff;
    }

    .normal,
    .custom {
      width: 500px;
    }
  }

  .header-container {
    display: flex;
  }

  .header-title {
    margin-right: 150px;
  }

  .social-section {
    font-weight: normal;
    display: flex;
  }

  .fa-facebook-f {
    font-size: 18px;
    color: #1877f2;
  }

  .fa-twitter {
    color: #1da1f2;
  }

  .fa-instagram {
    color: #c32aa3;
  }

  .fa-dribbble {
    color: #ea4c89;
  }

  .fa-twitter,
  .fa-instagram,
  .fa-dribbble {
    font-size: 20px;
  }

  .profile {
    .profile-head {
      display: flex;
      align-items: center;
      margin-bottom: 20px;
    }

    .profile-img {
      background-color: #fff;
      width: 85px;
      height: 85px;
      border-radius: 50%;
      box-shadow: 0 3px 6px rgba(129, 129, 129, 0.16),
        0 3px 6px rgba(105, 105, 105, 0.23);
      margin-right: 20px;

      img {
        width: 100%;
        height: 100%;
        border-radius: 50%;
      }
    }

    .profile-title {
      font-weight: 600;
      font-size: 1.25rem;
      display: inherit;
    }

    .profile-desig {
      margin-top: 5px;
      font-size: 13px;
      font-weight: 500;
      color: black;
      opacity: 0.8;
    }
  }
}

.mr-10 {
  margin-right: 10px;
}

.mr-20 {
  margin-right: 20px;
}
```
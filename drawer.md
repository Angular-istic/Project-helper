# Drawer

## Font awesome link

```html
<link rel="stylesheet" href="https://pro.fontawesome.com/releases/v5.10.0/css/all.css"
    integrity="sha384-AYmEC3Yw5cVb3ZcuHtOA93w35dYTsvhLPVnYs9eStHfGJvOvKxVfELGroGkvsg+p" crossorigin="anonymous" />
```

## Commands used

To generate module : `ng g m drawer`

To generate components : 

`ng g c drawer --module drawer --export true --flat true`

### commands explanation:

 - `--module drawer` will add components to drawer module.

 - `--export true` will add components to export array in module.

 - `--flat true` will skip creating additional folder.

## styles.scss

 ```scss
/* You can add global styles to this file, and also import other style files */
html, body {
    margin: 0;
    padding: 0;
}
body {
    width: 100vw;
    height: 100vh;
    font-family: Roboto, Helvetica Neue, sans-serif;
    font-size: 14px;
}
 ```

## drawer.component.scss

```scss
.p-sidebar {
  position: fixed;
  transition: transform .3s;
  display: flex;
  flex-direction: column;
  background-color: white;
  box-shadow: 4px 0 8px #dde5ec, -4px 0 8px #dde5ec;
}

.p-sidebar-content {
  position: relative;
  overflow-y: auto;
  margin: 0 15px;
}

.p-sidebar-header {
  display: flex;
  align-items: center;
  justify-content: space-between;
  margin: 0 15px;
}

.p-sidebar-left {
  top: 0;
  left: 0;
  width: 20rem;
  height: 100%;
}

.p-sidebar-right {
  top: 0;
  right: 0;
  width: 20rem;
  height: 100%;
}

.p-sidebar-top {
  top: 0;
  left: 0;
  width: 100%;
  height: 11rem;
}

.p-sidebar-bottom {
  bottom: 0;
  left: 0;
  width: 100%;
  height: 11rem;
}

.fa-times {
  font-size: 20px;
  cursor: pointer;
  color: #323232;
}

.sidebar-left-header {
  flex-direction: row-reverse;
  justify-content: start;

  .fa-times {
    margin-right: 25px;
  }
}
```

## app.component.scss

```scss
.buttons {
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
  height: 100%;
  background-color: #edf1f7;
}

.app-list {
  list-style-type: none;
  padding: 0;
  margin: 0;
}

.app-list-item {
  border-bottom: 1px solid #edf1f7;
  color: #222b45;
  font-size: 0.9375rem;
  line-height: 1.25rem;
  padding: 8px;
}

.app-list-item:last-child {
  border-bottom: none;
}

.app-list-icons {
  padding-right: 5px;
}

.app-button {
  line-height: 1.2;
  padding: 7px 10px;
  border-radius: 8px;
  border-color: transparent;
  font-size: 16px;
  background-color: #3182ce;
  color: #ffffff;
  cursor: pointer;
  outline: 0;
}

.mr-5 {
  margin-right: 5px;
}

.mb-10 {
  margin-bottom: 10px;
}
```
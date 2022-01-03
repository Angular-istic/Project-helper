# Incremental Notification

## Font awesome link

```html
<link rel="stylesheet" href="https://pro.fontawesome.com/releases/v5.10.0/css/all.css"
    integrity="sha384-AYmEC3Yw5cVb3ZcuHtOA93w35dYTsvhLPVnYs9eStHfGJvOvKxVfELGroGkvsg+p" crossorigin="anonymous" />
```

## styles.scss

```scss
body {
  margin: 0;
  padding: 0;
}
```

## app.component.scss

```scss
.container {
  display: flex;
  justify-content: center;
  align-items: center;
  flex-direction: column;
  width: 100vw;
  height: 100vh;
}

.notification {
  cursor: pointer;
  position: relative;
  padding: 1rem 1.1rem;
  background: #ff8084;
  border-radius: 50%;
  box-shadow: 0 0.3rem 0.75rem #e1e5e5;
  text-align: center;
  color: #fff;
}

.icon {
  font-size: 1.8rem;
}

.badge {
  position: absolute;
  background: #ff8084;
  right: -0.938rem;
  top: -0.938rem;
  padding: 0.3rem 0.6rem;
  border-radius: 50%;
  border: 3px solid #FFF;
}

.btn-send {
  cursor: pointer;
  font-weight: 600;
  font-size: 0.8rem;
  padding: 1rem 2rem;
  outline: none;
  color: #fff;
  border-radius: 0.3rem;
  background: #ff8084;
  border: 1px solid #ff8084;
  margin-top: 6.25rem;
}

.ripple {
  background-position: center;
  transition: background 0.9s;
}

.ripple:hover {
  background: #ff8084 
    radial-gradient(circle, transparent 1%, #ff8084 1%) center/15000%;
}

.ripple:active {
  background-color: #fc5c61;
  background-size: 100%;
  transition: background 0s;
}

.notify {
  transform-origin: 50% 4px;
  animation: ring 1.5s ease;
}

@keyframes ring {
  0% {
    transform: rotate(35deg);
  }

  12.5% {
    transform: rotate(-30deg);
  }

  25% {
    transform: rotate(25deg);
  }

  37.5% {
    transform: rotate(-20deg);
  }

  50% {
    transform: rotate(15deg);
  }

  62.5% {
    transform: rotate(-10deg);
  }

  75% {
    transform: rotate(5deg);
  }

  100% {
    transform: rotate(0deg);
  }
}
```
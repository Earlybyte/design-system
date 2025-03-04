# Page Layout

This is the page layout we recommand to use. The `bal-app` class enables the Baloise Design System styles underneath it.

The `.container` is a simple utility element that allows you to center content on larger viewports.

[Bulma Documentation](https://bulma.io/documentation/layout/container/)

:::tip
To stick the footer at the end of the page add the class `has-sticky-footer` to your body and apply the same structure as shown in the belows example.
:::

```html
<body class="bal-app has-sticky-footer">
  <main>
    <div class="container">
      <!-- Page content -->
    </div>
  </main>
  <footer class="footer">
    <div class="container">
      <!-- Footer content -->
    </div>
  </footer>
</body>
```

## Usage

### Angular Sticky Footer

In angular the setup for a sticky footer is slightly diffrent.

#### index.html

Place the `bal-app` component inside the angular root element.

```html
<body>
  <app-root>
    <bal-app>
      <main>
        <!-- Your application content -->
      </main>
      <footer></footer>
    </bal-app>
  </app-root>
</body>
```

#### app.component.html

In the app component we define the rest of the structure.

```html
<main>
  <div class="container">
    <!-- Page content -->
    <router-outlet></router-outlet>
  </div>
</main>
<footer class="footer">
  <div class="container">
    <!-- Footer content -->
  </div>
</footer>
```

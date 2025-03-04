# Breakpoints

The library supports those 4 breakpoints.

[Go to the Bulma documentation](https://bulma.io/documentation/overview/responsiveness/#breakpoints)

| Device               | Starts at screen width |
| -------------------- | ---------------------- |
| Mobile               | 0px                    |
| Tablet               | 720px                  |
| Desktop              | 960px                  |
| Fullhd or Widescreen | 1200px                 |

## Sass mixins

There are 9 responsive mixins, which can be easly be used in your sass files.

Use the scss mixins in your application like this.

```scss
@import 'node_modules/@baloise/design-system-components/src/styles/global.utilities';

.bal-element {
  width: 100%;
}

@include tablet() {
  .bal-element {
    width: 380px;
  }
}

@include desktop() {
  .bal-element {
    width: 570px;
  }
}
```

The file `global.utilities` provides all the defined scss variables like [colors](/guide/styles/colors.html) and also the mixins.

## CSS Helper Classes

Out of the responsive tokens we create a collection of helper css classes.

[Go to the Bulma documentation](https://bulma.io/documentation/modifiers/responsive-helpers/)

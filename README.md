# stylep-grid
<img src=https://avatars1.githubusercontent.com/u/16121328?v=3&s=200 title=stylep-button align=right height=95>

A simple flexbox grid system comprised of containers, rows and columns. With variable inheritance you can make it do whatever you want.


## Install
You can install using the [spm](https://github.com/stylep/stylep) command or install using npm and the project title.

``` shell
spm install grid
```

## Usage
``` css
/* grid.css */

@import “stylep-grid”;

.container {
  /* Container Pattern */
  @extend %container;
}

.row {
  /* Row Pattern */
  @extend %row;
}

.column {
  /* Column Pattern */
  @extend %column;
}

```

## Patterns
Placeholder selectors that contain common styles for structure and basic behavior.

#### `@extend %spacer;`
This is a generic pattern that expands the entirety of the space around the element it is applied to. See the example for absolute centered objects with spacer.

### Container

#### `@extend %container;`
A simple margin auto hack container.

#### `@extend container-column;`
Flexbox enabled column.

#### `@extend container-flex;`
Center aligned flexible container.

#### `@extend container-fluid;`
A simple container with inner padding.

### Row

#### `@extend %row;`
A basic flexbox enabled row.

#### `@extend %row-reverse;`
Same thing only backwards ordered columns in it.

#### `@extend %row-break;`
A row that does away with margins and bleeds right up to the edge of the containing element.

#### `@extend %row-collapse;`
This removes all horizontal padding from your columns in this row.

### Columns

#### `@extend %column;`
A column that horizontally expands to the containing element.

#### `@extend %column-reverse;`
Same as a column, only it appears in reverse order.

#### `@mixin column $width;`
A simple column sizing mixin.

#### `@extend %column-first;`
This takes your column and places it at the beginning of the containing row.

#### `@extend %column-last;`
This takes your column and places it at the end of the containing row.

#### `@extend %column-X;`
Replace X with any number between 1-12 to get a element with that specific number of columns.

#### `@extend %column-push-X;`
Replace X with any number between 1-11 to push your element that many columns wide.

#### `@extend %column-pull-X;`
Replace X with any number between 1-11 to pull your element that many columns wide.

## License
This project is licensed under the MIT [license](LICENSE).


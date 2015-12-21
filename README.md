# stylep-grid

Everything you need to get started making a new style pattern.
<img src=https://avatars1.githubusercontent.com/u/16121328?v=3&s=200 title=stylep-button align=right height=95>

## Install
You can install using the [spm](https://github.com/stylep/stylep) command or install using npm and the project title.

``` shell
spm install grid
```

## Usage
``` css
/* grid.css */

@import “stylep-grid”;

.class {

  /* Button Design Pattern */
  @extend %grid;

  /* Customize your button */
  @mixin grid param, param;

  /* or roll your own */

  /* add something custom in here */
}
```

## Patterns
Placeholder selectors that contain common styles for structure and basic behavior.

#### `@extend %grid-inline;`
Describe what this pattern does.

## Styles
Customizable presets that give your pattern a specific style-set.

### grid-solid
Describe the visual look and feel of this style.

##### Options

* `$param: default-value` Describe what this does

##### Example
```css
/* describe in english what this following statement really means in detail */
@mixin grid-solid default-value;
```


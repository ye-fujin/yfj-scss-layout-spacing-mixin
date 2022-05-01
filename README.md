# Yet another SCSS layout spacing mixin to generate a list of atomic classes for margin/padding

### If you need to generate a list of atomic CSS classes like

- `<div class"mx-10"></div>` to have horizontal margins,
- `<div class"my-10"></div>` to have vertical margins,
- `<div class"mxy-10"></div>` to have both horizontal and vertical margins,
- `<div class"m{t,r,b,l}-10"></div>` to set top/right/bottom/left margins in px (by default) or alternative units.

All the same goes for padding.

### Example usage for margin:

`$yfj-margin-map: ( 'x': ( 10 ), 'y': ( 20 ) );`

`@include yfj-layout-spacing-mapping('margin', $yfj-margin-map);`

### Example usage for padding:

`$yfj-padding-map: ( 'xy': ( 10 ), 'top': ( 20 ), 'right': ( 20 ), 'bottom': ( 20 ), 'left': ( 20 ) );`

`@include yfj-layout-spacing-mapping('padding', $yfj-padding-map);`

### Example usage with alternative units:

`$yfj-padding-map: ( 'x': ( 5 ), 'y': ( 10 ) );`

`@include yfj-layout-spacing-mapping('padding', $yfj-padding-map, '%');`

Version 1.0.0

Copyright Ye-Fujin, 2022<br>
License MIT

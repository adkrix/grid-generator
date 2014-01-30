GRID GENERATOR
==============

Custom grid generator with bootstrap style
I used bootstrap grid style. See http://getbootstrap.com/css/#grid for details. But you can create your own grid system using only `grid-generator` mixin.


LESS STYLE
----------

Include `grid-generator.less` into your main less file

>@import "vendor-path/css/grid-generator"

###Simple responsive grid 

> @cols: 12;
>
> @gutter: 30px;
>
> @col-name: 'xcol';
>
> @row-name: 'xrow';
>
> @min-width: 0; // if @min-width > 0 then wrapped by @media (min-width: @min-width)
>
> .grid-generator(@cols, @gutter, @col-name, @row-name, @min-width)

It generates classes: 
`.xrow` , 
`.xcol-1` ... `.col-12`,
`.xcol-offset-0` ... `.xcol-offset-12`,
`.xcol-pull-0` ... `.xcol-pull-12`,
`.xcol-push-0` ... `.xcol-push-12`.

###Responsive grid

Limits 768px / 992px / 1200px

> @cols: 12;
>
> @gutter: 30px;
>
> @col-name: 'col';
>
> @row-name: 'row';
>
> .grid-generator-responsive(@cols, @gutter, @col-name, @row-name)

It generates classes: `.row` , 

`.col-xs-1` ... `.col-xs-12`, 
`.col-xs-offset-0` ... `xcol-xs-offset-12`,

`.col-sm-1` ... `.col-sm-12`, 
`.col-sm-offset-0` ... `.col-sm-offset-12`,
`.col-sm-pull-0` ... `.col-sm-pull-12`,
`.col-sm-push-0` ... `.col-sm-push-12`,

`.col-md-1` ... `.col-md-12`, 
`.col-md-offset-0` ... `.col-md-offset-12`,
`.col-md-pull-0` ... `.col-md-pull-12`,
`.col-md-push-0` ... `.col-md-push-12`,

`.col-lg-1` ... `.xcol-lg-12`, 
`.col-lg-offset-0` ... `.col-lg-offset-12`,
`.col-lg-pull-0` ... `.col-lg-pull-12`,
`.col-lg-push-0` ... `.col-lg-push-12`.

###Mobile grid

Limits 480px / 768px / 992px / 1200px

> @cols: 16;
>
> @gutter: 20px;
>
> @col-name: 'grd';
>
> @row-name: 'grd';
>
> .grid-generator-mobile(@cols, @gutter, @col-name, @row-name)

It generates classes: `.grd`  for row and for  columns widths,  offsets and orderings

`.grd-xx-1` ... `.grd-xx-16`,
`.grd-xx-offset-0` ... `grd-xx-offset-16`,

`.grd-xs-1` ... `.grd-xs-16`,
`.grd-xs-offset-0` ... `grd-xs-offset-16`,
`.grd-xs-pull-0` ... `.grd-xs-pull-16`,
`.grd-xs-push-0` ... `.grd-xs-push-16`,

`.grd-sm-1` ... `.grd-sm-16`,
`.grd-sm-offset-0` ... `grd-sm-offset-16`,
`.grd-sm-pull-0` ... `.grd-sm-pull-16`,
`.grd-sm-push-0` ... `.grd-sm-push-16`,

`.grd-md-1` ... `.grd-md-16`,
`.grd-md-offset-0` ... `grd-md-offset-16`,
`.grd-md-pull-0` ... `.grd-md-pull-16`,
`.grd-md-push-0` ... `.grd-md-push-16`,

`.grd-lg-1` ... `.grd-lg-16`,
`.grd-lg-offset-0` ... `grd-lg-offset-16`,
`.grd-lg-pull-0` ... `.grd-lg-pull-16`,
`.grd-lg-push-0` ... `.grd-lg-push-16`.


SASS STYLE
----------

Include `_grid-generator.sass` into your main sass or scss file

>@import "vendor-path/css/grid-generator"

###Simple responsive grid

> $cols: 12;
>
> $gutter: 30px;
>
> $col-name: 'xcol';
>
> $row-name: 'xrow';
>
> $min-width: 0; // if $min-width > 0 then wrapped by @media (min-width: $min-width)
>
> @include grid-generator($cols, $gutter, $col-name, $row-name, $min-width)

See output in LESS part

###Responsive grid

Limits 768px / 992px / 1200px

> $cols: 12;
>
> $gutter: 30px;
>
> $col-name: 'col';
>
> $row-name: 'row';
>
> @include grid-generator-responsive($cols, $gutter, $col-name, $row-name)

See output in LESS part

###Mobile grid

Limits 480px / 768px / 992px / 1200px

> $cols: 16;
>
> $gutter: 20px;
>
> $col-name: 'grd';
>
> $row-name: 'grd';
>
> @include grid-generator-mobile($cols, $gutter, $col-name, $row-name)

See output in LESS part
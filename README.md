GRID GENERATOR
==============

Custom grid generator with bootstrap style


LESS STYLE
----------

Code has more simple functionality because LESS language is very primitive

Include `grid-generator.less` into your main less file

>@import "vendor-path/css/grid-generator.less"

###Simple responsive grid 

>@cols: 12;
>
>@gutter: 30px;
>
>@col-name: 'xcol';
>
>@row-name: 'xrow';
>
>@offsets: true;   // generate .xcol-offset-1 ...
>
>@ordering: true;   // generate .xcol-pull-1 ...,  .xcol-push-1 ...
>
>@min-width: 0;
>
> .grid-generator(@cols, @gutter, @col-name, @row-name, @offsets, @ordering, @min-width)

It generates classes: 
`.xrow` , 
`.xcol-1` ... `.col-12`,
`.xcol-offset-0` ... `.xcol-offset-11`,
`.xcol-pull-0` ... `.xcol-pull-11`,
`.xcol-push-0` ... `.xcol-push-11`.
See http://getbootstrap.com/css/#grid for details.

###Responsive grid

Limits 768px / 992px / 1200px

>@cols: 12;
>
>@gutter: 30px;
>
>@col-name: 'col';
>
>@row-name: 'row';
>
>@xs-offsets: true;   // generate .col-xs-offset-1 ...
>
> .grid-generator-responsive(@cols, @gutter, @col-name, @row-name, @xs-offsets)

It generates classes: `.row` , 

`.col-xs-1` ... `.col-xs-12`, 
`.col-xs-offset-0` ... `xcol-xs-offset-11`,

`.col-sm-1` ... `.col-sm-12`, 
`.col-sm-offset-0` ... `.col-sm-offset-11`,
`.col-sm-pull-0` ... `.col-sm-pull-11`,
`.col-sm-push-0` ... `.col-sm-push-11`,

`.col-md-1` ... `.col-md-12`, 
`.col-md-offset-0` ... `.col-md-offset-11`,
`.col-md-pull-0` ... `.col-md-pull-11`,
`.col-md-push-0` ... `.col-md-push-11`,

`.col-lg-1` ... `.xcol-lg-12`, 
`.col-lg-offset-0` ... `.col-lg-offset-11`,
`.col-lg-pull-0` ... `.col-lg-pull-11`,
`.col-lg-push-0` ... `.col-lg-push-11`.

###Mobile grid

Limits 480px / 768px / 992px / 1200px

>@cols: 16;
>
>@gutter: 20px;
>
>@col-name: 'grd';
>
>@row-name: 'grd';
>
>@xx-offsets: true;   // generate .col-xx-offset-1 ...
>
> .grid-generator-mobile(@cols, @gutter, @col-name, @row-name, @xx-offsets)

It generates classes: `.grd`  for row and for  columns widths,  offsets and orderings

`.grd-xx-1` ... `.grd-xx-16`,
`.grd-xx-offset-0` ... `grd-xx-offset-11`,

`.grd-xs-1` ... `.grd-xs-16`,
`.grd-xs-offset-0` ... `grd-xs-offset-15`,
`.grd-xs-pull-0` ... `.grd-xs-pull-15`,
`.grd-xs-push-0` ... `.grd-xs-push-15`,

`.grd-sm-1` ... `.grd-sm-16`,
`.grd-sm-offset-0` ... `grd-sm-offset-15`,
`.grd-sm-pull-0` ... `.grd-sm-pull-15`,
`.grd-sm-push-0` ... `.grd-sm-push-15`,

`.grd-md-1` ... `.grd-md-16`,
`.grd-md-offset-0` ... `grd-md-offset-15`,
`.grd-md-pull-0` ... `.grd-md-pull-15`,
`.grd-md-push-0` ... `.grd-md-push-15`,

`.grd-lg-1` ... `.grd-lg-16`,
`.grd-lg-offset-0` ... `grd-lg-offset-15`,
`.grd-lg-pull-0` ... `.grd-lg-pull-15`,
`.grd-lg-push-0` ... `.grd-lg-push-15`.




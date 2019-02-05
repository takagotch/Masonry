### Masonry
---
https://masonry.desandro.com/

```css
.grid-item {
  float: left;
  width: 80px;
  height: 60px;
  border: 2px solid hsla(0, 0%, 0%, 0.5);
}
.grid-item--width2 { width: 160px; }
.grid-item--height2 { height: 140px; }

.grid-sizer,
.grid-item { width: 20%; }
.grid-item--width2 { width: 40%; }

itemSelector: '.grid-item'

.grid-sizer,
.grid-item { width: 20% }
.grid-item--width2 { width: 40%; }

columnWidth: '.grid-sizer',
itemSelector: '.grid-item',
percentPosition: true

columnWidth: '.grid-sizer'
columnWidth: $grid.find('.grid-sizer')[0]

.grid-sizer { width: 33.333%; }
@media screen and (min-width: 768px){
  .grid-sizer { width: 20%; }
}

gutter: 10

.gridd-item {
  margin-bottom: 10px;
}
```

```js
$('.$grid').masonry({
  itemSelector: '.grid-item',
  columnWidth: '.grid-sizer',
  percentPosition: true
})

var $grid = $('.grid').masonry({
});
$grid.imagesLoaded().progress( function(){
  $grid.masonry('layout');
});

var $grid.imagesLoaded( function(){
  $grid.masonry({
  });
});


$('.grid').masonry({
  columnWidth: 200,
  itemSelector: '.grid-item'
});

var msnry = new Masonry( '.grid', {
  columnWidth: 200,
  itemSelector: '.grid-item'
});
```

```
<div class="grid" data-masonry='{ "columnWidth": 200, "itemSelector": ".grid-item" }'>
```


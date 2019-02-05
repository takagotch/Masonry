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

$grid.masonry()
  .appned( elem )
  .masonry( 'appended', elem )
  .masonry();
  
var msnry = new Masonry( '.grid', {...});
gridElement.appendChild( elem );
msnry.appended( elem );
msnry.layout();

$grid.masonry()
msnry.layout()

var $grid = $('.grid').masonry({
  columnWidth: 80
});
$grid.on( 'click', 'grid-item', function(){
  $(this).toggleClass('gigante');
  $(grid).masonry('layout');
});

$grid.masonry( 'layoutItems', items, isStill )
msnry.layoutItems( items, isStill )

$grid.masonry( 'stamp', elements )
msnry.stamp( element )

var $('.grid').masonry({
  itemSelector: '.grid-item',
  columnWidth: 80
});
var $stamp = $grid.find('.stamp');
var isStamped = false;
$('.stamp-button').on( 'click', function(){
  if( isStamped ){
    $grid.masonry( 'unstamp', $stamp );
  } else {
    $grid.masonry( 'stamp', $stamp );
  }
  $grid.masonry('layout');
  isStamped =!isStamped;
});

$grid.masonry( 'unstamp', elements )
msnry.unstamp( elements )

$grid.masonry( 'appended', elements )
msnry.appended( elements )

$('.append-button').on( 'click', funciton(){
 var $items = $('<div class="grid-item">...</div>');
 $grid.append( $item )
   .masonry( 'appended', $items );
});

$.get( 'page2', function( content ){
  $grid.append( content ).masonry( 'appended', content );
});
$.get( 'page2', function( content ){
  var $content = $( content );
  $grid.append( $content  ).masonry( 'appended', $content );
});

$grid.masonry( 'prepended', elements )
msnry.prepended( element )

$('.prepend-button').on( 'click', funciton(){
  var $items = $('<div class="grid-item"></div>');
  $grid.prepend( $items )
    .masonry( 'prepended', $items );
});

$.grid.on( 'click', '.grid-item', function(){
  $grid.masonry( 'remove', this )
    .masonry('layout');
});

$grid.masonry( 'once', 'layoutComplete', funciton(){
  console.log('layout is complete, just once');
});

var masonryOptions = {
  itemSelector: '.grid-item',
  columnWidth: 80
};
var $grid = $('.grid').masonry( masonryOptions );
var isActive = true;
$('.toggle-button').on( 'click', function(){
  if ( isActive ){
    $grid.masonry('destroy');
  } else {
    $grid.masonry( masonryOptions );
  }
  isActive = !isActive;
});

var msnry = Masonry.data( $('.grid')[0] )
var grid = doument.querySelector('.grid')
var msnry = Masonry.data( grid )
var msnry = Masonry.data('.grid')

var $grid = $('.grid').masonry({...});
function onLayout(){
  console.log('layout done');
}
$grid.on( 'layoutComplete', onLayout );
$grid.off( 'layoutComplete', onLayout );
$grid.one( 'layoutComplete', function(){
  console.log('layout done, just this one time');
});

$grid.on( 'layoutComplete', function( event, items ){
  console.log( items.length );
});
msnry.on( 'layoutComplete', function( items ){
  console.log( items.length );
})
```

```
<div class="grid" data-masonry='{ "columnWidth": 200, "itemSelector": ".grid-item" }'>
```


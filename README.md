# bootstrap-carousel-speed
Customized bootstrap 3.3.7 carousel.js plugin to have user defined transition speed of slides.

## About
As asked in many stackoverflow posts like http://stackoverflow.com/q/17332431/3429430 and http://stackoverflow.com/q/20840018/3429430 bootstrap 3.3.7 carousel cannot have different sliding speed only with css. The carousel.js file is also needed to be modified. With this plugin you can initialize bootstrap carousel in your js with custom user defined sliding speed. This is different from the interval option.

## Install with Bower
`bower install bootstrap-carousel-speed`

## How to Initialize

In your css put: 
```
@media all and (transform-3d), (-webkit-transform-3d) {   
    .carousel-inner > .item {    	
        transition: transform 1500 ease-in-out;
    }    
}
```

In your main js initialize bootstrap carousel with
```
$('#bslider').carousel({
  TRANSITION_DURATION: 1500 // This is my custom bootstrao property that sets each transitions time
})
```
Note that transition duration must be same in both css and js.



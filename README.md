# bootstrap-carousel-speed
Customized bootstrap carousel.js plugin to have custom transition speed for slides.
------------------------------------------------------------------------------------------------------------------

As asked in many stackoverflow posts like http://stackoverflow.com/q/17332431/3429430 and http://stackoverflow.com/q/20840018/3429430 bootstrap latest carousel cannot have different sliding speed only with css. The carousel.js file is also needed to be modified.

In your css put: 

@media all and (transform-3d), (-webkit-transform-3d) {   
    .carousel-inner > .item {    	
        transition: transform 1500 ease-in-out;
    }    
}

IN your main js initialize ootstrap carousel with

$('#bslider').carousel({
  TRANSITION_DURATION: 1500 // This is my custom bootstrao property that sets each transitions time
})

Note that transition duration must be same in both css and js.

# Make card 3d rotate on mouseover

* Insert div, set background image to card
* Select div, add class 'card'
* Add trigger on element trigger > mouse move over element
* Create new Play Mouse Animation
* Next to "Mouse Animation" click +; Name it: Rotate on mouseover
* Under Mouse X Actions, Add 0% rotate on y axis to -5deg
* At 100%, rotate y 5deg
* Under Mouse Y Actions, Add 0% rotate on x axis to -5deg
* At 100%, rotate x 5deg
* Notice it's still flat.  So add perspective 1000px on parent div element
* Close out of animation
* Experiment with smoothing slider
* Experiment with Animation Resting State values (affects mouseout)
* Add highlight by dragging in a div block
* Name it card-highlight
* set width = 400px; height = 400px
* set position to absolute
* position it to top-left
* ensure that parent element (card) is set to position:relative
* ensure that parent element (card) is set to overflow: hidden
* set card-highlight background color to white
* set border radius to 50%
* set opacity down to 10%
* add in a blur filter to 20px
* but temporarily turn off filter for now
* select card, select animation "rotate on mouseover"
* select card-highlight
* Under Mouse X Actions, At 0% Add a move x axis 100%
* At 100%, Add a move x axis -50%
* Under Mouse Y Actions, at 0%, Add a move y 50%
* At 100%, Add a move y -50%
* Turn filter back on










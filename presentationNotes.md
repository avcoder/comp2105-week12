# webflow.com

- here's their website
- as you can see, this is the kind of thing you can do with it
- it's a GUI based platform where you can make webpages
- wait for my email invite so you can create an account

# styles, nav, interactions

- I'll demonstrate what Webflow is about
- these are 3 main things I've used most often
- I'm going to introduce this styles panel
- I'll introduce all the buttons so you're not lost
- top right corner, you have 5 different tabs

## styles

- minimize everything, so styles tab contains everything about: layout, typography, backgd, ...
- out of all the buttons in layout, this is the most used which controls margins/padding
- width/height can be other units besides px
- position: relative, absolute, fixed

### typography

- font color
- font size

### background

- choose bg image, or gradient, or solid colour

### transitions & transforms

- we'll get into this in a minute but this is where you'd make those changes

### effects

- opacity

## navigator

- read it
- sometimes you need greater precision
- so here, you'll see the html structure under navigator which allows you to drag/drop with precision

## interactions

- this is where we do animations

# publish

- let's say you finished your website, on the top right corner, click publish
- it'll give you a published website for free, here's the web address

## left hand side

- left hand side, you can click Plus button to add elements
- what I find doing a lot is I'll add a section (create bricks), then within section I add container, then within container I add different elements
- image button to add image
- assets will show you all uploads
- final thing is this little eyeball called "toggle preview" you can see a preview of your page without the GUI

# 2D

- so these next 3 slides, we'll do a quick review of Weeks 3,4,5

## Challenge 1. Add transform (move/skew) upon click

- fyi: keep in mind where your selecting
- story: often times I'll click something, change a prop to the side, click elsewhere on page. But as soon as I click elsewhere, notice there's a blue outline on a different element, so if I decide to make another change -- it'll be the wrong element
- top right corner, click dropdown "States" > Pressed (notice how it entered a tag)
- btw this Selector, they call it tags or classes. So whatever you enter here, you can think of it as classes
- to add a transform, goto: transitions & transforms tab > Plus icon for transforms
- notice you have a prompt where you can move, scale, rotate, skew
- let's experiment with the x slider - so it moves it from side to side, let's just make it go to the left
- so that's what I want the image to do upon click
- to close it out, click X - and it's done
- go back to dropdown states > "none"
- click preview eyeball and click on image - basic transform (Done Week 3)
- Let's add skew as well
- notice I clicked on image, but based on blue outline I got its parent instead -- goto navigator tab and select img
- dropdown "Pressed", you should see your original transform
- add a Skew
- dropdown "None"
- click preview and click on image

## Challenge 2. Add transform (rotate/scale) upon hover

- Choose a button
- dropdown "hover"
- add transform scale (bigger), close that
- click plus sign to add a rotate also, close that
- dropdown "none"
- preview and hover over button

## Challenge 3. Add opacity change

- dropdown "hover"
- change opacity to mid
- dropdown "none"
- preview and hover

# transition

- so that was week 3, notice so far it's just jump cuts, they're not smoothly transitioning
- now to week 4, remember this? so in 2s it'll change the color
- so let's implement the above in webflow
- select same button
- click "transitions & transforms" > transitions > Add Transition button (looks like clock)
- dropdown "font color"
- 2000ms
- ease button and choose an ease in
- top right corner dropdown "states" > "hover" (we see button already styled there)
- typography tab > change color
- dropdown "none" then preview; in 2s font colour turns red
- make rotate and translateX also transition smoothly

# keyframes

- remember week 5?
- this is what we'll demonstrate using...

# Lab

- this is what we'll be doing
- show how each video corresponds to the section within webflow

# detect scrolling in js

- credit: Wes Bos JS30 exercise
- show demo
- there are 2 vanila JS ways - old vs new
- old way: If image is half shown, and if image is not totally scrolled past it, then add class, otherwise remove it
- how do you calculate half shown? (go thru calc)
- so that's the low-level way to do this kind of thing
- Demo it

  - open new tab to google
  - in console, create click Eye icon to create new live expression
  - window.scrollY
  - compare when there's a narrow window vs larger window - does max value change?
  - window.innerHeight
  - compare when there's a narrow window vs larger window - does max value change?

# new intersection observer

- however as of last year, there is a new way - IntersectionObserver browser API
- click link to Wes Bos' tweet
- read comments and try it

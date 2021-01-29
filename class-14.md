## CSS Transforms

- the **transform** property gives alternate ways to size, position, and change elements.
- two dimensional transforms work on the x and y axes.
- three dimensional transforms work on the x, y, and z axes.
- the transform property accepts a handful of different values. The `rotate` value provides the ability to rotate an element from 0 to 360 degrees. `transform: rotate(20deg);`
- using the `scale` value within the transform property, you can change the appeared size of an element. `transform: scale(.75);`
- using `translateX` will change the position of an element on the horizontal axis.
- using `translateY` will change the position of an element on the vertical axis.
- `skew` is used to distort elements on the page, used similarly like translate.
- in order for three-dimensional transforms to work, you need to change the perspective with the `perspective` value. Three deminsional tranforms also need to work with all three axes.

## CSS Transitions

- in order for a **transition** to take place, an element must have a change in state, and different styles must be identified for each state.
- `transition-duration` can be used in seconds and milliseconds.
- `transition-timing-function` is a property used to set the speed in which a transition wil move.
- `transition-delay` is a property used to set the delay in the transition.
- to set multiple points at which an element should udergo a transition, use the @keyframes rule. The @keyframes rule includes the animation name, any animation breakpoints, and the properties intended to be animated.
- once the keyframes for an animation have been declared they need to be assigned to an element. To do so, the `animation-name` property is used with the animation name, identified from the `@keyframes` rule.

[<===Home](README.md)
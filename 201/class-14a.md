# CSS Transforms, Transitions and Animations


## Transform
The <transform> property makes possible new ways to position and alter elements.  It has two different settings, each with their own propeties and values:
- 2D
- 3D

#### Syntax is simple
`transform: value(specific amount)`

#### 2D transform (x and y axis)
- transform: rotate(30deg) -rotates element 20 degrees clockwise
- transform: scale(.75) -reduces element size to 75%
  - transform: scaleX(.75)
  - transform: scaleY(1.5)
- transform: translate(-10px, 25%) -moves element a specific distance on each axis
  - transform: translateX(-10px)
  - transform: translateY(25%)
- transform: skew(5deg, -20deg)
  - transform: skewX(5deg)
  - transform: skewY(-20deg)

- **Combinations**
  - transform: rotate(25deg) scale(.75)
  - transform: skew(10deg, 20deg) translateX(20px)

## Transitions and Animations

Transitions allow you to alter the appearance and behavior of an element on a state change, e.g. hovered.  There are four transition properties:
- transition-property
- transition-duration
- transition-timing-function
- transition-delay

*Example:*
  transition-property: background, border-radius;
  transition-duration: 1s;
  transition-timing-function: linear;

*Shorthand*
  transition: background .2s linear, border-radius 1s ease-in 1s

> **not all properties may be transitioned**, only properties that have an identifiable halfway point. Colors, font sizes, and the alike may be transitioned from one value to another as they have recognizable values in-between one another. The display property, for example, may not be transitioned as it does not have any midpoint.

---

[Back to table of contents](../README.md)
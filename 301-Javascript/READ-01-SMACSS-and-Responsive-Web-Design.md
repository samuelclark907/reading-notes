# Responsive Web Design

- Responsive web design is the practice of building a website suitable to work on every device and every screen size, no matter how large or small, mobile or desktop.

- Focused around creating the best experience for everyone.

- Ethan Marcotte coined the term "responsive web design".

## Responsive vs Adaptive vs Mobile

### Responsive

- To react quickly and positivley to any change.

- Continually change based on changing factors.

- This is the most popular technique and it utilizes all three.

### Adaptive

- To be easily modified for a new purpose or situation.

- Built to a group of preset factors.

### Mobile

- To build a seperate website for mobile users.

- Comes with dependencies of a new code base and browser sniffing.

## Flexible Layouts

- Responsive web design is broken down into three main components, flexible layouts, media queries, and flexible media.

- Flexible layouts is the practice of building the layout of a website with a flexible grid, capable of dynamically resizing to any width.

## Media Queries

- They provide the ability to specify different styles for individual browser and device.

- Most recomended way to use media queries is to use the @media rule inside of an existing style sheet.

- Media rule -  `@media all and (max-width: 1024px)`

- Import rule - `@import url(styles.css) all and (max-width: 1024px)`

## Mobile First

- The mobile first approach includes using styles targeted at smaller viewports as the default styles for a website, then use media queries to add styles as the viewport grows.

## Viewport

- Apple invented the meta tag to help with the size, scale and resolution of a website.

- For the best looking website, it is recommend that you use the device defaults by applying the device-height and device-width values.

- `<meta name="viewport" content="width=device-width">`

## Flexible Media

- Images, videos, and other media types need to be scalable, changing their size as the size of the viewport changes.

- Using the max-width property with a value of 100% ensures that as the viewport gets smaller any media will scale down according to its containers width.

# All About Floats

- Float is a position property in CSS.

- Commonly used to wrap text around an image.

- There are four valid values for the float property: left, right, none, inherit.

- If a parent element contains nothing but floated elements the height will collapse to nothing.

## Problems of Floats

### Pushdown

- Is a symptom of an element inside a floated item being wider than the float itself (typically an image).

- IE will expand the float to contain the image, often drastically affecting layout.

### Double Margin Bug

-  If you apply a margin in the same direction as the float, it will double the margin.





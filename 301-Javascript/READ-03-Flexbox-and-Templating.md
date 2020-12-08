# Read: 03 - Flexbox and Templating

## Javascript Templating

- Javascript templating is a fast and efficient technique to render client-side view templates with Javascript by using a JSON data source.

## Mustache

- Mustache is a logic-less template syntax. It can be used for HTML, .config files, source code.

- It works by expanding tags in a template using values provided in a hash or object.

## Flexbox

- Defines flex container.

- `.container {
  display: flex; /* or inline-flex */
}`

- `flex-direction` - defines the main axis which defines the direction.

- `.container {
  flex-direction: row | row-reverse | column | column-reverse;
}`

- `flex-wrap` - By default, flex items will all try to fit onto one line. You can change that and allow the items to wrap as needed with this property.

- `flex-flow` - This is a shorthand for the `flex-direction` and `flex-wrap` properties, which together define the flex container’s main and cross axes.

`justify-content` - This defines the alignment along the main axis.

`flex-grow` - This defines the ability for a flex item to grow if necessary.

`flex-shrink` - This defines the ability for a flex item to shrink if necessary.

`flex-basis` - This defines the default size of an element before the remaining space is distributed.
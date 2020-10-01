# JQUERY

- jQuery is a JS file that you put in your web pages. Allows you to find elements using style selectors and then use jQuery methods to modify them.

- jQuery makes it easier to handle events because the event methods work across all browsers. 

- jQuery offers methods that make it quick and simple to achieve a range of tasks that JavaScript programmers
commonly need to perform. 

### Find an element with css-style selectors.

- The `jQuery()` function lets you find elements on a page.

- It creates an object which holds refrences to those elements.

- Short hand `jQuery()` = `$()`.

- The jQuery object has a lot of methods.

### Key differences from the DOM

- Selectin elements is simpler because of the CSS-style syntax and its more accurate.

- Additional methods are provided for popular required tasks.

### Why use JQUERY?

- jQuery doesn't do anything you cannot achieve with pure JavaScript. It is just a JavaScript file but estimates show it has been used on over a quarter of the sites on the web, because it makes coding simpler. 

- Simple selectors.

- Common tasks in less code.

- jQuery's motto is "Write less, do more." 

### Looping

- With jQuery, when a selector returns multiple elements, you can update all of them using the one method. There is no need to use a loop. 

### Chaining

- You can list several methods at a time using dot notation to separate each one.

- `$('li [id!="one"]').hide().delay(5OO).fadeln(1400); `

### Getting element content

- The `.html()` and `.text()` methods both retrieve and update the content
of elements. 

- `.html()` -  retrieves only the HTML inside the first element in the matched set, along with any of its descendants. 

- `.text()` -  returns the content from every element in the jQuery selection, along with the text
from any descendants. 

### Getting and setting attribute values.

- You can create attributes, or access and update their contents, using the following four methods. 

- `.atr()` - This method can get or set a specified attribute and its value. 

- `.removeAttr()` - This method removes a specified attribute (and its value). 

- `.aaddClass()` - This method adds a new value to the existing value of the class attribute.

- `.removeClass()` - This method removes a value from the cl ass attribute, leaving any other class names within that attribute intact.

### CSS

- The `.css()` method lets you retrieve
and set the values of CSS properties. 

### Event Methods

- The `.on()` method is use to handle all events .


# 6 Reasons for Pair Programming

1. Greater efficiency

- When two people focus on the same code base, it is easier to catch mistakes in the making. 

- Studies show that PP usually takes longer but produces higher quality code.

2. Enagaged collaboration

- When two people are focused on the same code both people will be more focused than if they were working alone.

3. Learning from fellow students

- Everybody has a different point of view. Working with someone like that can help you expand your point of view.

4. Social skills

- Working with someone forces you to sharpen your communication skills.

5. Job interview readiness

- A common step in many interview processes involves pair programming between a current employee and an applicant.

- So having experince PP will be helpful in the interview process.

6. Work environment readiness

- People who are already familiar with how pairing works can hit the ground running at a new job, with one less hurdle to overcome.
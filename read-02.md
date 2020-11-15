# Read 02

## jQuery

jQuery is a JavaScript library that uses CSS selectors to find and select elements and then perform tasks on these elements. jQuery doesn't do anything you cannot achieve with pure JavaScript. It is just a JavaScript file that makes coding simpler. jQuery's motto is "Write less, do more," because it allows you to achieve the same goals but in fewer lines of code than you would need to write with plain JavaScript. jQuery's CSS-style selector syntax makes it easier to select elements to work with. It also has methods that make it easier to traverse the DOM. jQuery makes it easier to handle events because the event methods work across all browsers. jQuery offers methods that make it quick and simple to achieve a range of tasks that JavaScript programmers
commonly need to perform.

You can get the element content in jQuery using these two mehtods:

1. `.html()`
2. `.text()`

You can update and the content of all elements in jQuery selection using the following method:

1. `.html()`
2. `.text()`
3. `.replaceWith()`
4. `.remove()`

You can also create attributes, or access and update their contents, using the following four methods:

1. `.attr()`
2. `.removeAttr()`
3. `.addClass()`
4. `.removeClass()`

You can also insert elements by first, creating them and  Once you have a variable holding th~ new content, you can use the
following methods to add the content to the DOM tree:

1. `.before()`
2. `.after()`
3. `.prepend()`
4. `.append()`

Example:

```javascript

$(':header').addClass('headline');
$('li: lt(3)').hide(). fadeln(1500);
$('li').on('click', function() {
    $(this).remove();
} ) ;

```

## Pair Programmin

Pair programming is the practice of two developers sharing a single workstation to interactively tackle a coding task together. While there are many different styles, pair programming commonly involves two roles: the Driver and the Navigator. The Driver is the programmer who is typing and the only one whose hands are on the keyboard. Handling the “mechanics” of coding, the Driver manages the text editor, switching files, version control, and—of course writing—code. The Navigator uses their words to guide the Driver but does not provide any direct input to the computer. The Navigator thinks about the big picture, what comes next, how an algorithm might be converted in to code, while scanning for typos or bugs.

Pair programming touches on all four skills: developers explain out loud what the code should do, listen to others’ guidance, read code that others have written, and write code themselves.

6 Reasons for Pair Programming:

1. When two people focus on the same code base, it is easier to catch mistakes in the making.
2. When two programmers focus on the same code, the experience is more engaging and both programmers are more focused than if they were working alone. It is harder to procrastinate or get off track when someone else is relying on you to complete the work.
3. If one developer has a unique approach to a specific problem, pair programming exposes the other developer to a new solution.
4. Pair programming is great for improving social skills. When working with someone who has a different coding style, communication is key. This can become more difficult when two programmers have different personalities.
5. The ability to work with and learn from others and stellar communication skills are as (or more!) important to a company than specific technical skills.
6. Many companies that utilize pair programing expect to train fresh hires  on how they operate to actually deliver a product.

[Back to Home](README.md)

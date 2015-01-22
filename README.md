BASE6
=====
Reset + Classless Styles for Developers
---------------------------------------

###Intro

**WIP** - Simply a way to reset all styles (without unncessary reset bloat) to 'even the playing field' for how browsers display the most basic elements. Then, one can apply the optional 'Base6' (basics) styles that apply simple, but design friendly styles to the basic elements.

These styles are classless -- that is, it applies styles without use of classes or specific IDs -- making for easy use of good-looking web elements for developers, specifically back-end developers who do not wish to go through the learning, sorting, and searching that most style frameworks require (Bootstrap, Foundation, etc).

At the same time, the ultimate goal is to allow use of a framework of one's choice on top of the reset and base6 styles, allowing for easy 'drag and drop' functionality that will display the same across all modern browsers.

###To Use

+ **Use the `reset.css` as a low-weight reset file.** This reset has the added benefit of resetting form elements better than most others.
+ **Use `base6.css`** for quick clean styles without the need to memorize special HTML structures or classes.
+ Profit. Or use any framework of your choice on top of these.

###Elements

The main focus of the reset centers around form elements. These are the elements that vary the most from browser to browser. I have been ultimately successful in making the form elements behave the same across all browsers, but there are a few caveats that are, as of now, unavoidable:

+ IE9 doesn't allow full overwrite of `<select>` style.
+ In order to style radio buttons, checkboxes and file upload without the use of javascript, it was necessary to partner these elements with a `<label>`. The element must have an ID name, and the label must call that ID. Example:
`<input id="radio1" type="radio"><label for="radio1">[Radio Title]</label>`
+ The base6 css overwrites the file input default. Therefore it will not display the filename uploaded without additional JS.

###To Note

This is WIP, and as such a couple of things to point out:
+ Doesn't specifically support IE8. Most things work, but a full support may be forthcoming.
+ Not tested with frameworks yet. Not sure how it plays with Bootstrap, etc. Next step in the process
+ Not all elements were reset. This was to save space, and only focus on the most common elements.
+ Not all elements were styled in base6. Same reason as above.
+ Sass versions forthcoming.
+ Not minified, optimized, etc. File sizes are small by default, though.

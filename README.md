# What The Flexbox
CSS Flexbox Layout Module
The Flexible Box Layout Module, makes it easier to design flexible responsive layout structure without using float or positioning.

reference:
 - http://flexbox.io/
 - https://www.w3schools.com/css/css3_flexbox.asp
 - https://css-tricks.com/snippets/css/a-guide-to-flexbox/

## 1.Introduction to Flexbox
 **Make it RWD easily.**
```
.container {  
	display: flex;  /* or inline-flex */  
}
```

## 2.Working with Flexbox flex-direction
**flex direction control the layout, default is `row`.**
```
.container {  
	flex-direction: row | row-reverse | column | column-reverse;
}
```

## 3.Wrapping elements with Flexbox
**flex wrap control the layout, default is `nowrap `** (single-line which may cause the container to overflow).
```
.container {
	flex-wrap: nowrap | wrap | wrap-reverse;
}
```

## 4.Flexbox Ordering
```
.item {
	order: <integer>;  /* default is 0 */
}
```

## 5.Flexbox justify-content
Alignment and Centering with justify-content.According to the **main axis**.
```
.container {
	justify-content: flex-start | flex-end | center | space-between | space-around | space-evenly;
}
```

## 6.Flexbox align-items
Alignment and Centering with align-items.According to the **cross axis**.
```
.container {
	align-items: flex-start | flex-end | center | baseline | stretch;
}
```

## 7.align-content
Alignment and Centering with align-content.For the **content inside** the flex item.
```
.container {
	align-content: flex-start | flex-end | center | space-between | space-around | stretch;
}
```

## 8.align-self
Alignment and Centering with align-self.
```
.item {
	align-self: auto | flex-start | flex-end | center | baseline | stretch;
}
```

## 9.Flexbox Box-sizing
When there has extra space it will auto resize the element, and the default size of element is flex 1.
```
.item {
	flex:1;
}
```

## 10.Flexbox flex-grow, flex-shrink and flex-basis
flex: 1 >> is a shorthand of properties below.
```
.item {
	flex-grow: 1;
	flex-shrink: 1;
	flew-basis: 1;
}
```

## 11.Flexbox flex-basis and wrapping work together
The container flex-direction, flex-warp will work with the flex-grow, flex-shrink, flex-basis.
## 12.Cross Browser Flexbox Support and Autoprefixer
Autoprefixer for the CSS Flexbox to support different version of browsers.

 - Install the `node`, `nmp init` (in your project)
 - Install `gulp -g`, `touch gulp.js`(create a file)
 - Install `gulp --save-dev`, Install `gulp-autoprefixer --save-dev`
 - Setting up gulp.js and auto build.

## 13.Pure Flexbox navigation code along
We can build a PWD navigation menu bar with pure Flexbox.

## 14.Mobile content reordering with Flexbox
Use Media Queries to reordering the Flexbox items.
```
@media all and (max-width:500px) {
	/* Reorder items */
	.wrapper > * {
		order:999;
	}
	/* Nav */
	.flex-nav {
		order:1; /* Default is 0, and it will order first */
	}
}
```

## 15-Nesting Flexbox for vertical and horizontal centering with Flexbox
Nesting Flexbox elements with **justify-content**,  **align-items**, **align-content**.

## 16-Flexbox Pricing Grid
Using Flexbox with **flex-wrap** to control the layout in multi-lines.

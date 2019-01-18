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
**flex wrap control the layout, default is `nowrap `.**
```
.container {
	flex-wrap: nowrap | wrap | wrap-reverse;
}
```
## 4-Flexbox Ordering
```
.item {
	order: <integer>;  /* default is 0 */
}
```

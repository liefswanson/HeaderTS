# HeaderTS
A very simple, and as far as I can tell, flawless auto-hiding header implemented in typescript, with a JQuery dependency.

JQuery and typescript definitions not included.

## Useage

Has a JQuery dependency, get over it.

If you are not using typescript, simply compile the .ts file using a typescript compiler, and put it in your project as a javascript file. Include it in your html and it will make your header hide automagically when you scroll as long as you label it with id="header"

If you are using typescript, you will need some JQuery definitions, but other than that, you should simply be able to include it in your file.

additionally everyone will need to add the following css to the element they choose to have as their header element.

```
#header {
	position: fixed;
	top: 0;
	left: 0; // don't want it all the way to the left? that can be changed
	height: 4rem; // you pick the height here
	width: 100%; // if you don't want the width to be 100% it can be changed
	background: black; // change the color if you like, it is just there so it is visible
	z-index: 100; // presumably you want the header on top. If you go above 100 you may need to increase this
}
```

## features
- [ ] No dependencies (sorry)
- [x] works without writing a single line of javascript
- [x] only does updates on page scroll events and on page load
- [x] loading mid way scrolled through a page will hide the bar
- [x] customizable animation time, and target

## untested scenarios

The only scenario I can think of that I have not tested for is when clicking a link that causes a scroll event. However, I don't think it would be a problem. If it is, show me the code and maybe I can help.

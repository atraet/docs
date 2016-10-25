
### Viewport

	<meta name="viewport" content="width=device-width, initial-scale=1">


### Simplifying Designs for Print

use media print to hide header and sidebar etc


### HTML and CSS Media Queries

3 ways to write media query css styles

	<link rel="styleshet" href="print.css" media="print />


	@import url('print.css') print;
	

	@media print {
		// styles goes here
	}

### Media types

- all
- screen
- print

- etc..


### Max-Width Media Queries

Media feature vs media type

Media features

- max-width
- min-width
- etc.


### Making the menu animate

### Logical operators

- and
- ,  (== or, there is no <s>or</s> operator)
- not
- only (not used very often)

**not** is the last operator being evaluated, see example:

	@media not print and (min-width: 300px){ ... }

### Resolution features

- -webkit-

webkit browsers: chrome

### Orientation and Aspect ratio

- orientation
- min-aspect-ratio: 1/1 = (orientation: portait)
- max-aspect-ratio: 1/1 = (orientation: landscape)

### More media query features

- @media (min-device-width: 300px) { ... }
- @media (min-color: 1) { ... }
- @media (min-color-index: 256) { ... }
- @media (monochrome) { ... }
- @media (scan: progressive) { ... }
- @media (grid) { ... }

### Animating on Breakpoints

	transition: .5s width ease

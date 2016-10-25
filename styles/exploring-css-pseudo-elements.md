## Introduction

### Pseudo classes vs Pseudo elements

#### Pseudo classes

- Target elements that match a certain **criteria** or **state**
- The name of the pseudo class is preceded by a single colon **:**
- Common pseudo classes
	- :hover
	- :first-child
	- :nth-child
	- :not()

#### pseudo elements

- Generally target a certain **part** of an element
- The name of the pseudo class is preceded by two colons **::**
- Common pseudo elements
	- ::before
	- ::after
	- ::first-letter
	- ::first-line
	- ::selection

IE 8 does not support ::-syntax, use : to start with pseudo elements instead.

## How to use Pseudo elements

#### ::before and ::after

examples:

- add icon text before
- add checked icon after item of a list
- speech bubble icon


you can insert text, image before and after element

- [Speech bubbles with ::before and ::after](http://nicolasgallagher.com/pure-css-speech-bubbles/demo/)
- [Pure CSS GUI icons](http://nicolasgallagher.com/pure-css-gui-icons/)


#### ::selection
example: highlighting slected text

#### ::backdrop

only supported by Chrome at this moment.

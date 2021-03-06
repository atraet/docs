## 1 Introduction

## 2 Selectors

### Basic selectors, relational selectors

- ID
- Class
- Tag name

#### Relational selectors

- ul li  (descendant)
- ol > li  (child)
- li.myClass + li  (adjacent sibling)
- li.myClass ~ li  (general sibling)

### Attribute selectors

'class' attribute is case-sensitive

- E[attr]
- E[attr  = val]  
- E[attr != val] (start with [dash])
- E[attr ~= val] (space separated full word)
- E[attr ^= val]
- E[attr $= val]
- E[attr *= val]

NOTE: multiple attributes work a[title][href]

Decorate mail link with icon

	a[href ^= mailto] {background-image: url(emailicon.gif); }

For print

	a[href ^= http]::after {content:  " attr(href) "; }

Decorate PDF link

	a[href $=pdf] {background-image: url(pdficon.gif); }
	a[href $=pdf]::after {content: "(pdf)"; }

### UI Pseudo classes

#### Based on current state of UI

- :enabled
- :disabled
- :checked

Make checked check-box label red

	input[type=checkbox]:checked + labed {color: red; }

#### Form related UI Pseudo-classes

- :valid
- :invalid
- :required
- :optional

- :in-range
- :out-of-range
- :read-only
- :read-write

- :default

- :contenteditable: behavior like a form but it is not a form

### Structural UI Pseudo-classes

- first-of-type
- first-child

Use CSS to draw US flag


### Navigation and empty pseudo-classes

- :not
- :empty

### Other pseudo-classes

- :lang
- :target

- :root

#### link & user action pseudo-classes

Do not use following 2 classes due to security reasons

- :link
- :visited

- :hover
- :active
- :focus

### Pseudo elements

- ::before
- ::after
- etc

jQuery $(selector) == **document.querySelectorAll(selector)**

Many, many more pseudo-elements with prefixes currently treated as a **shadow DOM**

- ::-webkit-progress-bar
- ::-webkit-meter-even-less-goood-value
- etc..

## 3 Specificity

- ID      100
- Class   010
- Element 001


## 4 Generated Content

Use cases

- Decorate tel, url, mail with icons
- Decorate blockquote/ text /paragraph with quotation marks
- Show url on mouse over a link
- Draw geometric shapes
- etc

## 5 Media queries

Media query syntax/punctuation

- only
- and
- not
- ,

## 6 Debugging

Mobile debugging

using npm package **weinre**

shadow dom

- ::-webkit-scrollbar {}
- ::-webkit-scrollbar-track{}
- and many many more

use debugger as a learning tool


## 7 Colors

What color is transparent: transparent **black**

CurrentColor:

## 8 Fonts, Shadows and Text Effects

To be back to review

## 9 Borders and Backgrounds

## 10 Gradients

## 11 Transforms

## 12 Transitions and Animations

## 13 Other CSS Features

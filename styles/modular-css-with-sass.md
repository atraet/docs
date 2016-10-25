# 1 Getting Modular with Mixins and Functions

## Configuration
- font
- color

```css
@if variable-exists(font-url--google){

}
```

Calculate em values

```css
@function em($target, @context: $base__font-size){
  @return ($target / $base__font-size) * 1em
}

```

# 2 SASS and BEM

## Then BEM pattern


We need to think in terms of abstraction layers for blocks, elements and modifiers

## Using BEM in our project

example
- nav
- nav__item
- nav__item--current

Only downside of BEM: long class name

## BEM Mixins

```css
@mixin e($element){
  &__#{$element}{
    @content;
  }
}
```

Reuse css definition by using placeholders (in file extends.scss)


# 3 SMACSS and SASS

## What is SMACSS

Style guide that helps organize and structure CSS for projects on any scale.

It also aims to identify repeating patterns in the code that are then combined into modular components.

SMACC categories
- Base
- Layout
- Modules
- States
- Themes

## SMACSS in our workflow

SMACSS is not a framework, but a style guide

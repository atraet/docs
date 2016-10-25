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

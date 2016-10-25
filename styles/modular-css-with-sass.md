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

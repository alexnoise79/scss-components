# scss-components
### sass mixin to generate checkbox and radio buttons from a minumim template with svg
## [Based on Ryan Seddon's solution](http://www.thecssninja.com/css/custom-inputs-using-css)
* works with ie9+ with graceful degradation in previous browser
# @params !WARNING USE UNESCAPED STRINGS
 ```scss
$type
```
could be checkbox or radio
 ```scss
$dim
```
the dimension (square) of the component

# SVG (base64)
 ```scss
 $unchecked
 ```
the default state
```scss
$checked
```
checked state
```scss
$unchecked-hover
```
hovered image
```scss
$unchecked-disabled
```
disabled unchecked image
 ```scss
 $checked-disabled
 ```
 disabled checkd image
 ```scss
 [$unchecked-active]
 ```
 __OPTIONAL__ unchecked active image
 ```scss
 [$checked-active]
 ```
 __OPTIONAL__ checked active
 ```scss
 [$indeterminate]
 ```
 __OPTIONAL__ only for checkbox three state image
 
 # MINIMAL TEMPLATE
 
```html
 <span class="cb || rb"><input id type="$type"/><label for="x"></label></span> [<label for="x">text here</label>]
```
# Example
```scss
@include components(checkbox, 18px, $cb-unchecked, $cb-checked, $cb-unchecked-hover, $cb-checked-hover, $cb-unchecked-disabled, $cb-checked-disabled, $cb-unchecked-active, $cb-checked-active, $cb-indeterminate);

@include components(radio, 18px, $rb-unchecked, $rb-checked, $rb-unchecked-hover, $rb-checked-hover, $rb-unchecked-disabled, $rb-checked-disabled, $rb-unchecked-active, $rb-checked-active);
```

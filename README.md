# scss-components
sass mixin to generate checkbox and radio buttons from a minumim template


 Based on Ryan Seddon's solution --> http://www.thecssninja.com/css/custom-inputs-using-css
 //    * works with ie9+ with graceful degradation in previous browser
 //
 //    @params !WARNING USE UNESCAPED STRINGS
 //    * $type could be checkbox or radio
 //    * $dim the dimension (square) of the component
 //
 //    * IMAGES (without extension)
 //    * $unchecked            the default state
 //    * $checked              checked state
 //    * $unchecked-hover                hovered image
 //    * $unchecked-disabled   disabled unchecked image
 //    * $checked-disabled     disabled checkd image
 //    * [$unchecked-active]   OPTIONAL unchecked active image
 //    * [$checked-active]     OPTIONAL checked active
 //    * [$indeterminate]      OPTIONAL only for checkbox three state image
 //
 //    * MINIMAL TEMPLATE
 //    * <span class="cb || rb"><input id type="$type"/><label for></label></span>

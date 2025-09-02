# How end value of a property is calculated?

Values of almost all properties of (especially animation) sequentials are calculated by some inputs. Here you'll find how it works.


## End Value Type

This option determines the calculation of the end value of the related property.

### Initial to Value

This changes the related property from its initial value (the value before this sequential starts) to the __Value__.


### From Value to Initial

This sets the property value to the __Value__ and then changes it to its initial value again.

### Initial Plus Value

This adds __Value__ to the initial property value and changes it to the calculated value.


### Initial Multiply Value

This multiplies the related property's initial value with the  __Value__ and changes the to the calculated value.

For Vector properties, it will multiply each component (x*x, y*y, z*z) and then creates a new Vector from this calculated value. 

### From A to B

This lets you define the starting value and end value of the animation independent from the initial value of the property.


## Value

This is the value that determines the end property value in accordance with the __End Value Type__ option as explained above.

It's possible to assign different kind of values to this property (e.g. directly, randomly, from variable).


!!! info
    To learn more about assigning values with different options, see [Value Assign](valueassign.md)

## From Value

This is only available when the __End Value Type__ is __From A to B__.

This is the starting property value of the animation.

# Change Light Range


This sequential lets you change the range of a Light component with animation.

!!! tip
    This does not apply to Directional lights.

!!! note "Base Properties"
    To learn about the common Base Properties, please see [Base Sequential](../sequential_base.md)

!!! note "Target Object Options"
    This sequential derives from __Object Returner Sequential__ and gets all its properties from that sequential. So, to learn about the __Target Object Options__ please see [Object Returner Sequential](../sequentialobjectreturner/index.md)

!!! note "Animation Options"
    This sequential derives from __Animation Sequential__ and gets all of its properties. So, to learn about the __Animation Options please see [Animation Base](index.md)

!!! warning "Target Object"
 
    Target Object (or Target Objects if Multiple Objects are returned) needs to be Light type. So please make sure that the game object assigned in this field has a Light component attached. Otherwise you'll see a runtime error log when this sequential plays.



## End Value Type

This option determines the calculation of the end value of the light range.

### Initial to Value

This changes the light range from its initial value (the value before this sequential starts) to the __Range__.


### From Value to Initial

This sets the light range to the __Range__ and then changes it to its initial value again.

### Initial Plus Value

This adds __Range__ to the initial light range and changes it to the calculated value.


### Initial Multiply Value

This multiplies the light range's initial value with the  __Range__ and changes the to the calculated value.

### From A to B

This lets you define the starting range and end range of the animation independent from the initial value of the light range.



## Range


This is the value that determines the end light range in accordance with the __End Value Type__ option as explained above.

It's possible to assign different kind of values to this property (e.g. directly, randomly, from variable).


!!! info
    To learn more about assigning values with different options, see [Value Assign](../../valueassign.md)


## From Range

This is only available when the __End Value Type__ is __From A to B__.

This is the starting range value of the animation.
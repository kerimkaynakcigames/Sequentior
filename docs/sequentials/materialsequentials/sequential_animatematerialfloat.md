# Material Float Property Animator Sequential

![Material Float Animator Sequential](/img/sequential_materialfloatanimator.jpg)

This sequential lets you modify any float property of a material, so it's a very powerful sequential that can be used for general animation purposes for shaders that expose a float property.

For example, you can use it to change the __Smoothness__ property of a shader.

!!! note "Base Properties"
    To learn about the common Base Properties, please see [Base Sequential](../sequential_base.md)

!!! note "Target Object Options"
    This sequential derives from __Object Returner Sequential__ and gets all its properties from that sequential. So, to learn about the __Target Object Options__ please see [Object Returner Sequential](../sequentialobjectreturner/index.md)

!!! note "Animation Options"
    This sequential derives from __Animation Sequential__ and gets all of its properties. So, to learn about the __Animation Options please see [Animation Base](../animationsequentials/index.md)

!!! note "Material Options"
    This sequential derives from __Material Sequential__ and gets all of its properties. So, to learn about the __Material Options__ please see [Material Base](index.md)

## End Value Type

This option determines the calculation of the end value of the float property.

### Initial to Value

This modifies the target shader property from its initial value (the value before this sequential starts) to the __Value__.


### From Value to Initial

This sets the target shader property to the __Value__ and then modifies it to its initial value again.

### Initial Plus Value

This adds __Value__ to the target shader property's initial value and modifies it to the calculated end value.


### Initial Multiply Value

This multiplies the shader property's initial value with the __Value__ and modifies the target shader property to the calculated value.

### From A to B

This lets you define the starting value and end value of the float animation independent from the initial value of the target shader property.


## Value

This is the float value that determines the end value in accordance with the __End Value Type__ option as explained above.

It's possible to assign different kind of values to this property (e.g. directly, randomly, from variable).


!!! info
    To learn more about assigning values with different options, see [Value Assign](../../valueassign.md)
 

## From Value

This is only available when the __End Value Type__ is __From A to B__.

This is the starting value of the float animation.

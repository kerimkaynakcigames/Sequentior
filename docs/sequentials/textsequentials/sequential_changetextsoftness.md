# Change Text Softness Sequential

![Softness](/img/sequential_textsoftness.jpg)

This sequential will change the Softness property of a TextMeshPro component with animation.


!!! note "Base Properties"
    To learn about the common Base Properties, please see [Base Sequential](../sequential_base.md)

!!! note "Target Object Options"
    This sequential derives from __Object Returner Sequential__ and gets all its properties from that sequential. So, to learn about the __Target Object Options__ please see [Object Returner Sequential](../sequentialobjectreturner/index.md)

!!! note "Animation Options"
    This sequential derives from __Animation Sequential__ and gets all of its properties. So, to learn about the __Animation Options please see [Animation Base](index.md)

!!! warning "Target Object"
 
    Target Object (or Target Objects if Multiple Objects are returned) needs to be TextMeshPro type. So please make sure that the game object assigned in this field has a TextMeshPro component attached. Otherwise you'll see a runtime error log when this sequential plays.

## End Value Type

This option determines the calculation of the end value of the softness.

### Initial to Value

This modifies the target text's softness from its initial value (the value before this sequential starts) to the __Softness__.


### From Value to Initial

This sets the target text's softness to the __Softness__ and then modifies it to its initial value again.

### Initial Plus Value

This adds __Softness__ to the target text's initial softness and modifies it to the calculated end value.


### Initial Multiply Value

This multiplies the text's initial softness with the __Softness__ and modifies the target text's softness to the calculated value.

### From A to B

This lets you define the starting softness and end softness of the animation independent from the initial softness of the target text.


## Softness

This is the softness that determines the end softness in accordance with the __End Value Type__ option as explained above.

It's possible to assign different kind of values to this property (e.g. directly, randomly, from variable).


!!! info
    To learn more about assigning values with different options, see [Value Assign](../../valueassign.md)
 

## From Softness

This is only available when the __End Value Type__ is __From A to B__.

This is the starting softness of the animation.


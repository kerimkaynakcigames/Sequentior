# Change Text Dilate Sequential

![Dilate](../../img/sequential_textdilate.jpg)

This sequential will change the Dilate property of a TextMeshPro component with animation.


!!! note "Base Properties"
    To learn about the common Base Properties, please see [Base Sequential](../sequential_base.md)

!!! note "Target Object Options"
    This sequential derives from __Object Returner Sequential__ and gets all its properties from that sequential. So, to learn about the __Target Object Options__ please see [Object Returner Sequential](../sequentialobjectreturner/index.md)

!!! note "Animation Options"
    This sequential derives from __Animation Sequential__ and gets all of its properties. So, to learn about the __Animation Options please see [Animation Base](index.md)

!!! warning "Target Object"
 
    Target Object (or Target Objects if Multiple Objects are returned) needs to be TextMeshPro type. So please make sure that the game object assigned in this field has a TextMeshPro component attached. Otherwise you'll see a runtime error log when this sequential plays.

## End Value Type

This option determines the calculation of the end value of the dilate.

### Initial to Value

This modifies the target text's dilate from its initial value (the value before this sequential starts) to the __Dilate__.


### From Value to Initial

This sets the target text's dilate to the __Dilate__ and then modifies it to its initial value again.

### Initial Plus Value

This adds __Dilate__ to the target text's initial dilate and modifies it to the calculated end value.


### Initial Multiply Value

This multiplies the text's initial dilate with the __Dilate__ and modifies the target text's dilate to the calculated value.

### From A to B

This lets you define the starting dilate and end dilate of the animation independent from the initial dilate of the target text.


## Dilate

This is the dilate that determines the end dilate in accordance with the __End Value Type__ option as explained above.

It's possible to assign different kind of values to this property (e.g. directly, randomly, from variable).


!!! info
    To learn more about assigning values with different options, see [Value Assign](../../valueassign.md)
 

## From Dilate

This is only available when the __End Value Type__ is __From A to B__.

This is the starting dilate of the animation.


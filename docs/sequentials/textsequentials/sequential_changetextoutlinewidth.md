# Change Text Outline Width Sequential

![Outline Width](/img/sequential_textoutlinewidth.jpg)

This sequential will change the Outline Width property of a TextMeshPro component with animation.


!!! note "Base Properties"
    To learn about the common Base Properties, please see [Base Sequential](../sequential_base.md)

!!! note "Target Object Options"
    This sequential derives from __Object Returner Sequential__ and gets all its properties from that sequential. So, to learn about the __Target Object Options__ please see [Object Returner Sequential](../sequentialobjectreturner/index.md)

!!! note "Animation Options"
    This sequential derives from __Animation Sequential__ and gets all of its properties. So, to learn about the __Animation Options please see [Animation Base](index.md)

!!! warning "Target Object"
 
    Target Object (or Target Objects if Multiple Objects are returned) needs to be TextMeshPro type. So please make sure that the game object assigned in this field has a TextMeshPro component attached. Otherwise you'll see a runtime error log when this sequential plays.

## End Value Type

This option determines the calculation of the end value of the outline width.

### Initial to Value

This modifies the target text's outline width from its initial value (the value before this sequential starts) to the __Outline Width__.


### From Value to Initial

This sets the target text's outline width to the __Outline Width__ and then modifies it to its initial value again.

### Initial Plus Value

This adds __Outline Width__ to the target text's initial outline width and modifies it to the calculated end value.


### Initial Multiply Value

This multiplies the text's initial outline width with the __Outline Width__ and modifies the target text's outline width to the calculated value.

### From A to B

This lets you define the starting outline width and end outline width of the animation independent from the initial outline width of the target text.


## Outline Width

This is the outline width that determines the end outline width in accordance with the __End Value Type__ option as explained above.

It's possible to assign different kind of values to this property (e.g. directly, randomly, from variable).


!!! info
    To learn more about assigning values with different options, see [Value Assign](../../valueassign.md)
 

## From Outline Width

This is only available when the __End Value Type__ is __From A to B__.

This is the starting outline width of the animation.


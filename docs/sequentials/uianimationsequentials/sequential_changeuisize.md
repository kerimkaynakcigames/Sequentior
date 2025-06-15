# Change UI Size

![Change UI Size](/img/sequential_changeuisize.jpg)

This sequential changes the size of a UI element by modifying its __sizeDelta__ property. This is different from [Scale Animation](../animationsequentials/sequential_scale.md) because it changes the scale but this changes the size while keeping the scale as it is.

!!! note "Base Properties"
    To learn about the common Base Properties, please see [Base Sequential](../sequential_base.md)

!!! note "Target Object Options"
    This sequential derives from __Object Returner Sequential__ and gets all its properties from that sequential. So, to learn about the __Target Object Options__ please see [Object Returner Sequential](../sequentialobjectreturner/index.md)

!!! note "Animation Options"
    This sequential derives from __Animation Sequential__ and gets all of its properties. So, to learn about the __Animation Options please see [Animation Base](../animationsequentials/index.md)



## Size Change Type

This option determines the calculation of the end value of the size.

### Initial to Value

This resizes the target UI element from its initial value (the value before this sequential starts) to the __Size__.


### From Value to Initial

This sets the size of target UI element to the __Size__ and then changes it to its initial value again.

### Initial Plus Value

This adds __Size__ to the target UI element's initial sizeDelta value and changes it to the calculated sizeDelta value.


### Initial Multiply Value

This multiplies the UI element's initial sizeDelta value with the  __Size__ and changes the target UI element's sizeDelta to the calculated value.

### From A to B

This lets you define the starting size and end size of the Change UI Size animation independent from the initial size of the target UI element.

![From A to B](/img/sequential_changeuisize_ab.jpg)

## Size

This is the Width and Height value that determines the end size in accordance with the __Size Change Type__ option as explained above.

It's possible to assign different kind of values to this property (e.g. directly, randomly, from variable).


!!! info
    To learn more about assigning values with different options, see [Value Assign](../../valueassign.md)

## From Size

This is only available when the __Size Change Type__ is __From A to B__.

This is the starting size of the Change UI Size animation.



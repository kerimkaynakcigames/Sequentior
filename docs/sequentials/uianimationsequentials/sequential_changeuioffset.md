# Change UI Offset

![Change UI Offset](/img/sequential_changeuioffset.jpg)

This sequential changes the position of a UI element by modifying its __offsetMin__ and __offsetMax__ properties. 

!!! note "Base Properties"
    To learn about the common Base Properties, please see [Base Sequential](../sequential_base.md)

!!! note "Target Object Options"
    This sequential derives from __Object Returner Sequential__ and gets all its properties from that sequential. So, to learn about the __Target Object Options__ please see [Object Returner Sequential](../sequentialobjectreturner/index.md)

!!! note "Animation Options"
    This sequential derives from __Animation Sequential__ and gets all of its properties. So, to learn about the __Animation Options please see [Animation Base](../animationsequentials/index.md)



## Offset Change Type

This option determines the calculation of the end value of the offset.

### Initial to Value

This moves the target UI element from its initial value (the value before this sequential starts) to the __Offset__.


### From Value to Initial

This sets the position of target UI element by the __Offset__ and then changes it to its initial value again.

### Initial Plus Value

This adds __Offset__ to the target UI element's initial position value and changes it to the calculated position.


### Initial Multiply Value

This multiplies the UI element's initial position (offset values) with the  __Offset__ and changes the target UI element's offsets to the calculated value.

### From A to B

This lets you define the starting position and end position of the Change UI Offset animation independent from the initial position of the target UI element.

![From A to B](/img/sequential_changeuioffset_ab.jpg)

## Offset

This is the Left, Right, Top and Bottom positions that determines the end position in accordance with the __Offset Change Type__ option as explained above.

It's possible to assign different kind of values to this property (e.g. directly, randomly, from variable).


!!! info
    To learn more about assigning values with different options, see [Value Assign](../../valueassign.md)

## From Offset

This is only available when the __Offset Change Type__ is __From A to B__.

This is the starting position of the Change UI Offset animation.



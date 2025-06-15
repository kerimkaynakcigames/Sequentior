# Scale Sequential

![Scale Sequential](/img/sequential_scale.jpg)

This sequential scales a transform with animation.

!!! note "Base Properties"
    To learn about the common Base Properties, please see [Base Sequential](../sequential_base.md)

!!! note "Target Object Options"
    This sequential derives from __Object Returner Sequential__ and gets all its properties from that sequential. So, to learn about the __Target Object Options__ please see [Object Returner Sequential](../sequentialobjectreturner/index.md)

!!! note "Animation Options"
    This sequential derives from __Animation Sequential__ and gets all of its properties. So, to learn about the __Animation Options please see [Animation Base](index.md)

## Scale Type

This option determines the calculation of the end value of the scale action.

### Initial to Value

This scales the target transform from its initial value (the value before this sequential starts) to the __Scale Value__.


### From Value to Initial

This instantly sets the scale of the target transform to the __Scale Value__ and then scales it to its initial value again.

### Initial Plus Value

This adds __Scale Value__ to the target transform's initial scale value and scales it to the calculated value.


### Initial Multiply Value

This multiplies each axis of the transform's initial scale with the corresponding axis of the __Scale Value__ and scales the target transform to the calculated value.

### From A to B

This lets you define the starting scale and end scale of the scale animation independent from the initial scale of the target transform.

![From A to B](/img/sequential_scale_ab.jpg)

## Scale Value

This is the Vector3 value that determines the end scale in accordance with the __Scale Type__ option as explained above.

It's possible to assign different kind of values to this property (e.g. directly, randomly, from variable).

For example, to scale the target transform to the scale of another transform, you can select __Another Transform__ or __Sequential__ for the value assigning option and then choose the transform to match the scale.

!!! info
    To learn more about assigning values with different options, see [Value Assign](../../valueassign.md)

!!! tip
    When you assign Scale Value with __Sequential__ option, you need to connect the related sequential's Sequential output port to this sequential's __To Scale input port__. 

## From Scale

This is only available when the __Scale Type__ is __From A to B__.

This is the starting scale value of the scale animation.

!!! tip
    When you assign From Scale with __Sequential__ option, you need to connect the related sequential's Sequential output port to this sequential's __From Scale input port__. 





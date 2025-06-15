# Time Scale Sequential

![Time Scale](/img/sequential_timescale.jpg)

This sequential changes scale of time over time by modifying Time.timeScale.

!!! note "Base Properties"
    To learn about the common Base Properties, please see [Base Sequential](../sequential_base.md)

!!! note "Animation Options"
    This sequential derives from __Animation Sequential__ and gets all of its properties. So, to learn about the __Animation Options please see [Animation Base](../animationsequentials/index.md)

!!! warning
    Although this sequential derives from __Object Returner__ sequential, it does not use any of the __Target Object Options__.


## End Value Type

This option determines the calculation of the end value of the time scale.

### Initial to Value

This changes the time scale from its initial value (the value before this sequential starts) to the __Time Scale__.


### From Value to Initial

This instantly sets the time scale to the __Time Scale__ property and then changes it to its initial value again.

### Initial Plus Value

This adds __Time Scale__ to the initial time scale and changes it to the calculated value.


### Initial Multiply Value

This multiplies initial time scale with the __Time Scale__ and changes the time scale to the calculated value.

### From A to B

This lets you define the starting time scale and end time scale of the animation independent from the initial time scale.

## Time Scale

This is the float value that determines the end time scale in accordance with the __End Value Type__ option as explained above.

It's possible to assign different kind of values to this property (e.g. directly, randomly, from variable).


!!! info
    To learn more about assigning values with different options, see [Value Assign](../../valueassign.md)

## From Volume

This is only available when the __End Value Type__ is __From A to B__.

This is the starting time scale value of the animation.
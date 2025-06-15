# Float Animator Sequential

![Float Animator Sequential](/img/sequential_floatanimation.jpg)

This sequential lets you modify any float property of a component, so it's a very powerful sequential that can be used for general animation purposes for objects that expose a float property.

For example, although there is a specific sequential to change the alpha value of CanvasGroup component, you can also change (animate) it with this sequential. So it's useful when there is no built-in sequential to animate a value.

!!! note "Base Properties"
    To learn about the common Base Properties, please see [Base Sequential](../sequential_base.md)

!!! note "Target Object Options"
    This sequential derives from __Object Returner Sequential__ and gets all its properties from that sequential. So, to learn about the __Target Object Options__ please see [Object Returner Sequential](../sequentialobjectreturner/index.md)

!!! note "Animation Options"
    This sequential derives from __Animation Sequential__ and gets all of its properties. So, to learn about the __Animation Options please see [Animation Base](index.md)

## End Value Type

This option determines the calculation of the end value of the float property.

### Initial to Value

This modifies the target property from its initial value (the value before this sequential starts) to the __Value__.


### From Value to Initial

This sets the target property to the __Value__ and then modifies it to its initial value again.

### Initial Plus Value

This adds __Value__ to the target property's initial value and modifies it to the calculated end value.


### Initial Multiply Value

This multiplies the property's initial value with the __Value__ and modifies the target property to the calculated value.

### From A to B

This lets you define the starting value and end value of the float animation independent from the initial value of the target property.

![From A to B](/img/sequential_floatanimation_ab.jpg)

## Value

This is the float value that determines the end value in accordance with the __End Value Type__ option as explained above.

It's possible to assign different kind of values to this property (e.g. directly, randomly, from variable).


!!! info
    To learn more about assigning values with different options, see [Value Assign](../../valueassign.md)
 

## From Value

This is only available when the __End Value Type__ is __From A to B__.

This is the starting value of the float animation.

## Property Options

In this section, you can define the target float property.

### Component Name

This is the class name with full namespace of a component that is attached to the target object and that has the property to animate.

So, for example, to get SpriteRenderer component attached, you need to type _UnityEngine.SpriteRenderer, UnityEngine_.

!!! note "What's full type?"
    * For custom types, you can use the full class name with namespace. e.g. com.kerimkaynakcigames.MyGame.GameManager
    * For built-in types, write the class name and then put a comma (,) and then assembly name. e.g. UnityEngine.SpriteRenderer, UnityEngine

### Property Name

This defines the which property to animate.

So this is the main target property of this sequential.

e.g. __fillAmount__ property of an Image component.




# Call Method Sequential

![Call Method](/img/sequential_callmethod.jpg)

This sequential lets you call a method of a component attached to the Target Object.

!!! tip
    Although this seems similar to the [Unity Event Trigger Sequential](../eventtriggersequentials/sequential_unityeventtrigger.md), this lets you call methods with multiple parameters too. So if you just want to call a parameterless or single parameter method, you can use [Unity Event Trigger Sequential](../eventtriggersequentials/sequential_unityeventtrigger.md) alternatively.

!!! note "Base Properties"
    To learn about the common Base Properties, please see [Base Sequential](../sequential_base.md)

!!! note "Target Object Options"
    This sequential derives from __Object Returner Sequential__ and gets all its properties from that sequential. So, to learn about the __Target Object Options__ please see [Object Returner Sequential](../sequentialobjectreturner/index.md)

## Component Name

This is the class name with full namespace of a component that is attached to the target object.

So, for example, to call a method of a SpriteRenderer component attached, you need to type _UnityEngine.SpriteRenderer, UnityEngine_.

!!! note "What's full type?"
    * For custom types, you can use the full class name with namespace. e.g. com.kerimkaynakcigames.MyGame.GameManager
    * For built-in types, write the class name and then put a comma (,) and then assembly name. e.g. UnityEngine.SpriteRenderer, UnityEngine

## Method Name

This is the name of the method to call.

## Parameters

If the method you want to call needs parameters, you can set them in this list in exactly same order defined in the method itself.

### Parameter Type

This should match the data type of the parameter of the method.

### Parameter Value

This is the value of the parameter to send to the method to call.

This property is dynamic and changes its type according to the __Parameter Type__. 
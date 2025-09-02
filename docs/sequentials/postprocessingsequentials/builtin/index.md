# Post Processing for Built-in RP Sequentials

Sequentials in this category let you animate parameters of Post Processing effects for Built-in Render Pipeline. 

In this page, you'll find common properties of built-in post processing sequentials. Every other property of these sequentials reflects the same properties of corresponding post processing effect. To learn more about fields/properties of each post processing effect please refer to the [Unity Post-Processing Stack V2 Documentation](https://docs.unity3d.com/Packages/com.unity.postprocessing@3.5/manual/)

!!! warning "Setup Post Processing first"
    To use Post Processing related actions, you need to go to the [Setup](../../setup.md) screen and choose related options. Please see the [Setup documentation](../../setup.md) for more information.


!!! note "Base Properties"
    To learn about the common Base Properties, please see [Base Sequential](../../sequential_base.md)

!!! note "Target Object Options"
    This sequential derives from __Object Returner Sequential__ and gets all its properties from that sequential. So, to learn about the __Target Object Options__ please see [Object Returner Sequential](../../sequentialobjectreturner/index.md)

!!! note "Animation Options"
    This sequential derives from __Animation Sequential__ and gets all of its properties. So, to learn about the __Animation Options please see [Animation Base](../../animationsequentials/index.md)

!!! warning "Target Object"
 
    Target Object (or Target Objects if Multiple Objects are returned) needs to be PostProcessVolume type. So please make sure that the game object assigned in this field has a PostProcessVolume component attached. Otherwise you'll see a runtime error log when this sequential plays.


## Override Option

This option lets you enable or disable this specific post processing effect.

* __Leave as is__: This won't change the status of the effect. If it's currently enabled, it stays enabled. If it's currently disabled, it stays disabled.
* __Force Enable__: This force enables the effect even if it's currently disabled.
* __Force Disable__: This force disables the effect even if it's currently enabled.


## Enable Options

For each options, there are checkboxes enables modifying the related property. If you don't enable a property, it won't modify its values.

## End Value Calculation
    
To learn about how the end values of parameters are calculated, please refer [this section](../../../endvaluetypecalculation.md)
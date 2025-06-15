# Set GameObject Variable Sequential

![Set Variable](/img/sequential_setgameobjvar.jpg)

This sequential sets the value of a variable to the game object retured from __Seq Obj Input port__.


!!! note "Base Properties"
    To learn about the common Base Properties, please see [Base Sequential](../sequential_base.md)

## Variable Name

The variable name to set. 

!!! warning
    This variable name should exist in the Parent Sequentior's Variables List and its value type should be GameObject.

## Variable Obj

This is the sequential that has the game object value to assign to the variable. This field will be automatically filled when you connect an [Object Returner](../sequentialobjectreturner/index.md) sequential to the __Seq Obj Input Port__
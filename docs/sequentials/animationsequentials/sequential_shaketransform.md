# Shake Transform Sequential

![Shake Transform Sequential](/img/sequential_shaketransform.jpg)

This sequential shakes the transform with animation.


!!! note "Base Properties"
    To learn about the common Base Properties, please see [Base Sequential](../sequential_base.md)

!!! note "Target Object Options"
    This sequential derives from __Object Returner Sequential__ and gets all its properties from that sequential. So, to learn about the __Target Object Options__ please see [Object Returner Sequential](../sequentialobjectreturner/index.md)

!!! note "Animation Options"
    This sequential derives from __Animation Sequential__ and gets all of its properties. So, to learn about the __Animation Options please see [Animation Base](index.md)
    

## Shake Type

Each shake type has its own parameters.

### Simple

This has basic parameters but it's useful for most of shake scenarios.

#### Shake Position

If enabled, it will shake by modifying the position of the transform.

#### Position Shake Strength

This is the strength of position shake. You can think of this as the maximum offset of position when shaking can be this value.


It's applied when the Shake Position is enabled.

!!! tip
    For shaking UI elements, set it much higher to see the effect.

#### Shake Rotation

If enabled, it will shake by modifying the rotation of the transform.

#### Angular Shake Strength


This will be the maximum quaternion that transform can rotate while shaking. 

e.g. 1 means the transform quaternion will increase/decrease by 1 at max. 

!!! tip
    For shaking UI elements, set it much higher (about 1) to see the effect.

### Advanced

This type of shake has more control over the shake animation so you can get better results with fine tuning comparing to the Simple type.

#### Shake Position
If enabled, it will shake by modifying the position of the transform.

#### Shake Rotation
If enabled, it will shake by modifying the rotation of the transform.

#### Frequency

How many times to shake per second.

#### Max. Position Shake 

This will be the maximum units that transform can move while shaking. 

e.g. 1 means the transform position will move 1 unit at max. 

!!! tip
    For shaking UI elements, set it much higher to see the effect.

#### Max. Angular Shake

This will be the maximum angles (degrees) that transform can rotate while shaking. 

e.g. 30 means the transform position will rotate 30 degrees at max.

#### Shake Strength Exponent

Defines the falloff value.

It calculates the next value of shake by power of this value.



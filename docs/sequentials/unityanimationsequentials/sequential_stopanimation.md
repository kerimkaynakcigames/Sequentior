# Stop Unity Animator Animation Sequential

![Stop Animation](../../img/sequential_stopanimation.jpg)

This sequentials stops a playing Unity Animator animation.

!!! note "Base Properties"
    To learn about the common Base Properties, please see [Base Sequential](../sequential_base.md)

!!! note "Target Object Options"
    This sequential derives from __Object Returner Sequential__ and gets all its properties from that sequential. So, to learn about the __Target Object Options__ please see [Object Returner Sequential](../sequentialobjectreturner/index.md)


!!! warning "Target Object"
 
    Target Object (or Target Objects if Multiple Objects are returned) needs to be Animator type. So please make sure that the game object assigned in this field has an Animator component attached. Otherwise you'll see a runtime error log when this sequential plays.


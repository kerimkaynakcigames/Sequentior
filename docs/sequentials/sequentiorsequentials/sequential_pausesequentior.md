# Pause Another Sequentior

![Pause Another Sequentior Sequential](/img/sequential_pausesequentior.jpg)

This sequential pauses any playing sequentials of another Sequentior Manager.


!!! note "Base Properties"
    To learn about the common Base Properties, please see [Base Sequential](../sequential_base.md)

!!! note "Target Object Options"
    This sequential derives from __Object Returner Sequential__ and gets all its properties from that sequential. So, to learn about the __Target Object Options__ please see [Object Returner Sequential](../sequential_objectreturner.md)



!!! warning "Target Object"
 
    Target Object (or Target Objects if Multiple Objects are returned) needs to be type of __Sequentior Manager__. So please make sure that the game object assigned in this field has the Sequentior Manager component attached. Otherwise you'll see a runtime error log when this sequential plays. 
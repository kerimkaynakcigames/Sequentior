# Material Sequentials

![Material Sequential Base](/img/sequential_materialbase.jpg)

This is the base sequential for animating material properties. All the derived sequentials has the options mentioned below.

!!! note "Base Properties"
    To learn about the common Base Properties, please see [Base Sequential](../sequential_base.md)

!!! note "Target Object Options"
    This sequential derives from __Object Returner Sequential__ and gets all its properties from that sequential. So, to learn about the __Target Object Options__ please see [Object Returner Sequential](../sequentialobjectreturner/index.md)

!!! note "Animation Options"
    This sequential derives from __Animation Sequential__ and gets all of its properties. So, to learn about the __Animation Options please see [Animation Base](../animationsequentials/index.md)

!!! warning "Target Object"
 
    Target Object (or Target Objects if Multiple Objects are returned) needs to be Renderer type. So please make sure that the game object assigned in this field has a Renderer component (e.g. Mesh Renderer or Sprite Renderer) attached. Otherwise you'll see a runtime error log when this sequential plays. 

## Apply For All Materials

If checked, the sequential actions will be performed for all the assigned materials of the target renderer component.

If unchecked, you can specify the indexes of the materials.

## Material Indexes

If __Apply For All Materials__ is not checked, you can specify the indexes of the materials by adding indexes in the Material slot of the Renderer component to the list.

## Shader Property Name

For some Material Sequentials, you need to specify the related property name defined in the shader of the material. 

If no name is defined, the sequential tries to perform the action with a default property name. 

e.g. for changing color it tries to change the __color__ property but if you need to change a color with another property name defined in the shader, you need to enter it here.



# Getting Multiple Target Objects

In this section, you'll find information about getting multiple game objects to be used as the Target Objects in most of the sequentials.

### Get Target Object By

This option lets you choose how to find the target objects. There are a few options to choose from and each of them has its own properties.

### Delay Between Multiple Targets

By default, a sequential starts performing its actions on every target game object in the same frame by looping. But if you want to wait for a time before performing the sequential action for the next target object in Target Objects list, set a value (in seconds) for this option.

!!! info
    You can enter different type of values here by clicking the down arrow ![Down Arrow](/img/valuearrow.jpg) and choosing another option.
    To see how this works, see the [Value Assign](../../valueassign.md) section

### Direct Assignment

![Target Objects](/img/sequential_objectreturner_multiple_direct.jpg)

This lets you select multiple game objects as the target objects from the scene.

#### Target Objects

This list is used to assign multiple target objects directly from a scene.




### By Name

![Target Object Name](/img/sequential_objectreturner_multiple_name.jpg)

This lets you find multiple target game objects that matches the name.

#### Target Objects Name

This is the name of the game objects to find from the scene. It returns all the game objects that has the same name with this property.

#### Find Only In Children

If this is enabled, it tries to find the target objects from child game objects of the game object that this sequential is attached to.

#### Find In Children Of This

This is only available when Find Only In Children is enabled.

If nothing is assigned to this field, it tries to find in children of the game object this sequential is attached to.

If you assign another game object here, it will try to find in children of that assigned game object.

### By Tag

![Target Object Tag](/img/sequential_objectreturner_multiple_tag.jpg)

This lets you find multiple target game objects that has this tag.

#### Target Objects Tag

This is the tag of the game objects to find from the scene. 

### By Type
![Target Object Tag](/img/sequential_objectreturner_multiple_type.jpg)

This lets you find  target game objects by their class type.

#### Target Objects Type
This is the class name with full namespace of a component that is attached to the target object.

So, for example, to find game objects with SpriteRenderer component attached, you need to type _UnityEngine.SpriteRenderer, UnityEngine_.

!!! note "What's full type?"
    * For custom types, you can use the full class name with namespace. e.g. com.kerimkaynakcigames.MyGame.GameManager
    * For built-in types, write the class name and then put a comma (,) and then assembly name. e.g. UnityEngine.SpriteRenderer, UnityEngine

#### Find Only In Children
See [Find Only In Children](#find-only-in-children)

#### Find In Children Of This
See [Find In Children Of This](#find-in-children-of-this)

#### Find Inactive Objects Too
By default, only the active objects are returned as the target objects. But to search in inactive objects too, enable this option.

### By Object Group

![Target Object Group](/img/sequential_objectreturner_multiple_objectgroup.jpg)

This lets you find game objects which have __Sequentior Object Group__ component and have the same Group Name.

This is similar to finding by Tag but has more options and because Tags are used for other purposes in game development, you may not want to add and assign tags just for getting target objects in Sequentior. So this is an alternative way for grouping objects to find them in sequentials.

#### Target Objects Group Name

For example, to perform actions on all (or some of) the Buttons in your scene, you can add __Sequentior Object Group__ component to these buttons and give them a Group Name (say "Buttons"). Then in sequentials, you can get all of those buttons by entering the same group name to the __Target Objects Group Name__ field.

#### Sequentior Object Group Component

![Sequentior Object Group Component](/img/objectgroup.jpg)

##### Group
This is the name of the group this game object belongs to.

To find this object in sequentials, Target Objects Group Name should match this value.

##### Order

When multiple game objects are found in the same group, the sequential performs its related actions for each of those game objects one by one. But the order of the found objects are not deterministic, so you can't be sure about that sequential will perform the action on which game object first. To define a specific order, you can enter values to this field for each game objects that belongs the same group.

The game object that has the minimum Order value will be the first game object in the list.


### By Sequential
![Target Object Sequential](/img/sequential_objectreturner_multiple_sequential.jpg)

This lets you get the target objects from another sequential's returned game objects.

Some sequentials return game objects and expose these returned game objects to their Sequential output pin. e.g. Instantiate Sequential or Find Object Sequential.

So, to get these returned game objects as the target of another sequential, choose this option and connect the __Sequential output pin__ of other sequential to the __Target Obj input pin__ of this sequential. 

#### Target Objects Sequential
This is the sequential that will return the game object as the target object.
!!! warning
    Do not assign this field manually. This is automatically assigned when you connect another sequential's Sequential output pin to this sequential's Target Obj input pin.

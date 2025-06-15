# Find Multiple Objects Sequential

![Find multiple objects](/img/sequential_findmultipleobj.jpg)

This sequential lets you find multiple game objects and exposes it to its __Sequential output port__ as GameObject[].

## Find By Options

### By Name

#### Objects Name

![Target Object Tag](/img/sequential_findmultipleobj_byname.jpg)

This is the name of the game objects to find from the scene. 

#### Find Only In Children

If this is enabled, it tries to find the objects from child game objects of the game object that this sequential is attached to.

#### Find In Children Of This

This is only available when Find Only In Children is enabled.

If nothing is assigned to this field, it tries to find in children of the game object this sequential is attached to.

If you assign another game object here, it will try to find in children of that assigned game object.


### By Tag

![Target Object Tag](/img/sequential_findmultipleobj_bytag.jpg)

This lets you find multiple game objects by their tag.

#### Obj Tag

This is the tag of the game object to find from the scene. The first game object with this tag will be returned.


### By Type
![Target Object Tag](/img/sequential_findmultipleobj_bytype.jpg)

This lets you find multiple game objects by their class type.

#### Objects Type
This is the class name with full namespace of a component that is attached to the objects to find.

So, for example, to find a game object with SpriteRenderer component attached, you need to type _UnityEngine.SpriteRenderer, UnityEngine_.

!!! note "What's full type?"
    * For custom types, you can use the full class name with namespace. e.g. com.kerimkaynakcigames.MyGame.GameManager
    * For built-in types, write the class name and then put a comma (,) and then assembly name. e.g. UnityEngine.SpriteRenderer, UnityEngine

#### Find Only In Children
See [Find Only In Children](#find-only-in-children)

#### Find In Children Of This
See [Find In Children Of This](#find-in-children-of-this)

#### Find Inactive Objects Too
By default, only the first active object is returned as the target object. But to search in inactive objects too, enable this option.



### By Object Group

![Target Object Group](/img/sequential_findmultipleobj_byobjectgroup.jpg)

This lets you find game objects which have __Sequentior Object Group__ component and have the same Group Name.

This is similar to finding by Tag but has more options and because Tags are used for other purposes in game development, you may not want to add and assign tags just for getting objects in Sequentior. So this is an alternative way for grouping objects to find them in sequentials.

#### Objects Group

For example, to perform actions on all (or some of) the Buttons in your scene, you can add __Sequentior Object Group__ component to these buttons and give them a Group Name (say "Buttons"). Then in sequentials, you can get all of those buttons by entering the same group name to the __Objects Group__ field.

#### Sequentior Object Group Component

![Sequentior Object Group Component](/img/objectgroup.jpg)

##### Group
This is the name of the group this game object belongs to.

To find this object in sequentials, Objects Group should match this value.

##### Order

When multiple game objects are found in the same group, the sequential performs its related actions for each of those game objects one by one. But the order of the found objects are not deterministic, so you can't be sure about that sequential will perform the action on which game object first. To define a specific order, you can enter values to this field for each game objects that belongs the same group.

The game object that has the minimum Order value will be the first game object in the list.


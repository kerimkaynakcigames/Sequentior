# Find a Single Object Sequential

![Find a single object](/img/sequential_findsingleobj.jpg)

This sequential lets you find a game object and exposes it to its __Sequential output port__.

## Find By Options

### By Name

#### Obj Name

![Target Object Tag](/img/sequential_findsingleobj_byname.jpg)

This is the name of the game object to find from the scene. The first game object with this name will be returned.

#### Find Only In Children

If this is enabled, it tries to find the object from child game objects of the game object that this sequential is attached to.

#### Find In Children Of This

This is only available when Find Only In Children is enabled.

If nothing is assigned to this field, it tries to find in children of the game object this sequential is attached to.

If you assign another game object here, it will try to find in children of that assigned game object.


### By Tag

![Target Object Tag](/img/sequential_findsingleobj_bytag.jpg)

This lets you find a single  game object by its tag.

#### Obj Tag

This is the tag of the game object to find from the scene. The first game object with this tag will be returned.


### By Type
![Target Object Tag](/img/sequential_findsingleobj_bytype.jpg)

This lets you find a single game object by its class type.

#### Obj Type
This is the class name with full namespace of a component that is attached to the object to find.

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

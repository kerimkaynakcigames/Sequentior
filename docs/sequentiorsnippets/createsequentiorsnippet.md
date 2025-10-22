# Creating Custom Sequentior Snippets

Creating a sequentior snippet is just adding a Sequentior Manager component to a gameobject and then creating your flow with adding sequentials to this sequentior manager and then making this gameobject a prefab.

That's it!

But for making snippets more flexible and dynamic, you need to set the important properties by variables instead of setting them directly. e.g. if you created an animation inside this sequentior snippet, this animation needs a duration because all Animation Sequentials plays for a duration. So instead of setting a constant duration to the sequentials inside this snippet, define a variable to the sequentior manager and then get the duration property from this variable. 

!!! tip
    To make the variable of a sequentior snippet modifiable from another sequentior, set its Expose property to true. See [Variables](../variables/index.md) for more information.
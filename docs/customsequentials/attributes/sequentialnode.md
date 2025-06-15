# SequentialNode Attribute

This attribute is used to decorate Sequential classes and it basically defines how to display the node of a sequential in the [Sequentior Graph Editor](../../sequentiormanager/sequentiorgrapheditor.md).

``` csharp title="Sample SequentialNode Attribute"
 [SequentialNode(Group = "Animations",
                    Title = "Change Color",
                    USSClassName = "animationnode",
                    InputNodeCount = 1,
                    DisplayOrder = 111)]
public class Sequential_ColorChangeFast : Sequential_Animation
{
}
```

Here are the parameteres that can be used for this attribute:

## Title

Title will be displayed in both [Sequential List Window](../../sequentiormanager/sequentiorgrapheditor.md#add-new-sequential-node) and also on the Sequential Node itself.

![Sequential List Window](/img/sequentialnodeattr_title.jpg)
![Animation Sequential](/img/sequential_changecolor.jpg)

## Group

When creating sequentials in [Sequentior Graph Editor](../../sequentiormanager/sequentiorgrapheditor.md), a list of sequentials will be displayed as grouped and __Group__ parameter defines which group this sequential belongs to. You can use a built-in group name or can define your own custom group name.

![Sequential List Window](/img/sequentiorgrapheditor_createnodewindow.jpg)

## DisplayOrder

This defines the displaying order of the sequential in the list explained above.

!!! warning
    Please do use a DisplayOrder greater than __9999__. Because the numbers smaller than 9999 might be used for built-in sequentials.

## USSClassName

When creating sequential nodes in [Sequentior Graph Editor](../../sequentiormanager/sequentiorgrapheditor.md) style classes in a style sheet is used to define the look of a node. 

So in this parameter, you can enter the style class name that's defined in the __SequentiorEditorStyle.uss__ file located in _EditorWindows_ folder in Sequentior package.

## DontDisplayInList

This is used for obsolute or abstract sequential types that hides the sequential from Sequential List Window in the Sequentior Graph Editor.

## Description

This is the description that will be displayed when the _Question Mark_ button clicked on the sequential node.

## MinWidth

Minimum width of the sequential node.

!!! tip
    Some properties of sequential might be wide than usual (for example when the property title is too long) and this prevents the user from seeing some parts of the properties. If that's the case for your custom sequential node, you can set a large value to this parameter and the sequential node will be wider.

## MaxWidth

Maximum width of the sequential node.

## MinHeight

Minimum height of the sequential node.

## Resizable

If true, you can resize the sequential node on the Sequentior Graph Editor.

## InputPortCount


Input ports are the ports that let the sequential accept other sequential's output values.

All the sequentials have the __IN__ input port because __NEXT__ output port of another sequential connects to the IN input port to create a flow. Because this is the default input port, this does not count to InputPortCount parameter.

All the other input ports are extra input ports and should be added to the InputPortCount parameter.

![Input Ports](/img/inputports.jpg)

For example, Move Sequential has 4 input ports including the IN. We don't count IN as extra, so InputPortCount parameter should be 3.


## DontDrawProperties

If true, only the input and output ports will be displayed. Properties won't be displayed.

[Start Sequential](../../sequentials/sequential_start.md) uses this property to hide properties derived from Sequential Base class.

## DontDrawInputPort

If true, input ports won't be displayed.

## DontDrawOutputPort

If true, output ports won't be displayed.



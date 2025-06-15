# Basics

!!! danger "Important"
    Every sequential should derive from __Sequential__ class or one of its descendant classes.

__SequentiorManager__ class is the main manager that manages the flow of sequentials and is responsible for playing its sequentials. 

``` csharp title="Start Sequentials"
    sequentialManager.StartAllSequentials();
```

Typically, it loops over all the sequentials and calls the sequentials' __DoSequentialAction()__ method which is a virtual method. So, you need to override this method in your custom sequential class and write the code that performs its actions inside this method.

For example; a simple __Log sequential__ can be defined as below:

``` csharp title="Log Sequential (partial)"
    
    /* The first imporant thing is to derive your sequential from Sequential class (or one of its derived classes)
    */
    public class Sequential_Log : Sequential
    {
        // this is a property of the sequential item
        public string Log;

        /* we need to override the DoSequentialAction method because
           this is where all the logic of the sequential is defined.
           SequentialManager will call this method for every sequential. 
        */
        public override void DoSequentialAction()
        {
            // This is the actual action this sequential performs (logging):
            Debug.Log(Log);

            /* Calling the base class's DoSequentialAction is important
               because it raises the complete event of the sequential.
               Otherwise SequentiorManager can't know if the sequential completed its action or not and this might cause problems.
            */
            base.DoSequentialAction();
        }

    }
```

Now, we've defined the custom sequential class. But to make this sequential usable in Sequentior Graph Editor, we need to add the [SequentialNode Attribute](attributes/sequentialnode.md) to this custom class.

``` csharp title="SequentialNode Attribute"
 [SequentialNode(Group = "My Sequentials",
                    Title = "My Log",
                    InputPortCount = 1,
                    DisplayOrder = 10001,
                    MinWidth = 300)]
public class Sequential_Log : Sequential
{
    //...
}
```

Now, you can see this sequential in the [Sequentior Graph Editor](../sequentiormanager/sequentiorgrapheditor.md#add-new-sequential-node).

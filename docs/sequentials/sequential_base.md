# Sequential Base Properties

![Sequential Base Properties](/img/sequential_base.jpg)

Because every sequential derives from the base Sequential class, every sequential has those properties.

## Seq Id
This is the auto generated Id of this sequential. This is useful for getting a sequential from script.

## Muted

This is mostly used to temporarily disable the sequential. When enabled, this sequential is ignored and not played.

## Comment

This is used for taking personal notes about this specific sequential.

## Delay

To delay the playing of the sequential, set a value in this field.

This does not delay the next sequentials, delays only this sequential.

For example, if you specify 1 for this sequential, this will wait 1 seconds to play but the next sequential will play without any wait (unless it has delay or it's a __Wait__ sequential)

## Chance

By default every sequential in the flow will play. But for creating some randomness, you can speecify a Chance value that determines if it will play this sequential or ignore it.

For example, if you specify 0.3 for this value, that means the chance of playing this sequential is 30%.

## Events

This section lets you call scripts when an event occurs.

### Action Completed

The methods you've added to this list will be called when this sequential completes its actions.

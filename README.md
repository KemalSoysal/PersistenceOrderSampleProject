#PersistenceOrderSampleProject

In MPS there are multiple persistence options for models.

There is a difference in the order of the nodes in the models.
This sample project is demonstrating the difference with `MPS 2021.1.3`.

## PersistenceOrderSample-Solution
is Solution Kind `Other`, so it is able to host a plugin model

### plugin-Model
contains an action to list the model roots in the order delivered by the iterator.
LogRootsInOrderOfIterator puts messages in the messages tool window 
with the model name and node presentation in order of their appearance 
from the model roots iterator.

## SampleSolution
### xmlbased_model
Classes A,B,C have been created in sequence.

### xmlbased_model_clone
xmlbased_model have been cloned to this model.

### xmlbased_per_root_model
Classes A,B,C have been copied to this model.

## Testing
Log model roots with the action on the model context menu.
Cut out node A from the top and add it again by pasting it.
Log model roots with the action on the model context menu again.

The log result will be different for the xml based models.

For the per root file models the file system will deliver the same order here.

Add a new Class b to the per root model. It will be listed underneath B.
The log shows it to you at the last position under C.

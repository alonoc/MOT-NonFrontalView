# Training and Test set

A correct selection of a training set and a test set for our upcomming evaluation 
of MOT approaches from a cenital view avoids situations of overfitting and underfitting, 
two common phenomena while dealing with artificial intelligence (AI).

To accomplish that is necessary to follow a serie of criterias in the test set:

* It should be large enough.
* It should be a representative part of the whole dataset. (With similar characteristics to the training set)

## K-Fold cross validation

K-fold cross validation was selected as the form to divide the training and test set.
Under this approach the dataset is divided under k subsets. Each time one of the k subsets is 
used as the test set and the remaining k-1 subsets as the test set. 
Then the error estimation is avegaged over all k trials to get the total effectiveness of the model. 
In this way the bias is reduced because most of the data is also being used in the test set.

This approach has the advantage that is easy to implement with the MatchNMingle dataset due to 
it is already divided in days that can be seen as subsets of the dataset, so no complex setup is required.

The mingle dataset contains data for three days of dates with data annotated for 3 different cameras,
each day of event were attended by different persons. So for our case k=3, and each subset contains the
data for the given data for the three different cameras. The video duration for each camera per day is 
approx 30min.










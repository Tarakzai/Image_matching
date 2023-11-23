# Image_matching

## Description
Root image matching using opencv

## Ransac

```diff
+ Green
- Red
! Orange
@@ Pink @@
# Gray


- RANSAC (Random Sample Consensus) is an iterative algorithm used for model fitting in the presence of outliers.

- Objective: RANSAC is designed to robustly estimate parameters of a mathematical model from a set of observed data points, even when a significant portion of the data is contaminated by outliers.

- Iterations: The algorithm operates through a series of iterations. In each iteration:

- A random subset of data points (minimum required for model fitting) is sampled.

- A model is fitted to this subset.

- All other data points are then tested against this model, and those that are consistent with the model (inliers) are identified.

- Model Evaluation: The quality of the model is evaluated based on the number of inliers it has. This is typically measured by a predefined threshold that determines whether a data point is considered an inlier.

- Consensus Set: The set of inliers for a particular model is called the consensus set.

- Termination Condition: The algorithm terminates when a sufficiently good model is found, or after a predetermined number of iterations.

- Trade-off: RANSAC trades computational cost for accuracy. By working with a subset of data points, it is less sensitive to outliers compared to methods that consider the entire dataset.
...

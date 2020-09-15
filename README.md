# Intersection-Over-Union---Object-Detection

Intersection over Union is an evaluation metric used to measure the accuracy of an object detector on a particular dataset. 
Intersection over Union is simply an evaluation metric. Any algorithm that provides predicted bounding boxes as output can be evaluated using IoU.Mean Intersection-Over-Union is a common evaluation metric for semantic image segmentation, which first computes the IOU for each semantic class and then computes the average over classes. IOU is defined as follows: IOU = true_positive / (true_positive + false_positive + false_negative). The predictions are accumulated in a confusion matrix, weighted by sample_weight and the metric is then calculated from it.

The predicted bounding box is drawn in red while the ground-truth (i.e., hand labeled) bounding box is drawn in green. The denominator is the area of union, or more simply, the area encompassed by both the predicted bounding box and the ground-truth bounding box.

Dividing the area of overlap by the area of union yields our final score — the Intersection over Union.
If sample_weight is None, weights default to 1. Use sample_weight of 0 to mask values.

Arguments

num_classes: The possible number of labels the prediction task can have. This value must be provided, since a confusion matrix of dimension = [num_classes, num_classes] will be allocated.
name: (Optional) string name of the metric instance.
dtype: (Optional) data type of the metric result.

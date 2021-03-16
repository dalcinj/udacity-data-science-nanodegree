Advantages of Using Pipeline Part 1:
1. Simplicity and Convencience
Automates repetitive steps - Chaining all of your steps into one estimator allows you to fit and predict on all steps of your sequence automatically with one call. It handles smaller steps for you, so you can focus on implementing higher level changes swiftly and efficiently.
Easily understandable workflow - Not only does this make your code more concise, it also makes your workflow much easier to understand and modify. Without Pipeline, your model can easily turn into messy spaghetti code from all the adjustments and experimentation required to improve your model.
Reduces mental workload - Because Pipeline automates the intermediate actions required to execute each step, it reduces the mental burden of having to keep track of all your data transformations. Using Pipeline may require some extra work at the beginning of your modeling process, but it prevents a lot of headaches later on.

Advantages of Using Pipeline Part 2:
2. Optimizing Entire Workflow
GRID SEARCH: Method that automates the process of testing different hyper parameters to optimize a model.
By running grid search on your pipeline, you're able to optimize your entire workflow, including data transformation and modeling steps. This accounts for any interactions among the steps that may affect the final metrics.
Without grid search, tuning these parameters can be painfully slow, incomplete, and messy.
3. Preventing Data leakage
Using Pipeline, all transformations for data preparation and feature extractions occur within each fold of the cross validation process.
This prevents common mistakes where you’d allow your training process to be influenced by your test data - for example, if you used the entire training dataset to normalize or extract features from your data.
You'll see what we mean by this in a video later in this lesson about using Pipeline with GridSearchCV.
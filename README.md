# CMI-Problematic-Internet-Use

This is the copied and modified notebook from the public one of author <a href="https://github.com/yunsuxiaozi/">yunsuxiaozi</a> in the <a href="https://www.kaggle.com/competitions/child-mind-institute-problematic-internet-use">CMI - problematic internet use</a> competition *(The post for that notebook has now been deleted by the author)*.

**Main changes made to this notebook:**
- Use actigraphy data, which was unused in the original.
- Use imputation for missing values.
- Add an objective function for retuning the hyperparameters of the model using Optuna, change binary classifier to multiclass.

**Procedure:**
1. Read HBN instruments and Actigraphy data, merge them to a single data set based on id, remove all records that don't have target sii value.
2. Perform imputation for missing values.
3. Perform feature engineer.
4. Run hyperparameters optimization (only need to run once).
5. Train the model.
6. Create submission file.

This notebook get 0.450 for public score and 0.451 for private score.

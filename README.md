The need for predictive maintenance system for wall surface buildings has emerged and several works have been done around developing and improving maintenance for buildings through the use of Artificial Intelligence, preferably Machine and deep learning algorithms. To able to build a maintenance system, deflection and Cracks were the yardstick for evaluating the structural health of a building. Image classification was done on the cracks dataset and prediction of deflection was achieved using the numerical dataset and set at a threshold based on the maximum permissible deflection for a wall surface building. 


Three models, VGG16, VGG19, and ResNet50 were trained, fitted, and implemented with same epochs of 15 taking accuracy and loss as metrics. I observed that training the data by increasing the epochs number enhanced the model’s accuracy and reduced the loss. The maximum accuracy of VGG16 was 99.7%, 99.6% for VGG19 and 94.1% for ResNet50 were all trained with 15 epochs. The VGG16 model slightly outperforms the other models in terms of accuracy, with the maximum accuracy of 99.7% on the validation data. The loss history plot for models indicates that as the epochs increased in number, the loss value had a decrease on the train and validation.

While for the accuracy graph, as epoch value increased, the accuracy improved for training, and showed a sinusoidal shape for the validation. For predicting deflection, Random Forest Regressor had the best performance based on evaluation of metrics of RMSE, MAE and R2-score making it a good fit after hyperparameter tuning through a 5-fold cross validation. The initial R2-score values from deflection prediction on train data for the model had a high value of 0.91 and 0.52 for test data which indicates an overfit model because the R2 score is high on train and very low for test data. Performing hyperparameter tuning through cross validation and grid search technique aided in fine tuning the model by optimizing the R2-scores on the train and test data to be 0.80 and 0.85 respectively which represents a good fit model. The successful implementation of these models will help to monitor and manage the structural health data of a reinforced concrete building through predictive maintenance based on deflection and Cracks.  
After the two best models were chosen, a graphical user interface was created for user interaction front end

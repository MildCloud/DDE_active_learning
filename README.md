# DDE_active_learning
The repository consists text CNN model for website clarrification, using short texts and long texts. The construction and training of model are mainly the work from Jiarong Shi(2675861415@qq.com). Based on his work, uncertainty methods are used to select the most efficient data for training.
## Long Texts
- The strategy is using the newly selected data and combining it with the original data to retrain the model. 
- The result shows that selecting the most certain datas has better efficiency, which controdicts to the uncertainty theory. 
- One possible reason is that the original model doesn't converge.
- Another possible reason is that the newly selected datas should be used to fine tune the model rather than retrain the model.
## Short Texts
- The strategy is using the newly selected data to fine tune the original model.
- The parameters in convolution layers and pooling layers are unchanged and the parameters in the linear layer are changed
- The model after fine tune yeilds a better result than the original model and even the model trained using more larger data.

# DeepLearningCancerDetection

The goal of this project was to train a deep neural network in Tensorflow to identify cancerous region in pathology images. The project was aimed at recreating the results of this paper using novel code and methods: https://arxiv.org/pdf/1703.02442.pdf.

The training dataset consisted of 10 gigapixel pathology images, each with two different magnification levels. The cancerous regions of each slide were labeled by a team of trained pathologists.

A multi-input convolutional neural network based on two InceptionV3 stacks was trained with transfer-learning on ImageNet and fine-tuning on the training dataset to classify each 299x299 pixel patch on the slides as either cancerous or benign, using the expert annotations as ground truth.

The model was tested on 3 additional pathology images, and achieved an overall accuracy of between 86%-99% in correctly annotating tumor regions as cancer or benign.

For a more in-depth overview of the methods, see the project_overview slides. For a peek into the code, take a look at the deep_learning_cancer_detection notebook.

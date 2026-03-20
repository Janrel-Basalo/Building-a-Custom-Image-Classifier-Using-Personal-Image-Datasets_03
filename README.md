# Building-a-Custom-Image-Classifier-Using-Personal-Image-Datasets_03

## Google Colab link : https://colab.research.google.com/drive/1LtY7AwrgScu7G7wK9SFemqhD6ssD7Wv5?usp=sharing

## Visualization & Overfitting

## 1. What signs indicated overfitting in your first model?
### Ans.  During the traing process, the models accuracy continued to rise, reaching up to 99% , while the accuracy on the validation remained at 93%. The validation loss continued to increase after the second epoch, indicating that the model was retaining information from the traing data rather than understanding broader patterns

## 2. How did data augmentation affect validation accuracy?
### Ans. It improved the model's ability to generalize. The system was trained to recognize plants in several orientations by randomly flipping, rotating, and zooming the image. This reduced overfitting and maintained more constant validation accuracy.

## Model Improvement

## 3. What is the purpose of dropout layers?
### Ans. T  o prevent the model from becoming overly dependent on any one neuron, dropout randomly shuts off certain neurons during training. This lessens overfitting by making it learn more broad traits.

## 4. Why does data augmentation improve generalization?
### Ans. By purposefully increasing the variety of training pictures, it enables the model to come across several iterations of the same image throughout each training cycle. As a result, it can process fresh pictures that it has never seen before more efficiently.

## Performance Comparison

## 5. Compare accuracy before and after improvements.
### Ans. The baseline model was overfitting, its validation accuracy was 92.96%. With a better trend, the enhanced model achieved 88.50% validation accuracy; the validation loss was still declining, indicating that it had not yet peaked.

## 6. Which technique contributed most to improvement?
### Ans. Data augmentation was the most effective approach because it directly addressed the underlying issue of overfitting by increasing the diversity of images. Dropout was helpful as well, but data augmentation had a more significant effect.

## Deployment & Application

## 7. Why is saving the model important? 
### Ans. Training took a long time. Saving it means we don't have to retrain every time we can just load it and use it immediately for predictions but sometimes it needs to retrain like what i experience.

## 8. How can this model be deployed in a real-world system?
### Ans. It may be implemented as a web application that allows users to upload a picture and receive a forecast. Additionally, it might be transformed into TensorFlow Lite for a mobile application that would enable users to recognize aquatic vegetation or any other plant that you want to train right from their phone.






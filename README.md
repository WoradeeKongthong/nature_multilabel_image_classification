# Nature Multi-label Image Classification 

## Objective 
To learn tags/labels given to each landscape image.  
There are 5 tags;  
- desert  
- mountains  
- sea  
- sunset  
- trees  

## Dataset
source : https://www.dropbox.com/s/0htmeoie69q650p/miml_dataset.zip?dl=0  
(You can follow the tutorial of multi-label image classification in this blog https://vijayabhaskar96.medium.com/multi-label-image-classification-tutorial-with-keras-imagedatagenerator-cd541f8eaf24, I only use his dataset.)  
Originally, images are in 'images' folder. Their tags are stored in miml_labels_2.csv.  
In this project, I preprocess the dataset and save it in .npz format. Then I use in-memory approach to ingest dataset into the notebooks.  

## Model Development (are performed on Google COLAB)
The models used in this multi-label image classification problem are
- NN with VGG blocks  
- NN with Keras pre-trained VGG16 as a feature extractor  

Both preprecessing and model development are in the same notebook.

## Prediction
The best model from above are selected and make a prediction.
There are both prediction of one image and several images (batch) at a time.

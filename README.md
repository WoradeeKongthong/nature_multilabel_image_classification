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
All preprecessing of the dataset is in 01_data_preparation.ipynb.

## Model Development (are performed on Google COLAB)
The models used in this multi-label image classification problem are
- NN with VGG blocks (developed in  )
- NN with Keras pre-trained VGG16 as a feature extractor (developed in  )
- NN with Keras pre-trained ResNet50 as a fetaure extractor (developed in  )

## Prediction
The best model from above are selected and make a prediction.
(Note : Need to get model.h5 from the selected model ipython notebook by running it first)
The prediction process is presented in 05_make_prediction.ipynb.  
There are both prediction of one image and several images (batch) at a time.

## My best trained models
- model with pretrained ResNet50 : https://drive.google.com/file/d/1DIHfvpTi3PH7XWdnBWO6Bp3wMDaLSo3Q/view?usp=sharing
## other trained models
- VGG blocks model : https://drive.google.com/file/d/1tV6ziKo9LOBLkbTJQBAyiDScvpshFWe9/view?usp=sharing
- model with pretrained VGG16 : https://drive.google.com/file/d/181hvkzL1zd9gmPYsMapf3tPetK7iqZ26/view?usp=sharing

# Indoor/Outdoor/Map classifier


## Description 
Images Clasification
The goal of your project is to create a robust classifier, to collect data and prepare custom dataset.
You will build a model that will recognize

Properties

Indoor

    Kitchen 
    Living room
    Bathroom
    Bedroom 

Outdoor

Garbage

Map 
    Other things, Garbage (Logo, tables, signatures ...)

This project consists of the following activities :

    Dataset info
    https://drive.google.com/drive/folders/1HOn2LPxoKKTG3whaxkTQrEyltw6uz82n?usp=sharing

    Raw Data : Useful for garbage and maybe outdoor images
    Room data : Useful for Indoor images

Plan

Phase 1 :

Dataset and team planning

Team Planning

Full git project Integration

General Project Research

Dataset Collection

Dataset Preparation

Phase 2 :

Training
        
Research about neural networks

Compose and train neural network architectures

Ping Pong phase with Dataset labelers

Generate syntethic data if needed

Fine tunning of your model
    
Phase 3 :

Deployment

Analysis and benchmark Precision/Recall + Confusion Matrix

Model Deploy (Git)

Write git Readme.md file

Receive Feedback from PM

## Notebook
Notebook is given at this [link](https://colab.research.google.com/drive/17hodAaCM-5eQU-2tpnk6WdVvux6pimZF?usp=sharing)


## Predictions

| Bathroom | Bedroom | dining_room  | kitchen |maps | other | outdoor |
|:------: | :------: | :------: |:------: | :------: | :------: | :------: | 
|<img src="https://i2-prod.manchestereveningnews.co.uk/incoming/article18734591.ece/ALTERNATES/s1200c/1_254857696.jpg" width = 220px height = 120px > |<img src="https://media.istockphoto.com/photos/white-modern-bedroom-picture-id500120991" width = "220px" height = "120px" >| <img src="https://www.mydomaine.com/thmb/yDqpl0RLlsS-AslxDX9cav17RdA=/500x350/filters:no_upscale():max_bytes(150000):strip_icc()/cdn.cliqueinc.com__cache__posts__275260__modern-california-house-tour-275260-1545071142629-image.700x0c-0aaafe385afa49ebacc261ca3ed9c4f6.jpg" width = "220px" height = "120px" >| <img src="https://www.mydomaine.com/thmb/BDTs_CfbqrpvpgQ-YxWtjMawmv8=/500x350/filters:no_upscale():max_bytes(150000):strip_icc()/AuslandInteriors-bb94e66cf78c449eb8316d30f5f6b19a.jpg" width = 220px height = 120px >|<img src="https://www.google.com/maps/d/thumbnail?mid=1OyNxaAJ66dh23Kh5fMDhY2Xs5L4&hl=iw" width = 220px height = 120px > |<img src="https://assets-global.website-files.com/580ea75512564ed05c3a8455/59f4ce1cdefbd9000100e63c_hellosign-blog-header%20copy%20139.jpg" width = 220px height = 120px >| <img src="https://media.istockphoto.com/photos/colonial-style-house-picture-id1284097677?b=1&k=20&m=1284097677&s=170667a&w=0&h=1A7BkHG5OU4WCN7m22OOhvVmU21q4UsYVJPrS1kgcKI=" width = 220px height = 120px > |
### Supported Classes :
* Bathroom
* Bedroom
* Dining room
* Kitchen
* Outdoor
* Other
* Map

# Dataset
Dataset is given at this [link](https://drive.google.com/file/d/1-_B2JbcUISxzmcW7nj46iASBFFb2kNPh/view?usp=sharing)

# Model 
The model is given at this [link](https://drive.google.com/file/d/1iBxOY9dx4aSJ_PF50te1VMoPim_1Xunk/view?usp=sharing)

# Visualizations

This model is created to differ indoor from outdoor images. It also regonizes maps from other images. The main purpose of this model is to be inplemented in a many applications for classifying the type of the images (for example Bathroom images).

# Installation

```
pip install -r requirements.txt
```

## File tree structure 

```
## File hierarchy
    

    |── Notebook.ipynb                              Train functions
    |── Requirements.txt                            Dependencies
    |── Prediction.ipynb                            Prediction Notebook

```



For the purposes of this project transfer learning was used with: 
- [x] Resnet 50 (Large)
- [] Mobilenet V3 )



# Evaluation results
Classification for indoor-outdoor images

```
precision    recall  f1-score   support

    bathroom       0.91      0.93      0.92      1000
     bedroom       0.95      0.91      0.93      1000
 dining_room       0.82      0.89      0.86      1000
     kitchen       0.87      0.84      0.86      1000
        maps       0.99      0.99      0.99       872
       other       0.99      0.98      0.99       998
     outdoor       1.00      0.99      0.99       962

    accuracy                           0.93      6832
   macro avg       0.93      0.93      0.93      6832
weighted avg       0.93      0.93      0.93      6832
```

## Future Work

Future work


# Indoor/Outdoor/Map classifier

## Predictions

| Bathroom | Bedroom | Map |
| :------: | :------: | :------: |
| <img src="https://i2-prod.manchestereveningnews.co.uk/incoming/article18734591.ece/ALTERNATES/s1200c/1_254857696.jpg" width = 300px height = 200px > | <img src="https://cdn2.furniture1.eu/v7/_v2_/494/494166.jpg?w=700&h=440&p=fw" width = "300px" height = "200px" > |<img src="https://media.wired.com/photos/59269cd37034dc5f91bec0f1/191:100/w_1280,c_limit/GoogleMapTA.jpg" width = "300px" height = "200px" > |

### Supported Classes :
* Bathroom
* Bedroom
* Kitchen
* LivingRoom
* Outdoor
* Other
* Map

# Dataset
Link...

# Model 
Link
# Visualizations

This model is created to differ indoor from outdoor images. It also regonizes maps from other images. The main purpose of this model is to be inplemented in a many applications for classifying the type of the images (for example Bathroom images).

## File tree structure 

```
## File hierarchy
    

    |── Notebook.ipynb                              Train functions
    |── requirements.txt                            Dependencies
    |── Prediction.ipynb                            Prediction Notebook

```



For the purposes of this project transfer learning was used with: 
- [x] Resnet 50 (Large)
- [] Mobilenet V3 )

## Future Work

Future work

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


# face-recognition
Implements Siamese Neural Network for One Shot Image Recognition

## Dependencies
1. Unzip the file at [this](https://drive.google.com/file/d/1Uiw4CZk1unSKW6GH2BFoGd9lRrKVaQT3/view?usp=sharing) location and add those files in **20180402-114759** folder (These are pre-trained weights)
2. Pre-trained models are alread present in **mtcnn** folder
3. Python modules required are
   - tensorflow==1.13.1
   - numpy==1.16.3
   - sklearn==0.20.0
   - cv2==3.4.3
   - flask==1.0.2
   - werkzeug==0.14.1
   - tqdm==4.28.1
   - matplotlib==2.2.4
   - pandas==0.23.4

## Handling data
Enter your images in the folder **data**
Make sure you enter images class-wise, i.e. if you have photos of 100 different people, make 100 folders inside **data** and keep at least 1 image inside each of it.

Note: Seems like there is some issue with using .png images. Try using .jpeg or .jpg 

## Running the model

Run the python files in the order
```
python create_face_embeddings
python align_dataset_mtcnn
python rest-server
```

The last commands launches a server at http://127.0.0.1:5000/ on which the FR system can be accessed

In case you want to train your own models, follow these 2 links:


* Facenet training: https://github.com/davidsandberg/facenet/wiki
* MTCNN training: https://github.com/wangbm/MTCNN-Tensorflow

Feel free to ping me in case anything is broken. Thanks for visiting. Cheers!

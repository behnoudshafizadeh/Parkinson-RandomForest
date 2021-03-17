# Parkinson-RandomForest
using RandomForest for detecting Parkinson Disease
## DISCRIPTION
> In this Project, I use OpenCV and machine learning to automatically detect Parkinson’s disease in hand-drawn images of spirals and waves.The researchers found that the drawing speed was slower and the pen pressure lower among Parkinson’s patients — this was especially pronounced for patients with a more acute/advanced forms of the disease.One of the symptoms of Parkinson’s is tremors and rigidity in the muscles, making it harder to draw smooth spirals and waves.After reviewing the dataset, I use the HOG image descriptor to quantify the input images and then how we can train a Random Forest classifier on top of the extracted features.
>
## DATASET
> We’ll then examine our dataset of drawings gathered from both patients with and without Parkinson’s.The dataset we’ll be using here today was curated by `Adriano de Oliveira Andrade and Joao Paulo Folado` from the [NIATS of Federal University of Uberlândia](http://www.niats.feelt.ufu.br/en/node/81),The dataset itself consists of 204 images and is pre-split into a training set and a testing set, consisting of:
> * Spiral: 102 images, 72 training, and 30 testing
> * Wave: 102 images, 72 training, and 30 testing
> you can see the sample of dataset as below :
>
![sampledataset](https://user-images.githubusercontent.com/53394692/111483162-cc9aee00-8749-11eb-8c84-2a73caf4af36.PNG)
>
## STRUCTURE of This Project
> Our `dataset` directory  is first broken down into `spiral` and `wave` . Each of those folders is further split into `testing` and `training` . Finally our images reside in `healthy` or `parkinson`  folders.
>
> for running algorithms,we use `detect_parkinsons.py` file,and run it by following command:
```
python detect_parkinsons.py --dataset dataset/spiral
or
python detect_parkinsons.py --dataset dataset/wave
```
> after training by `wave` immage dataset,you see result basis on `test` dataset as below:
> 
![result](https://user-images.githubusercontent.com/53394692/111487360-89db1500-874d-11eb-9c91-5c2a13972e29.PNG)
>
> furthermore,you see results of test dataset,basis on training on `Spiral` iamge dataset.

## License
> [Detecting Parkinson’s Disease with OpenCV, Computer Vision, and the Spiral/Wave Test](https://www.pyimagesearch.com/2019/04/29/detecting-parkinsons-disease-with-opencv-computer-vision-and-the-spiral-wave-test/) by Adrian Rosebrock

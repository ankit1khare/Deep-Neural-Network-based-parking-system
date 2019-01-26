# Deep-Neural-Network-based-parking-system

![](deep_park.gif)

Features:
- [Fastai library](https://github.com/fastai) (lesson 1) is utilized to train Resnet101 based deep neural network classifier which classifies empty space and car
- Laplacian opertor gives edges and their density is used to check the status of a parking spot and then whenever there's any change in the status of any parking spot, classifier is introduced at the spot to determine if its a car and change the color of the spot to indicate whether it is occupied or empty
- OpenCV is used and its inbuilt functions are played with, to observe their efficiency
- Minor computer vision techniques like background subtraction, kernel dilation and morphing were tried  
- Code is written using google colab for ease of use and to enable people not having a GPU to be able to keep up with deep learning using google's generous technologies
- The accuracy of classifier is 97% and it is trained using [standord's car dataset](https://ai.stanford.edu/~jkrause/cars/car_dataset.html)
- The performance achieved is not so good in terms of FPS. I'll write a separate post comparing various techniques like YOLO, MASKRCNN and simple Resnet based classifier used in the way shown in this repository
- Any suggestions and pull request aimed at making the system better are most welcomed



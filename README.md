# Deep-Neural-Network-based-parking-system

![](deep_park.gif)

# Features:
- [Fastai library](https://github.com/fastai) (lesson 1) is utilized to train Resnet101 based deep neural network classifier which classifies empty space and car
- Laplacian opertor gives edges and their density is used to check the status of a parking spot and then whenever there's any change in the status of any parking spot, classifier is introduced at the spot to determine if its a car and change the color of the spot to indicate whether it is occupied or empty
- OpenCV is used and its inbuilt functions are played with, to observe their efficiency
- Minor computer vision techniques like background subtraction, kernel dilation and morphing were tried  
- Code is written using google colab for ease of use and to enable people not having a GPU to be able to keep up with deep learning using google's generous technologies
- The accuracy of classifier is 97% and it is trained using [standord's car dataset](https://ai.stanford.edu/~jkrause/cars/car_dataset.html)
- For now I've added the parking spots using my utility program included in this repository which I call, "Real-time boxing". All the coordinates are recorded in a yaml file and used by the main program as parking spots to be observed at all periods of time. In my street parking project, I've automatically detected the spots. Also, it is faster due to use of MASK-RCNN. You can check that [here](https://github.com/ankit1khare/Easy_street_parking_with_MASK-RCNN) 
- The video taken is full of occlusions. There was a glass in the middle and people walking down the stairs had a shadow of them in the glass which reflects within parts of reording as well. Therefore, a lot of times, motion tracking detects continuous change in textures which is due to the aforementioned reasons and not due to actual vehicle movements. You can try using other videos recorded for a parking lot  
- The performance achieved is not so good in terms of FPS. I'll write a separate post comparing various techniques like YOLO, MASKRCNN and simple resnet based classifier used in the way shown in this repository
- Any suggestions and pull request aimed at making the system better are most welcomed



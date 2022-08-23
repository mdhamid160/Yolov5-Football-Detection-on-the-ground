# Yolov5-Football-Detection-in-live-match




![Football](https://github.com/mdhamid160/Yolov5-Football-Detection-on-the-ground/blob/main/football.mp4)




Such an amazing model thank you YOLOv5, it helps to better understand the object detection. 

I trained Yolo model on my custom data and can identify objects easily.
These are simple steps for taining and testing.

Step1. 

Prepare your dataset in following order in folders


                   [train]
         images->
                    [val]


Data->

                    [train]   
          labels->
                    [val]
                  
images folder will contain images for training and validation in the ratio of 7:3
Similarly the lables folder will contain  annotation txt file for images.

we can use https://www.makesense.ai for annotaion.

Step2.

In the yolov5-master we have .\data\coco128.yaml file.
Provide the path for your test data and train data and lables
Make changes in number of classes , i.e. nc=2 for two classes ['foot', 'person'].


Step3.

Trainig the model:
Run train.py file with modified number of parameter like batch size, number of epochs, learnning rate.


Step4.

Output:
The output after training the model will be availble in the new folder called test .\runs\train. New weights will be there in folder.


Step5.

Inferencing:
We can use new best weights to test our model on new unseen images or video.
Place your images or video in .\test folder 
Execute the detect.py 
The output will be availble at .\runs\detect\exp


Here you Go.





Before Training..........

![img1](https://user-images.githubusercontent.com/33762043/174591500-bd7cb07f-b569-4097-9887-ba64e0b2a0f4.jpg)



After Traing.............

![img1](https://user-images.githubusercontent.com/33762043/174591922-478673aa-8c69-45b1-8987-b816361081b3.jpg)








<----------------------------------------------------Enjoy Learning------------------------------------------------------------------->

# Drowsiness-Detection-in-Real-Time
Drowsiness detection is a safety technology that can prevent accidents that are caused by drivers who fell asleep while driving. The objective of this project is to build a drowsiness detection system that will detect drowsiness through the implementation of computer vision system that automatically detects drowsiness in real-time from a live video stream and then alert the user with an alarm notification.

# Motivation
According to the National Highway Traffic Safety Administration, every year about 100,000 police-reported crashes involve drowsy driving. These crashes result in more than 1,550 fatalities and 71,000 injuries. The real number may be much higher, however, as it is difficult to determine whether a driver was drowsy at the time of a crash. So, we tried to build a system, that detects whether a person is drowsy and alert him.

# Algorithms and Formulas
Using the Dlib library, the 6 coordinates on each eye and 20 coordinates on the mouth region were marked. Using those landmarks, Eye Aspect Ration (EAR) and Mouth Aspect Ratio (MAR) were calculated as shown in the formulas below:

<p align="center">
          <img src="https://user-images.githubusercontent.com/66065738/152203244-52d8c827-1fbf-4387-8237-c5d63779f741.png">
</p>

<p align="center">
          <img src="https://user-images.githubusercontent.com/66065738/152202994-75fdb868-61b7-4164-973e-1b62c1252800.png">      
</p>

<p align="center"> EAR=(||p2-p6|| + ||p3-p5||)/2x||p1-p4||)</p>


          
![image](https://user-images.githubusercontent.com/66065738/152202892-4a3a2c66-a9d1-4249-9651-7204d2fb84c7.png)

# MAR = (||p62-p68|| + ||p63-p67|| + ||p64-p66||)/(3x||p61-p65||) 

# Results

![1](https://user-images.githubusercontent.com/66065738/151976404-d03b693e-d260-4243-a67b-f952a5c5548c.png)
![4](https://user-images.githubusercontent.com/66065738/151977127-5707590c-32ea-4f55-9907-eeffa587c2ed.png)
![2](https://user-images.githubusercontent.com/66065738/151976418-a77b87e8-720a-4b35-9894-b7df2c661bc2.png)
![3](https://user-images.githubusercontent.com/66065738/151976426-7e9af900-9778-4cb4-8940-2383745d90e0.png)






# References
1) https://ieeexplore.ieee.org/document/8808931
2) https://www.pyimagesearch.com/2017/05/08/drowsiness-detection-opencv/

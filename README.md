# Drowsiness-Detection-in-Real-Time
Drowsiness detection is a safety system that can help avoid accidents caused by drivers who fall asleep behind the wheel. Using image processing techniques, the system captures the videos and recognises the driver's face in each frame. Based on adaptive thresholding, the system detects driver sleepiness by recognising facial landmarks and computing Eye Aspect Ratio (EAR) and Mouth Aspect Ratio (MAR).

# Algorithms and Formulas
Using the Dlib library, the 6 coordinates on each eye and 20 coordinates on the mouth region were marked. Using those landmarks, Eye Aspect Ration (EAR) and Mouth Aspect Ratio (MAR) were calculated as shown in the formulas below:

<p align="center">
          <img src="https://user-images.githubusercontent.com/66065738/152203244-52d8c827-1fbf-4387-8237-c5d63779f741.png">
</p>

<p align="center">
          <img src="https://user-images.githubusercontent.com/66065738/152202994-75fdb868-61b7-4164-973e-1b62c1252800.png">      
</p>

# <p align="center"> EAR=(||p2-p6|| + ||p3-p5||)/2x||p1-p4||)</p>

<p align="center">
          <img src="https://user-images.githubusercontent.com/66065738/152202892-4a3a2c66-a9d1-4249-9651-7204d2fb84c7.png">      
</p>

# <p align="center"> MAR = (||p62-p68|| + ||p63-p67|| + ||p64-p66||)/(3x||p61-p65||) </p>



# Results
<p align="center">
<img src="https://user-images.githubusercontent.com/66065738/151976404-d03b693e-d260-4243-a67b-f952a5c5548c.png">
</p>
<p align="center">          
<img src="https://user-images.githubusercontent.com/66065738/151977127-5707590c-32ea-4f55-9907-eeffa587c2ed.png">
</p>
<p align="center">         
<img src="https://user-images.githubusercontent.com/66065738/151976418-a77b87e8-720a-4b35-9894-b7df2c661bc2.png">
</p>
<p align="center">           
<img src="https://user-images.githubusercontent.com/66065738/151976426-7e9af900-9778-4cb4-8940-2383745d90e0.png">
</p>       






# References
1) https://ieeexplore.ieee.org/document/8808931
2) https://www.pyimagesearch.com/2017/05/08/drowsiness-detection-opencv/

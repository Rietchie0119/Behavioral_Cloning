# Behavioral_Cloning
Self-driving Car program<br/>
This program uses the open source self-driving car simulator offered by Udacity.<br/>

![](https://github.com/Rietchie0119/Lane-detection/assets/28763133/3c437aba-4d0d-44f5-a247-be763e2add57)<br/>
To train the model, I first drove the car three laps to get images and steering angle log. They are stored in Data folder so you can easily access them. In jupyter notebook file, I made training set with each frame and corresponding steering angle. This time, I used Nvidia model to train the data. Finally, I downloaded the trained model.h5 so I can connect to the simulator using Flask. In drive.py file I imported Flask so that the simulator
can communicate through port 4567. The client(simulator) sends each frame to the server app(drive.py) and drive.py computers the appropriate steering angle and throttle value. The simulator receives steering angle and throttle value and autonomously drives the car on the track.<br/>

![](https://github.com/Rietchie0119/Lane-detection/assets/28763133/514990ed-42a5-43c3-831f-57095b42a0bf)<br/>
Just in like road-sign classifier, I incorporated different techniques such as dropout layers, and data augmentation to improve overall performance of the model.<br/>

![](https://github.com/Rietchie0119/Lane-detection/assets/28763133/a366f0c8-7594-47fe-8a61-117209363cfc)<br/>
We're getting approximately 3.95% training loss and 2.93% on validation loss, which means that the model is doing pretty good on predictions.<br/>

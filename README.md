# K-means_demo
Suppose, we want to do vibration analysis of bridges under moving vehicles for its structural health monitoring.
In this demo, I'll be using a breadboard (as a bridge on which vibration analysis has to be performed), a few coin vibration motors(for producing vibrations), an accelerometer module (ADXL355B/ GY-61), and any microcontroller to receive data serially on monitor.
I'll be using K-means algorithm which is an unsupervised learning approach, that helps us visualise the patterns/sub-groups within a population of datapoints.
I have shown three different plots for the same set of readings. It simply means, that the algorithm has clusterised the data in 3 different ways each time.

STEPS:
1. Firstly, we will configure our accelerometer such that it gives 0g readings on monitor, along X and Y-axis. It depicts that bridge is stable.
2. Now, use the first motor and record the readings on a text file.
3. Repeat step 2 for 2 motors, 3 motors, and so on (I have used maximum 5 motors). More the number of motors, more the vibrations on the breadboard, hence more will be the deflections along X and Y-axis.
4. Merge all the readings in one text file.
(The arrangement of motors on the breadboard is shown in pictures).
5. Then we will write a pyhton code for implementing K-means algorithm.
6. I have considered two features here, deflections across x-axis and deflections across y-axis. So, the curve will be a 2-D curve.
7. Now, with all the data in one file, we will feed it to K-means algorithm and plot the curve for K=5.
(The python file and curve is given in this repository).

## About the app
SplitRatioEstimator is an Android application developed to collect data on network stationarity from a wide variety of users. We are interested in gathering information about how the round trip times and available bandwidth of WiFi and Cellular networks vary over time. This information will inform our design for a multipath scheduling algorithm which relies on the assumption that users have access to stationary networks most of the time. 



## How to participate?  

### Prerequisites
Following are the pre-requisites to participate in this study:

1. A cell phone running Android 6,7,8 or 9. 
2. An active WiFi and Cellular connection on the cell phone.


### Steps
If you have the pre-requisites and want to participate in this study, please follow these steps:

1. Click on the "Download APK File" button to download the apk file. You can either directly download the apk file to your cell phone or download it through a computer and then move it to the cell phone.

2. Install the apk file on your Android cell phone. You might need to allow apps to be installed from unknown sources for this step to work. 


## App workflow
The app makes periodic measurements at a frequency communicated to the app through a server. Each measurement comprises of several tasks done in an order. They are listed as follows.

1. Download files of size ranging from 4KB to 8MB in increments of power of 2 (2<sup>12</sup>,2<sup>13</sup>, …, 2<sup>23</sup> bytes) on WiFi. Download logs for each file size are stored locally. Each download log tells how many bytes were received after how much time during the download of a specific size file. 

2. Download files of size ranging from 4KB to 8MB in increments of power of 2 (2<sup>12</sup>,2<sup>13</sup>, …, 2<sup>23</sup> bytes) on Cellular network. Similar to step 1, download logs are stored locally.

3. Compute Split Ratios for all the file sizes through download logs recorded in step 1 and 2. 

4. Estimate available bandwidth on WiFi by downloading a 4MB file three times and computing the mean and standard deviation of the three measurements.

5. Estimate round-trip time on WiFi by downloading a 1KB file.

6. Estimate available bandwidth on Cellular network by downloading a 4MB file three times and computing the mean and standard deviation of the three measurements.

7. Estimate round-trip time on Cellular network by downloading 1KB file.

8. Input the estimated bandwidth and round-trip times to the model and predict split ratios. 

9. Download files of size 4KB to 8MB using the measured and predicted split ratios. Record the download times locally. 


## Privacy Policy
To understand what data we collect and how we use it, please refer to the [Privacy Policy](https://drive.google.com/file/d/1z593pqp7ac1Vk8Sj5OzfaPgq-fXXMYbn/view?usp=sharing).


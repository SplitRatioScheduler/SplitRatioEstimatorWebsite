## SplitRatio Scheduling Algorithm


## User Study


## App Workflow
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
To understand what data we collect and how we use it, please refer to the [Privacy Policy](https://drive.google.com/file/d/1z593pqp7ac1Vk8Sj5OzfaPgq-fXXMYbn/view?usp=sharing)


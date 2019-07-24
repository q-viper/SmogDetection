# Smog-Detection
This repository is created while attending Udacity's Secure and Private AI Challange.
## Dataset available on: <a href = "https://sites.google.com/view/reside-dehaze-datasets"> Here</a>

<h2 align = "center"> What i did? </h2>
<h3> Try1: </h3>

* Downloaded some of datasets and saved each class of image into a single csv file after resize into (100, 100, 3).(Which literally takes more space than entire images.)
* Then merged those files into single list. (I tried numpy array also but showed memory error on 8gb local RAM.)
* Created a numpy array from list, gave class 1 for clear and 0 for smog. Then first label holds class and rest 30000 holds pixel property. Alos normalized data in 0 - 1.
* Created a Simple CNN. Got accuracy 80+.
<h3> Try2:</h3>
* Used Google Colaboratory. And used VGG net.
* Got accuracy 90%.

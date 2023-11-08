# The-Smart-Lustro
 IOT-based smart mirror
Our IOT-based smart mirror detects the face of the person standing in front of it, and then it displays the following personalized information: 
1. To-do list, diet, remainders, and emails 
2. Irrespective of the person scanned, information like weather, news, YouTube videos, etc., can be accessed.
   
<i>The face detection model can be found in the '' file, which used deep learning to train the model in such a way that faces can be recognized even in dark lighting conditions. The algorithm detects the facial expression of the person standing and even sets the smart mirror's mood accordingly</i>
### Hardware requirements:
<ol>
 <li>Wood Frame</li>
 <li>Desktop Monitor</li>
 <li>Raspberry Pi</li>
 <li>Arduino</li>
 <li>Py Cam</li>
</ol>

### Software requirements:
<ol>
 <li>Magic Mirror</li>
 <li>Raspberry Pi Raspbian Buster</li>
 <li>Alexa</li>
</ol>

#### Instructions:
Raspbian Buster Installation

![image](https://github.com/meghsat/The-Smart-Lustro/assets/46103704/53f87db9-4029-4663-a72e-57a36be91b13)

<ol>
<li>Download and install The latest Raspbian OS which can be found on Raspberry Pi</li>
<li>Download Etcher and install the application on your computer. </li>
<li>Plug your Micro SD card Adapter with your SD card into the computer.</li>
<li>Open Balena Etcher and select extracted the image you’ve downloaded.</li>
<li>Ensuring the correct disk has been selected click “Flash!” to begin writing the image to your SD Card. Note: This process could take 10-15 minutes</li>
<li>Remove the SD Card and plug in Pi. Whereby you could access Pi via VNC or Mouse and Keyboard</li>
</ol>

Magic Mirror Installation

![image](https://github.com/meghsat/The-Smart-Lustro/assets/46103704/cabcf6bb-c38d-4e1a-a0e6-99fd29633cf6)

https://magicmirror.builders/

Upon boot-up of the Raspberry Pi, complete the remaining setup, and ensure you’re connected to the internet via LAN/Wi-Fi. Full instructions and extra features can be found here: https://docs.magicmirror.builders/getting-started/installation.html#manual-installation

![image](https://github.com/meghsat/The-Smart-Lustro/assets/46103704/08d44a8a-e0f5-4428-a84f-f4ddb7ba844d)

<i>Nodejs</i>
```
curl -sL https://deb.nodesource.com/setup_10.x | sudo -E bash -
sudo apt install -y nodejs
```
<i>Clone the repository and check out the master branch: </i>
```
git clone https://github.com/MichMich/MagicMirror
cd MagicMirror/
```
<i>Install the application: </i>
```
npm install
```
<i>Make a copy of the config sample file:</i>
```
cp config/config.js.sample config/config.js
```
```
npm run start
npm run server 
```


### Installing the modules:
```
 cd ~/MagicMirror/modules
   git clone https://github.com/meghsat/The-Smart-Lustro.git
   cd TheSmartLustro
   npm install
```

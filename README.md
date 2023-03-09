# Make you own Raspberry Pi Camera Stream

Created a custom live stream from a Raspberry Pi using the Pi camera module.

## Dependencies

```
sudo apt-get update
sudo apt-get upgrade

sudo apt-get install libatlas-base-dev
sudo apt-get install libjasper-dev
sudo apt-get install libqtgui4
sudo apt-get install libqt4-test
sudo apt-get install libhdf5-dev

sudo pip3 install flask
sudo pip3 install numpy
sudo pip3 install opencv-contrib-python
sudo pip3 install imutils
sudo pip3 install opencv-python

```

## Clone the project
Open up terminal and clone the Camera Stream repo:

```
cd /home/pi
git clone https://github.com/vishwshah/desktop-tutorial.git
```

## Launch Stream

Note: Creating an Autostart of the main.py script to keep the stream running on bootup.
```bash cd modules
sudo python3 /home/pi/pi-camera-stream-flask/main.py
```

## Autostart Pi Stream

```
sudo nano /etc/profile
```

Go the end of the and add the following (from above):

```
sudo python3 /home/pi/pi-camera-stream-flask/main.py
```

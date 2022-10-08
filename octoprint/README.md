# OctoPrint

```sh
sudo docker run -d -v octoprint:/octoprint --privileged --device /dev/ttyUSB0:/dev/ttyUSB0 --device /dev/video0:/dev/video0 -e ENABLE_MJPG_STREAMER=false -p 8080:80 --name octoprint octoprint/octoprint

# debug usb connection issues - should be accessible on /dev/ttyUSB0
ls /dev.ttyUSB*
sudo dmesg

# sudo pip3 install vcgencmd
https://stackoverflow.com/questions/70123431/why-would-ch341-uart-is-disconnected-from-ttyusb
sudo apt remove brltty



```

## Resources
https://www.frakkingsweet.com/octoprint-and-kubernetes
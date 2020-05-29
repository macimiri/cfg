Logitech Options remapping!
https://github.com/PixlOne/logiops
1. sudo apt install cmake
2. sudo apt install libevdev-dev
3. sudo apt install libudev-dev
4. sudo apt install libconfig-dev
5. sudo apt install libconfig++-dev (yes, really)
6. then follow instructions for building, installing on the github page
7. copy the logid.cfg file to /etc/
9.to get it to start up at reboot, run
	sudo systemctl start logid (to get it going first)
	sudo systemctl enable logid (to get it starting on reboot)

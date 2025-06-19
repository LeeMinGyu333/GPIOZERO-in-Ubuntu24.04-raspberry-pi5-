# GPIOZERO-in-Ubuntu24.04-raspberry-pi5-

sudo apt update
sudo apt install python3-gpiozero
(venv) pip install gpiozero
pip install lgpio --break-system-packages  # or env
pip3 install rpi-lgpio

# give the authorize to gpio group
sudo nano /etc/udev/rules.d/99-rpi)gpio.rules
#add that 1 line
SUBSYSTEM=="gpio", KERNEL=="gpiochip*", MODE="0666"
#close
sudo udevadm control --reload-rules
sudo udevadm trigger
sudo reboot


# NOW we have a test code in this repository.
# Just send this python file to your Pi and use it in Terminal

sudo python3 zerg2.py

산딸기 렛ㄱㄱ

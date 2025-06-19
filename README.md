# GPIOZERO-in-Ubuntu24.04-raspberry-pi5-

sudo apt update
sudo apt install python3-gpiozero
(venv) pip install gpiozero
pip install lgpio --break-system-packages  # or env

# give the authorize to gpio group
sudo groupadd gpio
sudo usermod -aG gpio username
sudo reboot

# if u want to check this change.
groups username

# NOW we have a test code in this repository.
# Just send this python file to your Pi and use it in Terminal

sudo python3 zerg2.py

산딸기 렛ㄱㄱ

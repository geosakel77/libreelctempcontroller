sudo nano /etc/rc.local
python /home/pi/fan.py &



stress test

sudo apt-get install stress
wget https://raw.githubusercontent.com/ssvb/cpuburn-arm/master/cpuburn-a53.S
gcc -o cpuburn-a53 cpuburn-a53.S (edited)

while true; do vcgencmd measure_clock arm; vcgencmd measure_temp; sleep 10; done& stress -c 4 -t 900s

# Raspberry-Pi-IoT-2018
This is a project to that purely uses php and wirepy to remotely control the Raspberry pis GPIO. This will work on most of the raspberry pi. 
Before you can start working with PHP on Raspberry Pi, you need to install PHP itself on the machine. In most situations, PHP is used in tandem with a web server like Apache. Installing both PHP and Apache on Raspberry Pi is a matter of running.

1.Install php in a raspberry pi.Php is shipped alongside appache or lighttpd. To install either, 

sudo apt-get install apache2 php5
sudo apt-get install lighttpd php5

2.Deploy the Wiring Pi library for working with GPIO pins and then use the library with PHP via the shell_exec() function. For this solution to work, you need to install Wiring Pi on Raspberry Pi first.

Start with installing the Git software using:
sudo apt-get install git-core

Then, clone the Wiring Pi Git repository by running:
git clone git://git.drogon.net/wiringPi

3.Switch to the resulting wiringPi directory and use the ./build command to compile and install Wiring Pi:

cd wiringPi
./build

4.To make sure Wiring Pi is installed and works properly, run the  command; 
gpio -v

It should return the current version of Wiring Pi along with the basic Raspberry Pi info. 

5. Execute the gpio readall command to view a detailed GPIO layout diagram.
gpio readall

6.Connect an LED with a resistor to GPIO pin 17 and GND as shown,
 No Image.
7.Open the terminal on your Raspberry Pi (or connect to it via SSH) and switch to the /var/www directory. 
Then, create the gpio.php file for editing.
sudo nano gpio.php.

Place the code in the gpio.php.





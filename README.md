
This piece of code was combined from several sources:

https://github.com/adafruit/Adafruit_BME280_Library
https://cdn-shop.adafruit.com/datasheets/BST-BME280_DS001-10.pdf
https://projects.drogon.net/raspberry-pi/wiringpi/i2c-library/

Tested on RASPBIAN JESSIE LITE
https://www.raspberrypi.org/downloads/raspbian/

```
git clone https://github.com/andreiva/raspberry-pi-bme280.git

```

Dependencies
```
sudo apt-get install libi2c-dev i2c-tools wiringpi
```
Compiling
```
make
```
Copy binary to /usr/bin
```
sudo cp bme280 /usr/bin
```
Now you should be able to run the program, simply by typing
```
bme280
```
Output should look like this
```
(25.58, 54.36, 1011.89)

```
ugly but it works

mysql -u user -pgeheim database -e  "INSERT INTO table(temp,humidity, pressure) VALUES $(./bme280)"

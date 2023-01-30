# 0-10v PWM LED Dimming Controller (includes Home Assistant Integration)

This repository provides the code and instructions to build a custom LED dimming controller using 0-10v pulse-width modulation (PWM) technology including the code and setup to integrate with Home Assistant. The controller allows for precise adjustment of LED light brightness and is a cost-effective and personalized solution compared to commercially available dimming options.  Includes stl for 3D printed case.

## Parts Needed
- [ESP32](https://www.google.com/search?q=ESP32+development+boards) or [ESP8266](https://www.google.com/search?q=ESP8266+development+boards) development board with [SPI pins](https://www.google.com/search?q=spi+pins)  
This baby right here is the mastermind behind our controller setup. It's got Wi-Fi built in and can easily connect to your Home Assistant server through the ESPHome plugin. And the best part? We're using a wicked cheap [Wemos D1 Mini ESP8266](https://www.google.com/search?q=wemos+mini+d1) for this project.  
    <img src="/images/esp8266%20wemos%20d1%20mini.jpg" height="150">

- [10v AC/DC Wall Plug Adapter](https://www.digikey.ca/en/products/detail/globtek-inc/WR9HU1800LCP-F-R6B/10187591)  
This here is the type of plug we're gonna use to power up our project. Keep in mind, all we really need is a 10V power supply, so feel free to switch it up if you want. We'll be using a wire terminal to connect this to both the Adafruit PWM board and the LM2596 voltage regulator board.  
    <img src="/images/10v%20AC-DC%20Wall%20Plug%20Adapter.jpg" height="150">

- [Adafruit TLC5947 **24-Channel** 12-bit PWM LED Driver](https://www.adafruit.com/product/1429)
or [Adafruit TLC59711 **12-Channel** 16-bit PWM LED Driver](https://www.adafruit.com/product/3995)  
These boards are capable of generating PWM signals up to 30v! The PWM voltage that the board produces is based on the voltage you feed to it (hence the 10v power supply).  
    <img src="/images/Adafruit%2024%20channel%20PWM%20LED%20driver.jpg" height="150"> <img src="/images/Adafruit%2012%20channel%20PWM%20LED%20driver.jpg" height="150">

- 2x [Break-Away 0.1" 2x20-pin Strip Dual Male Headers](https://www.google.com/search?q=Break-Away+0.1%22+2x20-pin+Strip+Dual+Male+Header) or 8 3x2 pin headers  
We will cut these down to 3x2 segments and solder them onto the PWM board.  
    <img src="/images/Break-Away%200.1-inch%202x20-pin%20Strip%20Dual%20Male%20Header.jpg" height="150">

- [LM2596 DC to DC Voltage Regulator 4-40V to 1.5-35V Buck Converter with LED Display](https://www.google.com/search?q=LM2596+DC+to+DC+Voltage+Regulator+4-40V+to+1.5-35V+Buck+Converter+with+LED+Display)  
So we've got our PWM board that needs a 10V power source. But wouldn't it be awesome if we could use that same power supply to juice up our ESP too? The only catch is that the ESP runs on 5V, and 10V is just too high. That's where this regulator board comes in - it lets us connect the 10V source and then dial it down to the perfect 5V for our ESP. Sweet, right?   
    <img src="/images/LM2596-DC-to-DC-Voltage-Regulator.png" height="150">



- _wagos/wirenuts_
- _project box (need size)_

# To be added:
## Assembly Instructions
## Software Configuration
## Usage

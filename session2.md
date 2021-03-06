---
layout: default
title: Session 2- General Purpose IO, Interrupts, PWM and Servos
date: September 4, 2013
---

##Session 2 - General Purpose IO, Interrupts, PWM and Servos

Our second class will jump into the use of input/output ports then move on to driving motors, fading LEDs and playing back sounds. We'll learn about how to use the Raspberry Pi to control actuators or light up LEDs. We'll also discover how to read digital inputs like switches and sensors. Finally, we'll move on to an explanation of Pulse Width Modulation (PWM) and how to use it on the Raspberry Pi. 

#### Updating the RPi-GPIO Library
  To use the interrupt features of the RPi-GPIO library, we need to upgrade to the latest version. Run these commands on your Raspberry Pi:
{% highlight bash %}
  wget https://raspberry-gpio-python.googlecode.com/files/python-rpi.gpio_0.5.3a-1_armhf.deb
  sudo easy_install pip
  sudo pip uninstall RPi.GPIO
  sudo dpkg -i python-rpi.gpio_0.5.3a-1_armhf.deb
{% endhighlight %}

Once complete, you can check the installation by running: 
{% highlight bash %}
python -c "import RPi.GPIO; print RPi.GPIO.VERSION"
{% endhighlight %}
You should see the value "0.5.3a" printed out.


##Class Resources
* [Bash Control of GPIO](session2/bash.html)
* [LED Blink and Stopwatch](session2/project1-beginner.html)
* [Polled and Interrupt Driven Input](session2/input.html)
* [Reaction Timer](session2/project2-beginner.html)
* [PWM And Servo Control](session2/pwm-servo.html)

##Projects
* [Simon Says](session2/project1-intermediate.html)
* [Frequency Counter - Under Construction]()




<br/>

## References
* [Breadboard Connections](https://dl.dropboxusercontent.com/u/1733921/Raspberry%20Pi/Breadboard%20Connections.jpg)
* [raspberry-gpio-python Documentation](https://code.google.com/p/raspberry-gpio-python/wiki/Examples)

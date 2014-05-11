Living Robots
=============
 
Living Robots, is the Github repository for the new Ebook about LeJOS "Living Robots with EV3".
http://juanantonio.info/lejos-ebook/

"Living Robots with EV3" is a ebook designed to learn about development of Robots with modern techniques and technologies. The book put the focus in the platform Lego Mindstorms EV3, Linux and the programming language Java. The ebook cover modern topics as "Internet of things" (IOT) and the integration with other technologies as Web, Raspberry PI & Arduino.

Help the project with a donation or book your copy. Further information here: http://juanantonio.info/lejos-ebook/

    2014/05/04: First commit

## Chapter 0:

Downloads: https://github.com/jabrena/livingrobots/raw/master/chapter0/docs/LRWE_Chapter0.pdf

## Chapter 1: Introduction

### Lego Mindstorms

![ScreenShot](https://raw.githubusercontent.com/jabrena/livingrobots/master/LDD/Base1/Base1_5.png)

### LeJOS Project

### Alternatives to Lego Mindstorms

## Chapter 2: Fundamentals of Robotics

Pending

## Chapter 3: Sensors

In this chapter, we will cover the most popular and useful sensors compatible with EV3 Brick.

### Exteroceptors sensors

Exteroceptors are sensors that measure the positional or force-type interaction of the robot with its environment. 

    Example: IRSensor to detect a Beacon
    Example: The magic 8 ball using a EV3GyroSensor

### Proprioceptors sensors

Proprioception in robotics means sensing the internal state of the robot or a part of it . For example the posture of a mechanical manipulator, leg or other jointed mechanism or the battery level.

## Chapter 4: Actuators

Pending

## Chapter 5: Navigation

In this chapter, user will learn basic concepts about Local & Global navigation

### Occupancy grid maps

![ScreenShot](https://raw.githubusercontent.com/jabrena/livingrobots/master/chapter8/docs/mapping.png)

### References

http://www.cs.ox.ac.uk/people/michael.wooldridge/teaching/robotics/lect05.pdf

https://github.com/edgemaster/robotics/tree/master/lejos/tut5Probability/src/navigation

## Chapter 6: Cognition

Pending

## Chapter 7: Computer vision

Pending

## Chapter 8: Web interfaces

In this Chapter, the reader will learn many stuff about Web Servers and  Web interfaces for robots with EV3 Brick.

### Web Servers

In this section, user will learn the different among httpd and other developments in Java to run a Web Server as NanoWeb server.

    root@(none):~# start-stop-daemon -K -n httpd
    stopped httpd (pid 1823)
    root@(none):~# httpd -v -h /home/lejos/www/

An example when the httpd is pretty busy:

    Mem: 49048K used, 11812K free, 0K shrd, 516K buff, 25556K cached
    CPU:   8% usr  35% sys   0% nic   0% idle   0% io  15% irq  39% sirq
    Load average: 11.89 12.35 10.50 17/101 9146
      PID  PPID USER     STAT   VSZ %MEM %CPU COMMAND
     1551  1197 root     S     178m 300%  16% /home/root/lejos/ejre1.7.0_55/bin/java
     1735     1 root     R     2880   5%  11% httpd -v -h /home/lejos/www/ 

Nano Web server running on EV3 and suffering a DOS Attack:

    Mem: 59800K used, 1060K free, 0K shrd, 48K buff, 4288K cached
    CPU:  23% usr  26% sys   0% nic   0% idle  23% io   9% irq  17% sirq
    Load average: 3.60 1.78 0.77 1/373 2030
    PID  PPID USER     STAT   VSZ %MEM %CPU COMMAND
    1577  1538 root     S     266m 447%  43% /home/root/lejos/ejre1.7.0_55/bin/java -classpath /ho
        4     2 root     SW       0   0%  11% [events/0]
      430     2 root     DW       0   0%   8% [mmcqd]
     1538  1184 root     S     179m 301%   5% /home/root/lejos/ejre1.7.0_55/bin/java -classpath /ho
      180     2 root     DW       0   0%   4% [kswapd0]
     1594  1567 root     R     3072   5%   2% top 

### Web Interfaces

In this section, user will learn basic stuff about Modern web development.

### Websockets

In this section, user will learn to develop a distributed application using Websockets technology.

![ScreenShot](https://raw.githubusercontent.com/jabrena/livingrobots/master/chapter8/docs/remoteControl.jpg)

### References

https://jcp.org/en/jsr/detail?id=356

https://tools.ietf.org/html/rfc6455

https://github.com/TooTallNate/Java-WebSocket

https://github.com/NanoHttpd/nanohttpd

## Chapter 9: Communications

This chapter covers the following technologies: Websockets, Http, RMI, D-Bus & I2C.

## Chapter 15: Hacking robots

It is very important to ensure that your robot operates in a secure environment. Learn some stuff about security for Robots and avoid future robot's hacks.

![ScreenShot](https://raw.githubusercontent.com/jabrena/livingrobots/master/chapter15/docs/Tachikoma.png)

In this chapter you will learn some concepts about security for Unix. Remember that your EV3 Brick run over a Busybox distro.

### Examples

The examples included in this chapter are:

    Example: Discover ports opened in your EV3 Brick
    Example: Hack your SSH root account using Brute force
    Example: Read /var/volatile/log/ to discover ssh attacks
    Example: A mini example about a DOS Attack to the service httpd included Busybox
    Example: Shell scripts to remove some no necessary processes

### Exercises

    Exercise 1: How to add a program in the startup
    Exercise 2: Create a Virus for EV3 brick

### References

http://freeware.the-meiers.org/

http://www.openwall.com/john/

http://www.jcraft.com/jsch/

https://www.thc.org/thc-hydra/

http://nmap.org/

## Annexes

## Annex 1: Getting started with LeJOS

### References

http://sourceforge.net/p/lejos/wiki/Getting%20started%20with%20leJOS%20EV3/

## Annex 2: Busybox

LeJOS project uses Busybox as the way to offer a Linux experience. It was specifically created for embedded operating systems with very limited resources. BusyBox provides several stripped-down Unix tools in a single executable file. The authors dubbed it "The Swiss Army Knife of Embedded Linux", as the single executable replaces basic functions of more than 300 common commands

In this Annex, the reader will learn how to use Busybox in a EV3 environment.

Download preview: https://github.com/jabrena/livingrobots/raw/master/annex2/docs/LRWE_Annex2_Busybox.pdf 

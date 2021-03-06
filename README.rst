
********************************************************
Adapting OV7670 camera module with Nexys4 DDR board
********************************************************

.. contents:: Table of Contents
   :depth: 2
   
Introduction 
=======================
The project is done in Vivado 2016.3. A camera module OV7670 is addapted to the nexys4DDR board. The camera module is configured using I2C interface. The register configuration is preloaded in the FPGA. A simple BRAM is used on the FPGA is used to buffer the captured video data. The buffered data will then be sent to the VGA output and displayed on the monitor.

The source HDL code of this project is from this `Github Repository <https://github.com/laurivosandi/hdl.git>`_. This code is packed and modified a little bit to be able to run it on Nexys4DDR board.

Also, this `page <http://hamsterworks.co.nz/mediawiki/index.php/OV7670_camera>`_ offered a lot of useful information when I started.

This is the first github project I have ever created. The project itself is simple and straight forward, all I want is to get familiar with Github and reStructuredText. Hopefully this is helpful for you if you are new to FPGA.

Camera Interface
=======================
.. image:: https://github.com/bwang40/OV7670_NEXYS4DDR_HDL/blob/master/images/ov7670.PNG
   :scale: 25
+---+----+---+----+
|PIN|SIG |PIN|SIG |
+===+====+===+====+
|1  | D1 |2  | D0 | 
+---+----+---+----+
|3  | D3 |4  | D2 | 
+---+----+---+----+
|5  | D5 |6  | D4 | 
+---+----+---+----+
|7  | D7 |8  | D6 | 
+---+----+---+----+
|9  | PCK|10 | XCK| 
+---+----+---+----+
|11 | VS |12 | HS | 
+---+----+---+----+
|13 | SCL|14 | SDA| 
+---+----+---+----+
|15 | 3V3|16 | GND| 
+---+----+---+----+





IP-core Creation
=======================




Result
=======================

.. image:: https://github.com/bwang40/OV7670_NEXYS4DDR_HDL/blob/master/images/IMG_4585.JPG

.. image:: https://github.com/bwang40/OV7670_NEXYS4DDR_HDL/blob/master/images/IMG_4587.JPG


Summary
=======================

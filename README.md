# Alexa-ACK

The ACK is a SW and Hw developed by Amazon with espressif partnership to simplify and improve the connection system with alexa devices to IoT application. reading a qrcode is all it takes to connect our device alexa
The ACK espressif use the “esp32-pico-v3-zero” with dedicated amazon firmware in the ACK.
In this work we introduce the Amazon material with some tips to make this system work.

- HELLOWORLD.INO and others root files: this files will be edited by the user to make work, like he want, the hmcu interface.
- SRC: library of IMPL.CORE, responsible for the communication between ACK and HMCU;
- The ack_arduino_platform.cpp: this file can be changed by the user, because it is the interface between IMPL.CORE files (from src folder);
- If your HMCU is a STM core you will have do the following:
o Change: Serial”n” to UART”n”;
o Add Hardware Serial UART1(PB7,PB6) and UART3(PB11,PB10);
- I add the “HelloWorld_2” with the needed changes to test a prototype;
- It is essential read all Amazon Material that you find in the links of file “important alexa.txt”.
Enjoy yourself!!!

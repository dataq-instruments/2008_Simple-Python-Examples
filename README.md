# DI-2008 Simple Python Examples


**Prerequisites**:

1) Install Python (3.9 was what the program was tested on)

2) Install Pyserial and Keyboard (from command prompt if you are using Window)
    - python -m pip install -U pyserial --user
    - python -m pip install -U keyboard --user
    - If you are in Linux, and keyboard is not available, you will have to modify the codes reference to it

3) Latest firmware is recommended https://github.com/dataq-instruments/2008_Firmware_Upgrade. 

4) Understand the protocol, please refer to  https://www.dataq.com/resources/pdfs/misc/Dataq-Instruments-Protocol.pdf

5) Turn DI-2008 into CDC mode: plug the device to USB port, if the LED already blinks Yellow, stop, you are already in CDC mode. If not, once the LED turns blinking Green, push the button 5 times, the LED should blink yellow to indicate CDC mode. If you need to exit CDC mode, repeate the same action and a green blinking LED will indicate LibUSB mode.

6) Find out the COM port in use

    - From Windows Device Manager, find out the COM port of the device connected to, and modify the program accordingly<br/>
    ![alt text](https://www.dataq.com/resources/repository/matlab_devicemanager.png)
    
7) Modify the sample with the correct COM port number 

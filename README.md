# Xojo_lgpio_Interrupt_SR04
In the Xojo programming language, an Interrupt is created to accurately determine when a button has been pressed.

This example has code to run an interrupt which notifies the user when the button has been pressed, and does not take additional time or resources. Using the interrupt-option saves cycle resources on the Raspberry Pi and makes the program run faster. Switch debouncing has also been added.

Below is the electrical schematic for the Raspberry Pi.

![](https://github.com/eugenedakin/Xojo_lgpio_Interrupt_SR04/blob/main/InterruptSchematic.png)


Below is a screen grab from the running program.

![](https://github.com/eugenedakin/Xojo_lgpio_Interrupt_SR04/blob/main/ScreenGrab.png)


The lgpio library can be installed Raspberry Pi OS (2026) and instructions are available at https://github.com/joan2937/lg (updated 2024)

Install instructions are:

1. install Raspberry Pi OS (64-bit)
2. Open a terminal and type the following commands:
3. sudo apt install swig python3-dev
4. sudo apt install python3-setuptools
5. sudo apt install libunwind8
6. wget https://github.com/joan2937/lg/archive/master.zip
7. unzip master.zip
8. cd lg-master
9. make
10. sudo make install
11. create an Example program and copy the program and libraries to the RaspberryPi Desktop (make a 64-bit version)
12. give the executable permission to run with something like: 'sudo chmod +x Example'
13. run the program with something like: 'sudo ./Example'

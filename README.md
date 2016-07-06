# YARM_DEV Project
##Two simple project to speed up the hands on YARM_DEV!
Download the project and uncompress inside the *Atmel Studio\7.0\* forder.

###YARM2_8510_L21_YARM_TX_Simple
This project simulate a weather station that transmit every 30 sec the pressure, temperature and humidity.
And if you shake the board, the accelerometer starts two events: *ACTIVITY* and *INACTIVITY*. For this events 
the radio send two messages. The log is enabled. You can use the serial port to see them.
On this project I use the AES module as **cryptographic hashing function**, to hash the MCU UID. The goal is to reduce the 128 bit MCU UID to a more suitable length, like 32bit, maintaining a good uniqueness.


###YARM2_8510_L21_YARM_RX_Simple
This project is for the YARM receiver station. The USB port is configured as serial port.

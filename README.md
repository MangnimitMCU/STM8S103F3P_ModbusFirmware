# STM8S103F3P_ModbusFirmware

### Hardware Modify
![1a.jpg](https://github.com/MangnimitMCU/STM8S103F3P_ModbusFirmware/blob/main/1a.jpg)

![1.jpg](https://github.com/MangnimitMCU/STM8S103F3P_ModbusFirmware/blob/main/1.jpg)

![3.jpg](https://github.com/MangnimitMCU/STM8S103F3P_ModbusFirmware/blob/main/3.jpg)

### Device Address Config
# -- Address --
0x4000

### -- Value --
0x0001 - 0x00FF

### example
### read addr
00 03 40 00 00 01 90 1B

### set addr 1
00 06 40 00 00 01 5C 1B

### set addr 2
00 06 40 00 00 02 1C 1A

### Baud Rate Config
### need restart after setting
### -- Address --
0x2000

### -- Value --
- 0x0000 : 9600
- 0x0001 : 19200
- 0x0002 : 38400
- 0x0003 : 57600
- 0x0004 : 115200
- 0x0005 : 128000
- 0x0006 : 256000

### example
### read baud rate
00 03 20 00 00 01 8E 1B

### set baud rate 9600
00 06 20 00 00 00 83 DB

### set baud rate 19200
00 06 20 00 00 01 42 1B

### set baud rate 38400
00 06 20 00 00 02 02 1A

### set baud rate 57600
00 06 20 00 00 03 C3 DA

### set baud rate 115200
00 06 20 00 00 04 82 18

### set baud rate 128000
00 06 20 00 00 05 43 D8

### set baud rate 256000
00 06 20 00 00 06 03 D9

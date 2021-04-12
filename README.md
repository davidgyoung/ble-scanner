# BLE Scanner

A command line utility for Bluetooth LE scanning on Linux / BlueZ

## Compiling

1. Install prerequisites

`sudo apt-get install libbluetooth-dev`

2. Compile the program

`cc scanner.c -lbluetooth -o scanner`

## Running

Run the program like this:

`./scanner`

Each time it detects a Bluetooth LE advertisement it prints out the MAC address of the advertisting device, the RSSI and the bytes of the advertisement like this:

```
B8:27:EB:1F:93:4D -68 02 01 06 11 06 82 75 25 D9 37 9D D7 8F 5F 4A F4 20 00 00 75 30
71:5C:23:9D:BC:7F -68 02 01 1A 02 0A 0C 0B FF 4C 00 10 06 03 1A 3B D4 B2 EB
B8:27:EB:1F:93:4D -68 02 01 06 11 06 82 75 25 D9 37 9D D7 8F 5F 4A F4 20 00 00 75 30
```

In the first line above, `B8:27:EB:1F:93:4D` is the hardware MAC address, -68 is the RSSI and the remaining values are the hex bytes of the advertisement.

## Need Help?  Want to change this?

Feel free to open an Issue or submit a Pull Request on Github here: https://github.com/davidgyoung/ble-scanner


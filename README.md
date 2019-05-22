

# Iiyama screen

Turn iiyama screen on/off using REST GET request.
## Installation

Enter to the project folder from terminal ("iiyama-windows" for Windows system, "iiyama-linux" for Linux system, iiyama-macos for Mac) and type:

```bash
npm install
```
Once the process is done, edit the serialScreen parameter of config.json file to use the serialport that is connected the RS232 cable of the screen.
Example Linux:

```bash
"serialScreen":"/dev/ttyUSB0"
```
Example Windows

```bash
"serialScreen":"COM5"
```
Example MacOS

```bash
"serialScreen":"/dev/tty.usbserial-14330"
```

## Start server

Linux:

```bash
./screen-linux
```

Windows:

```bash
./screen-win.exe
```

MacOS:

```bash
./screen-macos
```


## Usage

Use get requests to turn on and off the screen. Replace the IP address with the corresponding to the IP of your device. 
Port listening: 3000

To turn on:

 ```bash
http://192.168.1.120:3000/on
```

To turn off:

 ```bash
http://192.168.1.120:3000/off
```

## Author

Frosyni Boziki Siman,
<frosyni.boziki@hmy-group.com>

# Application

This project was generated with [Angular CLI](https://github.com/angular/angular-cli) version 6.2.1.

## Development server

Run `ng serve` for a dev server. Navigate to `http://localhost:4200/`. The app will automatically reload if you change any of the source files.

## Code scaffolding

Run `ng generate component component-name` to generate a new component. You can also use `ng generate directive|pipe|service|class|guard|interface|enum|module`.

## Build

Run `ng build` to build the project. The build artifacts will be stored in the `dist/` directory. Use the `--prod` flag for a production build.

## Running unit tests

Run `ng test` to execute the unit tests via [Karma](https://karma-runner.github.io).

## Running end-to-end tests

Run `ng e2e` to execute the end-to-end tests via [Protractor](http://www.protractortest.org/).

## Further help

To get more help on the Angular CLI use `ng help` or go check out the [Angular CLI README](https://github.com/angular/angular-cli/blob/master/README.md).
# Angular-Project



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

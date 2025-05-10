# t25
![image](/web/assets/logo/wide.jpg)

<div align="center">
<strong>
<samp>

[English](README.md) 

</samp>
</strong>
</div>

### Main Features
* Various types of data supported, including CAN, acceleration, GPS, digital/analog signals and wheel speeds
* Micro SD card support
* Real-time telemetry
* Real world time tracking via RTC
* Web based data visualization and analysis tools

### [Documentation](https://github.com/1tz-j0rdan/t25/wiki)

t25 consists of `TMA-1` datalogger, `TMA-2` telemetry monitor and `TMA-3` data analysis tools.

<br>

## TMA-1 Datalogger
TMA-1 is an onboard device that gathers data from the car. It can record the following data:

* CAN 2.0(A/B) bus traffic
* 8-channel digital input signals
* 4-channel analog input signals
* 4-channel external wheel speed sensors (digital pulse period)
* 3-axis ±4g acceleration (ADXL345)
* GPS informations (NEO-6/7M)
* Supply voltage(LV) and internal CPU temperature
* Real world time(RTC)

Refer to the [TMA‐1 Features and Usage Guide](https://github.com/1tz-j0rdan/t25/wiki/%5BEN%5D-TMA%E2%80%901-Features-and-Usage-Guide) for detailed explanations about each feature.

### 1-1. TMA-1 Do It Yourself!
TMA-1 is a datalogger. It is designed with commercial modules and through-hole components for easy build.

Required components and build instructions are described in the [TMA-1 DIY Guide](https://github.com/1tz-j0rdan/t25/wiki/%5BEN%5D-TMA%E2%80%901-DIY-Guide).

<img src='https://github.com/1tz-j0rdan/t25/assets/17094868/062e846b-619e-4b5e-a784-63690c4cd73f' style='width: 700px'>

### 1-2. TMA-1 Configuration Tool
This is a GUI tool that builds and uploads the firmware to the TMA-1 with configured features.

With this tool, you can activate features in the datalogger, synchronize TMA-1's clock to your computer time, and configure the networks for the telemetry.

For the detailed information, please refer to the [TMA-1 Configuration Tool Guide](https://github.com/1tz-j0rdan/t25/wiki/%5BEN%5D-TMA%E2%80%901-Configuration-Tool-Guide).

<img src='https://github.com/1tz-j0rdan/t25/assets/17094868/2350a23e-c4a7-4766-830a-d4313ee9fbee' width='700px'>

<br><br>

## TMA-2 Telemetry monitor
TMA-2 consists of the telemetry server that TMA-1 communicates with, and the web client for real-time data monitoring.

### Server
Users do not need to set up the server individually, except in case you want your own server. TMA-1 uses the default t25 server for the telemetry.

If you want to self-host your own server, follow the [TMA-2 Server Setup Guide](https://github.com/1tz-j0rdan/t25/wiki/%5BEN%5D-TMA%E2%80%902-Server-Setup-Guide).

### Client
Real-time monitoring client is served at https://cfsaetelemetry.site.

Each user can set up their own UI with their preferences. It also supports the UI export and import features.

For the detailed information, please refer to the [TMA‐2 Client Usage Guide](https://github.com/1tz-j0rdan/t25/wiki/%5BEN%5D-TMA%E2%80%902-Client-Usage-Guide).

<img src='https://github.com/1tz-j0rdan/t25/assets/17094868/5ba95b27-f435-4d70-a965-757269b4843e'>

<br><br>

## TMA-3 Log Translator and Data Analysis Tool
TMA-1 datalogger stores the log in the SD card in a binary format, according to the predefined [protocol](https://github.com/1tz-j0rdan/t25/wiki/%5BEN%5D-Log-Protocol).

TMA-3 is a set of tools that can translate binary logs to human-readable format(JSON/CSV) and visualize the collected data into graphs and a map.

All these features are web application services that can be instantly accessed.

For the detailed information, please refer to the [TMA‐3 Data Analysis Tool Guide](https://github.com/1tz-j0rdan/t25/wiki/%5BEN%5D-TMA%E2%80%903-Data-Analysis-Tool-Guide).

<img src='https://github.com/1tz-j0rdan/t25/assets/17094868/7734849b-b7c6-4fe3-9ab6-27e2969be806' width='700px'>

<br><br>


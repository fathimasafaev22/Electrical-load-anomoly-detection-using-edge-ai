# Electrical Load Anomaly Detection System Using Edge AI

## Overview

This project presents a real-time Electrical Load Anomaly Detection System using Edge AI and ESP32. The system continuously monitors electrical load conditions and detects abnormal power consumption patterns such as overloads, current spikes, and fluctuations. By performing AI inference directly on the edge device, the system provides fast and reliable anomaly detection without cloud dependency.

## Problem Statement

Traditional electrical monitoring systems rely on manual supervision or simple threshold-based methods, which may fail to accurately detect abnormal load conditions. This project addresses the need for a low-cost, real-time, AI-powered anomaly detection system capable of operating on embedded hardware.

## Objectives

* Monitor electrical load conditions in real time.
* Detect abnormal power consumption patterns.
* Perform AI inference on an ESP32 microcontroller.
* Provide immediate visual and audio alerts.
* Improve electrical safety and energy efficiency.

## Features

* Real-time electrical load monitoring
* Edge AI-based anomaly detection
* ESP32 embedded implementation
* OLED display for live status updates
* Buzzer alert for anomaly conditions
* Low-cost and energy-efficient design
* Cloud-independent operation

## System Architecture

Sensor → ESP32 ADC → Feature Collection → Edge AI Model → Decision Logic → OLED Display & Buzzer

### Workflow

1. Electrical load data is collected using a current/load sensor.
2. ESP32 converts analog sensor values into digital data.
3. Multiple samples are collected and converted into feature arrays.
4. The trained Edge AI model performs classification.
5. The system identifies the load condition as:

   * NORMAL
   * ANOMALY
6. Results are displayed on the OLED screen.
7. A buzzer is activated when an anomaly is detected.

## Hardware Components

* ESP32 Development Board
* Electrical Current/Load Sensor
* OLED Display (SSD1306 I2C)
* Active Buzzer Module
* Breadboard
* Connecting Wires
* Power Supply

## Software Tools

* Arduino IDE
* Edge Impulse Studio
* Serial Monitor

## Dataset

A custom dataset was collected from different electrical load conditions:

### Normal Condition

* Single 9W, 12V bulb

### Abnormal Condition

* Three bulbs connected in parallel:

  * 9W, 12V
  * 12W, 12V
  * 12W, 12V

The collected sensor data was uploaded to Edge Impulse for training and validation.

## Results

The developed system successfully detected electrical load anomalies in real time.

### Performance Metrics

| Metric            | Actual Value   |
| ----------------- | -------------- |
| Accuracy          | 92%            |
| Latency           | 500 ms         |
| Power Consumption | 120 mW         |
| Throughput        | 1 Decision/sec |
| Reliability       | High           |

## Applications

* Smart Energy Monitoring
* Industrial Electrical Systems
* Predictive Maintenance
* Electrical Safety Systems
* Smart Homes and Buildings
* IoT-based Monitoring Systems

## Future Improvements

* Support for multiple anomaly categories
* Wireless cloud dashboard integration
* Mobile application alerts
* Advanced deep learning models
* Smart grid integration

## SDG Alignment

### SDG 7 – Affordable and Clean Energy

Promotes efficient power monitoring and energy conservation.

### SDG 9 – Industry, Innovation and Infrastructure

Demonstrates the integration of Edge AI with embedded systems for intelligent monitoring.

## Team Members

* Fadiya Poozhikuth
* Fathima Safa
* Risha Febin
* Riza KP

## Guide

Dr. Ramesh Kumar P

## License

This project was developed as part of an academic mini-project under the Department of Applied Electronics and Instrumentation Engineering.

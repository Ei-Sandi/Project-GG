# GermGurdian 🛡️

**A Automated Home Sanitising System Built on MQTT**

![Project Status](https://img.shields.io/badge/Status-77%25_Complete-yellow)
![Language](https://img.shields.io/badge/Language-Python-blue)
![University](https://img.shields.io/badge/Institution-Coventry_University-red)

## 📖 Overview

**GermGurdian** is an IoT-based home safety and sanitisation solution designed to automate the cleaning of indoor environments. Built using Python and the MQTT protocol, the system relies on a network of publishers (sensors) and subscribers (controllers) to monitor environmental data such as air quality, temperature, and human presence.

The system ensures that sanitisation only occurs under safe and optimal conditions (e.g., when no motion is detected and air chemical levels are high).

## 🚀 Features

* **Motion Detection**: Monitors rooms for human presence to prevent sanitisation while occupied.
* **Air Quality Monitoring**: Tracks chemical concentrations to trigger cleaning cycles when air quality drops.
* **Environmental Sensing**: Monitors real-time temperature and weather data to optimize system performance.
* **Location Tracking**: Integrated location services to potentially trigger system states based on user proximity.
* **MQTT Architecture**: decoupled communication using the Publish-Subscribe model for real-time data exchange.

## 📂 Project Structure

The project is divided into Publisher (Sensor) and Subscriber (Controller/Monitor) scripts:

| Component | File Name | Description |
| :--- | :--- | :--- |
| **Motion** | `Motion_Sensor.py` | Publishes motion detection status. |
| | `Motion_Subscriber.py` | Listens for motion events to toggle safety locks. |
| **Air Quality** | `Air Chem Publisher` | Publishes simulated/real chemical concentration levels. |
| | `Air_Chemical_Concentraction Subscriber` | Triggers alerts or actions based on air quality. |
| **Temperature** | `Temprature_publisher.py` | Publishes current room temperature. |
| | `temperature_subscriber.py` | Monitors temperature data. |
| **Weather** | `Weather_Publisher.py` | Publishes external weather conditions. |
| | `Weather_Subscriber.py` | Receives weather updates. |
| **Location** | `location.py` | Handles location-based logic. 

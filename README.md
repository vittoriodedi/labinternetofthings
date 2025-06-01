# labinternetofthings

This repository contains my “Laboratorio Sistemi IOT” course final project.

## Overview

The final assignment for the course required students to collaboratively design a complete IoT system. Working in a team of three, we developed **PanApp**, a **real-time servo control dashboard** that connects hardware components via **micro\:bit** and visualizes data through a **web application** built with **Python** and **Flask**. The system integrates radio communication, serial data parsing, real-time visualization, and persistent logging.

## Contents

* 📁 **`PanApp/`** – Core folder containing the full web application:

  * `app.py` – Flask application entry point, manages routes and WebSocket updates.

  * `data_logger_script.py` – Handles serial input from the micro\:bit and logs it to the backend.

  * 📁 **`static/`** – Frontend assets:

    * 📁 `js/` – Contains `dashboard.js` for dynamic UI updates and WebSocket handling.
    * 📁 `css/` – Contains `dashboard.css` for dashboard styling.

  * 📁 **`template/`** – Contains `dashboard.html`, the main layout of the real-time dashboard.

* 📁 **`documenti/`** – Project documentation:

  * `Presentazione Laboratorio Sistemi IoT.pdf` – Slide deck used for the final presentation.
  * `Relazione Laboratorio Sistemi IoT.pdf` – Written report describing the project in detail.

## System Description

**PanApp** is composed of two interconnected micro\:bit devices and a web-based dashboard:

1. **Transmitter** – Reads values from 3 potentiometers and a button, then transmits them via radio.
2. **Receiver** – Interprets incoming data to control 3 servo motors and an LED.
3. **PC/Web App** – Receives serial data from the receiver micro\:bit, logs it, and displays it on a real-time dashboard via Flask and WebSockets.

Main features include:

* Radio-based wireless data transfer
* Real-time UI with live chart updates
* Persistent data logging for analysis
* CSV export functionality

## Purpose

This project demonstrates our ability to:

* Integrate **embedded systems** with **web technologies**
* Use **MicroPython** on micro\:bit for sensor and actuator control
* Manage real-time data via **serial communication** and **WebSockets**
* Build **interactive dashboards** with **Flask**, **JavaScript**, and **CSS**
* Collaborate effectively on a modular IoT architecture

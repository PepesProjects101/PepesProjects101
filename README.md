# Hey, I'm Grant! 👋

### Embedded Systems Developer · Maker · 3D Printing Enthusiast

I'm an 8th-grade maker and aspiring engineer from Connecticut. I enjoy designing and building custom electronics, embedded systems, microcontroller peripherals, and 3D-printed hardware from the ground up.

My projects combine firmware development, electronics, mechanical design, and software into functional physical devices. Whether it's building a custom handheld gaming console, engineering a multi-sensor measurement tool, or developing a PC control center, I enjoy taking an idea from a rough concept to a working prototype.

I'm particularly interested in the intersection of hardware and software: making physical devices interact with computers, designing custom interfaces, integrating sensors, and developing useful tools with inexpensive microcontrollers.

**My philosophy:** The best way to learn engineering is to build something, break it, figure out why, and make it better.

---

## 🛠️ Hardware & Technology

### Electronics & Embedded Systems
- **Microcontrollers:** ESP32, ESP32-S3, ESP32-C3 SuperMini, Arduino Mega 2560, Arduino Uno R4 Minima, RP2040-LoRa
- **Single-Board Computers:** Raspberry Pi 5 (2GB), Raspberry Pi Zero, Raspberry Pi Zero 2 W
- **Displays:** ST7735, ST7789V, ILI9341, SSD1306 OLED, Waveshare touchscreen displays
- **Sensors:** VL53L1X, MPU-6050, MLX90614, TCS34725, DS3231, NTC thermistors
- **Communication:** I²C, SPI, UART, Serial, Wi-Fi, Bluetooth
- **Frameworks:** Arduino, LVGL, PlatformIO

### 3D Printing & Mechanical Design
- **3D Printer:** Creality Ender 3 V2 Neo
- **Upgrades:** Sprite Pro Direct Drive, Dual Z-axis, MRiscoC Professional Firmware
- **Bed Leveling:** Unified Bed Leveling (UBL)
- **Printer Management:** OctoPrint
- **CAD & Modeling:** Blender
- **Fabrication:** Custom enclosures, functional mechanical components, prototyping, and hardware integration

### Programming & Software
- **C/C++:** Embedded firmware, microcontroller applications, and custom gaming systems
- **Python:** PC automation, serial communication, Windows control, and hardware backends
- **HTML/CSS:** Web interfaces and ESP32 web applications
- **Libraries & Tools:** Pycaw, PyAutoGUI, LVGL, Git, GitHub, Arduino IDE, VS Code, PlatformIO

---

# 🚀 Featured Projects

A selection of my electronics, embedded software, and hardware engineering projects.

## 01. Digital Shop Multitool
**ESP32-C3 SuperMini · C++ · I²C · SPI · 3D Printing**

A compact, handheld multifunction workshop tool designed to combine several measurement instruments into one custom-built device.

The project uses an ESP32-C3 SuperMini to integrate four different sensors alongside a color TFT display, all housed inside a custom 3D-printed enclosure.

**Hardware:**
- ESP32-C3 SuperMini
- ST7735 SPI TFT display
- VL53L1X laser time-of-flight distance sensor
- MPU-6050 6-axis accelerometer and gyroscope
- MLX90614 non-contact infrared thermometer
- TCS34725 RGB color sensor

**Features:**
- Laser-based distance measurement
- Non-contact infrared temperature readings
- Digital level and angle measurement
- RGB color detection
- Integrated sensor monitoring
- Custom handheld 3D-printed enclosure

The sensors communicate over a shared I²C bus, while the ST7735 display uses SPI.

The goal is to create an inexpensive, portable workshop instrument that combines multiple tools into one device.

[**View Repository →**](https://github.com/PepesProjects101/digital-shop-multitool)

## 02. MacroTimmy
**Arduino Mega 2560 · Python · Windows Automation · OLED**

A custom desktop macro pad and PC control center originally developed for Coolest Projects 2026.

MacroTimmy combines a physical control interface with a Python backend to provide direct control over Windows audio, monitor brightness, and frequently used applications.

**Hardware:**
- Arduino Mega 2560
- 0.96-inch SSD1306 I²C OLED
- 10-button macro matrix
- Analog joystick / rotary encoder
- USB serial communication

**Python Backend (`macrotimmy.py`):**

**Four-channel audio mixer**
- Master Windows volume
- Spotify audio
- Active game audio
- Microsoft Edge audio

Uses Pycaw to communicate with Windows audio sessions.

**Dual-monitor brightness control**
- Lenovo Generic Monitor
- Dell S2340M

Uses `screen_brightness_control` to adjust monitor brightness independently.

**Programmable macro controls**
- Arduino IDE
- UltiMaker Cura 5.8.1
- Steam
- Microsoft Edge

Uses PyAutoGUI for application launching and desktop automation.

**OLED interface:**
- Custom "MacroTimmy By Grant R." splash screen
- Serial connection status
- System dashboard
- Individual volume sliders
- Monitor brightness indicators

The Arduino and Python backend communicate through serial over COM3.

The goal is to create a dedicated physical interface for controlling a PC without constantly switching between desktop applications and system settings.

[**View Repository →**](https://github.com/PepesProjects101/macrotimmy)

## 03. SmarterWatch
**ESP32-S3 · C++ · LVGL · Touchscreen · 3D Printing**

A custom programmable smartwatch built around the Waveshare ESP32-S3 Touch LCD 1.28-inch development board.

The project combines a round touchscreen, embedded firmware, custom graphical interfaces, and a purpose-built 3D-printed wearable enclosure.

**Hardware:**
- Waveshare ESP32-S3 Touch LCD 1.28"
- 240 × 240 round IPS display
- Capacitive touchscreen
- Onboard IMU
- Integrated battery management

**Software & Design:**
- C++ Arduino firmware
- LVGL graphical interface
- Custom watch faces
- Utility applications
- Touch-based navigation
- Custom 3D-printed watch body and strap mounts

The objective is to develop a fully customizable smartwatch rather than relying on an off-the-shelf wearable operating system.

[**View Repository →**](https://github.com/PepesProjects101/smarterwatch)

## 04. MacinClock
**ESP32 · ILI9341 · DS3231 RTC · C++ · 3D Printing**

A miniature vintage Macintosh-inspired desktop clock that recreates the look and feel of classic Macintosh computers.

The device uses an ESP32 to render a retro computer interface on a color TFT display, with a dedicated real-time clock module for accurate timekeeping.

**Hardware:**
- ESP32 microcontroller
- ILI9341 SPI TFT display
- DS3231 real-time clock module
- Custom 3D-printed Macintosh enclosure

**Features:**
- Macintosh-inspired display interface
- Dedicated real-time clock
- Battery-backed timekeeping
- Custom retro desktop enclosure
- Embedded graphics and display control

The project combines retro computing aesthetics with modern embedded electronics.

[**View Repository →**](https://github.com/PepesProjects101/macinclock)

## 05. Web-Controlled Filament Dryer
**ESP32 · Wi-Fi · Web Server · Temperature Monitoring**

A custom Wi-Fi-enabled 3D printing filament dryer built by repurposing spare components from a Creality Ender 3 V2 Neo.

Rather than purchasing an entirely new drying system, this project uses existing printer hardware and an ESP32 to create a remotely controllable drying chamber.

**Hardware:**
- ESP32 DevKit V1
- NTC thermistor
- Tolako 5V relay module
- Repurposed Ender 3 V2 Neo heatsink
- Cooling fan

**Software & Features:**
- Built-in ESP32 web server
- Live chamber temperature monitoring
- Wi-Fi connectivity
- Remote drying-cycle toggling
- Relay-controlled heating system

The project explores practical IoT applications and hardware reuse within the 3D printing ecosystem.

[**View Repository →**](https://github.com/PepesProjects101/esp32-filament-dryer)

## 06. Timmy 2.0
**ESP32 · C++ · ST7789V · Custom Gaming Firmware**

A standalone handheld gaming device designed and programmed from scratch.

Timmy 2.0 runs approximately 3,200 lines of custom C++ firmware and features a custom launcher, multiple original game implementations, and a procedural neon-themed startup screen.

**Hardware:**
- ESP32 DevKit V1
- Waveshare 2-inch ST7789V TFT display
- 240 × 320 resolution, configured in landscape
- MicroSD card reader
- Passive buzzer
- Tactile button matrix

**Custom Firmware:**
- Custom launcher and menu system
- Display rendering and input handling
- Procedural neon splash screen
- Audio feedback through a passive buzzer
- Game selection and navigation

**Five playable games:**
1. Tetris
2. Snake
3. Flappy Bird
4. AI Tic-Tac-Toe
5. Retro Racing

The project demonstrates how a relatively inexpensive ESP32 can be used to create a complete standalone gaming system with custom firmware and multiple playable applications.

[**View Repository →**](https://github.com/PepesProjects101/timmy-2)

## 07. PocketPi Series
**Raspberry Pi Zero · Python · RetroPie · 3D Printing**

A collection of portable retro gaming handheld projects based on the PiGRRL Zero concept.

These builds explore compact Raspberry Pi systems, portable gaming hardware, and custom enclosures.

**Hardware & Software:**
- Raspberry Pi Zero / Zero 2 W
- RetroPie
- Python
- GPIO-connected gamepad controls
- Custom 3D-printed enclosures

The focus is on combining single-board computers, physical controls, and compact mechanical designs into portable gaming systems.

[**View Repository →**](https://github.com/PepesProjects101/pocketpi)

## 08. Batocera "Baby North"
**Raspberry Pi 5 · Batocera Linux · Retro Emulation**

A compact desktop retro gaming console built around the Raspberry Pi 5.

The system uses Batocera Linux to provide a dedicated emulation environment inside a custom-designed chassis.

**Hardware & Software:**
- Raspberry Pi 5 (2GB)
- Batocera Linux
- Custom-designed thermal chassis
- Compact desktop form factor
- Retro gaming and emulation environment

The project focuses on creating a small, dedicated retro gaming system with an emphasis on compact hardware integration and thermal design.

[**View Repository →**](https://github.com/PepesProjects101/baby-north-console)

---

## 🔬 What I'm Exploring

I'm constantly experimenting with new technologies and looking for ways to make my projects more capable.

Some of my main interests include:

- **Embedded Systems:** More advanced ESP32 applications, sensor integration, and custom firmware.
- **Custom PC Peripherals:** Physical interfaces for controlling computers, audio, lighting, and applications.
- **IoT Development:** Wi-Fi-connected devices, remote monitoring, and browser-based hardware control.
- **Wearable Electronics:** Custom smartwatches and compact touchscreen devices.
- **3D Printing:** Functional enclosures, mechanical assemblies, and rapid prototyping.
- **Game Development:** Small-scale games and custom gaming hardware.
- **Hardware & Software Integration:** Connecting microcontrollers to desktop applications and operating systems.

## ⚙️ How I Build

I enjoy managing the entire development process, from the first idea to the finished physical device.

My typical workflow:

1. **Concept:** Identify a problem or come up with an idea for a useful device.
2. **Research:** Explore components, sensors, microcontrollers, and possible implementations.
3. **Electronics:** Prototype circuits, configure pinouts, and integrate hardware.
4. **Firmware:** Develop the embedded software and communication systems.
5. **Mechanical Design:** Model custom enclosures and components in Blender.
6. **Fabrication:** 3D print and assemble the physical hardware.
7. **Testing:** Debug, troubleshoot, improve, and refine the finished project.

I prefer building things that actually work in the real world, not just software simulations or theoretical designs.

---

## 📫 Find Me

- **GitHub:** [@PepesProjects101](https://github.com/PepesProjects101)
- **Location:** Connecticut, USA

---

*Always experimenting. Always building something new.* ⚡

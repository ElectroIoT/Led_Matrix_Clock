# Arduino Matrix Clock V1.5

A compact and attractive real-time clock (RTC) based on the Arduino Mini and a 4x MAX7219 LED Matrix display. Designed with a custom PCB and powered via TP4056 Li-ion charging module, this project makes a beautiful desk clock with a 3D printed case.

## 🔧 Features

- 🕒 Real-time clock using DS1307+ RTC
- 💡 Bright and crisp 32x8 LED Matrix display (MAX7219)
- 🔋 Battery-powered with TP4056 charging circuit
- 🔘 Multiple buttons for settings
- 🧠 Based on Arduino Mini (3.3V or 5V)
- 📦 Custom 3D printed case

## 🖼️ Demo

![Clock Demo](Image/clock.JPG)

## 📦 Hardware Components

| Component          | Quantity | Notes                        |
|--------------------|----------|------------------------------|
| Arduino Pro Mini    | 1        | 3.3V or 5V                   |
| MAX7219 LED Matrix  | 4        | Dot matrix, 8x8              |
| DS1307 RTC Module   | 1        | With 32.768KHz crystal       |
| TP4056 Module       | 1        | For charging 3.7V Li-ion     |
| Push Buttons        | 3        | Time set / mode / reset      |
| 3D Printed Case     | 1        | STL shared below             |
| Custom PCB          | 1        | Designed in EasyEDA          |

## 🖥️ PCB Design

- Designed using **EasyEDA**
- Version: V1.5
- Includes:
  - Slots for Arduino Mini, DS1307, TP4056
  - Ports for 4x Matrix displays
  - Button pads (KEY1, KEY2, KEY3)
  - Power input (BAT / DC 5V)
  - Download PCB: 

### PCB Front:
![PCB Front](Image/Arduino_PCB_Front.JPG)

### PCB Back:
![PCB Back](Image/Arduino_PCB_back.JPG)

## 🧾 Circuit Diagram

Refer to the PDF for the full schematic:
- [Arduino Matrix MAX7219 Clock.pdf](Diagram/Arduino_Matrix_MAX7219_Clock/Arduino_Matrix_MAX7219_Clock.pdf)

## 💻 Arduino Code

You can find the complete source code here:

👉 [`Led_Matrix_Clock.ino`](Code/Arduino/Led_Matrix_Clock.ino)

### Features in Code:
- Displays current time in HH:MM:SS
- Allows setting time using buttons
- RTC synchronization
- LED scrolling effect (optional)

### 📚 Required Libraries

Make sure you install these libraries before compiling:

| Library         | Description                          | Download Link |
|----------------|--------------------------------------|---------------|
| **LedControl** | Control MAX7219 LED Matrix           | [Arduino Library](https://www.arduinolibraries.info/libraries/led-control) |
| **FontLEDClock** | Custom fonts for matrix display      | [GitHub](https://github.com/javastraat/arduino/tree/master/libraries/FontLEDClock) *(Manual install)* |
| **Wire**        | I2C communication (built-in)         | Built-in |
| **RTClib**      | DS1307 RTC timekeeping               | [Arduino Library](https://www.arduinolibraries.info/libraries/rt-clib) |
| **Button**      | Simplified button control            | [Arduino Library](https://www.arduinolibraries.info/libraries/button) |

You can install these via the Arduino Library Manager or manually via the provided links.

## 🖨️ 3D Case

- Designed for a 4x MAX7219 display
- Button holes and charging port access included
- You can customize the name on top

## 🔌 Powering the Clock

- Connect a 3.7V Li-ion battery to TP4056
- Or power directly via 5V DC port
- TP4056 manages battery charging safely

## 📷 Build Preview

![Final Clock](Image/clock.JPG)


Stay tuned on our channel:
- [YouTube - ElectroIoT](https://www.youtube.com/ElectroIoT)

## 🌐 More Projects

- Website: [https://electroiot.in](https://electroiot.in)
- GitHub: [ElectroIoT](https://github.com/ElectroIoT)

---

## 🙏 Special Thanks

A big thank you to the following platforms for their amazing tools and support in designing this open-source hardware project:

<p align="center">
  <img src="Image/EasyEDA.png" alt="EasyEDA Logo" width="100"/>&nbsp;&nbsp;&nbsp;&nbsp;
  <img src="Image/OSHWLab.png" alt="OSHWLab Logo" width="100"/>
</p>

- **[EasyEDA](https://easyeda.com/)** – for their powerful PCB design tools  
- **[OSHWLab](https://oshwlab.com/)** – for hosting open-source hardware projects

Their platforms made this project possible and easy to share with the maker community ❤️

## 📬 License

Open Source Hardware — OSHWA Certified

---

Happy Making! 💡

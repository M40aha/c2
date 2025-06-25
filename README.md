# 🔌 Neat Stantia-Hillar – Arduino LED Sequence Project

💡 A simple yet elegant Arduino-based circuit that controls **3 LEDs** in sequence using **digital pins** and basic components on a breadboard.

![Project Preview](Neat%20Stantia-Hillar.png)

---

## 🧠 Project Description

This project demonstrates how to connect and control multiple LEDs using an **Arduino Uno** and a **breadboard**. It’s ideal for beginners looking to practice digital output, circuit wiring, and sequential LED logic.

---

## 📦 Components Used

- 🟦 Arduino Uno
- 🔴 3x LEDs (any color)
- 🟡 3x 220Ω resistors
- 🧠 Breadboard
- 🔌 Jumper wires
- 🖥️ Arduino IDE (for uploading code)

---

## ⚙️ Circuit Connections

| Arduino Pin | Connection            |
|-------------|------------------------|
| GND         | Breadboard ground rail |
| Pin 5       | LED 1 (via resistor)   |
| Pin 6       | LED 2 (via resistor)   |
| Pin 7       | LED 3 (via resistor)   |

Each LED’s **anode (+)** connects to the digital pin via a resistor, and the **cathode (-)** goes to ground.

---

## 🧾 Sample Arduino Code

```cpp
int led1 = 5;
int led2 = 6;
int led3 = 7;

void setup() {
  pinMode(led1, OUTPUT);
  pinMode(led2, OUTPUT);
  pinMode(led3, OUTPUT);
}

void loop() {
  digitalWrite(led1, HIGH);
  delay(500);
  digitalWrite(led1, LOW);

  digitalWrite(led2, HIGH);
  delay(500);
  digitalWrite(led2, LOW);

  digitalWrite(led3, HIGH);
  delay(500);
  digitalWrite(led3, LOW);
}

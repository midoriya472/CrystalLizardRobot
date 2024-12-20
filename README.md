# Crystal Lizard Robot Prototype

## **Overview**
The Crystal Lizard Robot is a functional prototype inspired by the popular game *Dark Souls*. It is designed to showcase autonomous movement, obstacle detection, and aesthetic appeal. This project is built using Arduino components and custom-designed mechanical parts.

---

## **Features**
- Obstacle avoidance using an ultrasonic sensor.
- Reactive LED lighting for visual feedback.
- Programmable logic for autonomous decision-making.
- Compact and durable design.

---

## **Hardware Components**
1. **Microcontroller:** Arduino Uno
2. **Sensors:** Ultrasonic sensor for obstacle detection
3. **Power Supply:** 9V Battery
4. **LEDs:** Yellow/Red/Blue for visual effects
5. **Chassis:** Custom 3D-printed crystal-like design

---

## **Software**
- **Programming Language:** Arduino IDE
- **Libraries Used:** 
  - `Servo.h` for motor control
  - `NewPing.h` for ultrasonic sensor integration
- **Code Overview:**
  The program uses the ultrasonic sensor to detect obstacles within 10 cm and triggers a motor response to "run away" in the opposite direction.

---

## **Getting Started**
1. **Hardware Setup:**
   - Assemble the components as per the schematic diagram in the documentation.
   - Connect the ultrasonic sensor to the Arduino using jumper wires.
   - Install the 9V battery pack for power.
   
   Software Setup:
   - Download and install the Arduino IDE from [Arduino's official website](https://www.arduino.cc/en/software).
   - Clone this repository using Git:
     ```
     git clone https://github.com/YourUsername/CrystalLizardRobot.git
     ```
   - Open the `CrystalLizardRobot.ino` file in the Arduino IDE.

3. Uploading the Code:
   - Connect the Arduino Uno to your PC via USB.
   - Select the correct COM port in the Arduino IDE.
   - Click **Upload** to load the code onto the microcontroller.

---

## Code Highlights
```cpp
// LED Blinking Function
void blinkLED(int pin, int duration) {
  digitalWrite(pin, HIGH);
  delay(duration);
  digitalWrite(pin, LOW);
  delay(duration);
}

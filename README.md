# Interfacing-Seven-Segment-Display-with-Arduino-Mega
# Seven Segment Counter using Arduino

This project demonstrates how to use an Arduino to display numbers from 0 to 9 (and back) on a **7-segment display**. The sequence starts when a **push button** is released (using `INPUT_PULLUP` logic). An LED is also turned on during the counting process.

---

## Features

- Counts from 0 to 9 and then reverses (9 to 0)
- Displays digits on a 7-segment display
- Uses a push button to control the counting
- LED indicator turns ON while counting

---

## Components Required

- Arduino Uno (or compatible board)
- 1 × 7-Segment Display (Common Cathode)
- 1 × Push Button
- 1 × LED
- 8 × 220Ω resistors (for segments + LED)
- Jumper wires and breadboard

---

##  Circuit Connections

| Segment | Arduino Pin |
|---------|-------------|
| A       | 12          |
| B       | 11          |
| C       | 10          |
| D       | 9           |
| E       | 8           |
| F       | 7           |
| G       | 6           |
| Button  | 4 (with INPUT_PULLUP) |
| LED     | 3           |

---

## How It Works

- On power-up, the LED turns ON.
- When the **button is not pressed** (logic HIGH due to pull-up), the display starts counting from 0 to 9 and back.
- The digits are displayed on a 7-segment display with 1-second intervals.

---

## 🧾 Code Overview

- `setup()`: Sets pin modes for segments, button, and LED.
- `loop()`: Continuously checks the button state and triggers the counting logic.
- `print_sev_seg()`: A custom function to display a digit on the 7-segment display.

---

## How to Upload

1. Open Arduino IDE
2. Select the correct board and COM port
3. Copy the code from `seven_segment_counter.ino`
4. Upload the code to your Arduino

---

## License

This project is open-source under the [MIT License](LICENSE).

---

## Author

**Your Name Here**  
Feel free to fork, contribute, or raise issues if you'd like to enhance the project!

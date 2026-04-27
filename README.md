# STM32L476 Nucleo board.

# 🏁 Hot Wheels Speed Tracker (STM32)

A real-time embedded system built using an STM32 Nucleo board to measure the speed and timing of a Hot Wheels car on a track using IR sensors.

---

## 🚀 Features

- ⏱ Measures total race time
- 📏 Calculates segment speeds:
  - Start → Midpoint
  - Midpoint → Finish
- 🚦 Drag-race style countdown lights (Red → Yellow → Green)
- 🖥 OLED display output (SSD1306 128x64)
- 🔘 Button-controlled start and reset
- ⚡ Interrupt-based sensor detection for high accuracy
- 🧠 State machine-based system design

---

## 🧰 Hardware Used

- STM32 Nucleo board
- SSD1306 OLED display (I2C, 128x64)
- 3x IR break-beam sensors
- Push button (PC13)
- 3 LEDs (Red, Yellow, Green)
- Hot Wheels track 😄

---

## ⚙️ How It Works

1. Press button to start countdown
2. LEDs sequence:
   - 🔴 Red
   - 🔴🟡 Red + Yellow
   - 🟢 Green → GO
3. Car starts moving
4. Sensors detect:
   - Start
   - Midpoint
   - Finish
5. System calculates:
   - Total time
   - Segment speeds
6. Results displayed on OLED

Uses GitHub SSD1306 library by Afiskon (https://github.com/afiskon/stm32-ssd1306)

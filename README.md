# 7-Segment Display Counter 🎉

This project demonstrates how to use a 7-segment display with an Arduino to increment a number every time a button is pressed. Each time the button is pressed, the display shows the next number in sequence from 0 to 9. After 9, the number resets back to 0 🔄.

## 🛠️ Components Used

- **Arduino Board** (e.g., Arduino Uno)
- **7-Segment Display** (Common Cathode or Common Anode depending on your setup)
- **Button** (Push button switch)
- **Resistors** for button and display connections
- **Wires and Breadboard** for prototyping

## 📸 Circuit Diagram

- **Button Pin** is connected to pin 2.
- **7-Segment Display** pins are connected to the following Arduino pins:
  - Segment A: Pin 3
  - Segment B: Pin 4
  - Segment C: Pin 5
  - Segment D: Pin 6
  - Segment E: Pin 6
  - Segment F: Pin 9
  - Segment G: Pin 10

Make sure to properly connect the 7-segment display based on its type (Common Cathode or Common Anode). The common pin of the display should be connected to ground or VCC accordingly ⚡.

## 💻 Code Explanation

- **Button Press Detection:** The button is connected to pin 2, and the code checks its state. When pressed, it increments the number on the display.
- **7-Segment Display:** The display is controlled by sending HIGH or LOW signals to each of the seven segments. The segment configuration for each digit (0-9) is predefined in the `digits` array 📱.
- **Debouncing:** A small delay (`200 ms`) after each button press is used to debounce the switch and prevent multiple increments from mechanical bounce of the button ⏳.

## 🧑‍💻 How It Works

1. Initially, the display shows the digit 0.
2. When the button is pressed, the displayed digit increments by 1 (cycling through 0 to 9) 🔟.
3. The display updates to show the current digit, and the cycle repeats 🔄.

## 📋 Requirements

- Arduino IDE to upload the code to your Arduino board
- Arduino-compatible hardware (e.g., Arduino Uno)
- 7-segment display and button connected as shown in the circuit diagram

## 🚀 Installation

1. Clone this repository to your local machine 💻.
2. Open the `.ino` file in the Arduino IDE.
3. Connect your Arduino to your computer and select the correct board and port in the Arduino IDE.
4. Upload the code to the Arduino 🚀.
5. Connect the 7-segment display and button as per the circuit diagram 🔌.
6. Press the button to increment the number on the display and enjoy the show! 🎉

## 📜 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 🙌 Acknowledgements

- Thanks to the awesome Arduino community for inspiration and guidance on working with 7-segment displays and buttons! 💡

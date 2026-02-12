# 📸 Memento Flex

**The Student "Flexible" Camera** — Memento Flex is a versatile, AI-powered smart camera built on [Adafruit MEMENTO](https://www.adafruit.com/product/5800).
 Designed for students, creators etc, it "flexes" between a standard digital camera, a scientific observation tool, and an AI-vision assistant.

## ✨ Features

* **🧠 AI-Powered Insights:** Connects to OpenRouter to provide real-time image descriptions.
* **⏳ Smart Time-Lapse:** Includes a "Low Power" mode that dims the screen to save battery during long observations.
* **🎞️ Animation Suite:** Support for both looping GIFs and Onion-skinning Stop Motion.
* **🌐 Automated Sync:** Fetches local time automatically via NTP over Wi-Fi.
* **🛠️ Custom Text UI:** Result text is intelligently wrapped and scaled to be readable on the 240x240 display.

---

## 🚀 Setup Instructions

### 1. Requirements
* **Hardware:** Adafruit MEMENTO Camera board & a microSD card.
* **Firmware:** [CircuitPython 10.x](https://circuitpython.org/board/adafruit_memento_camera/)
* **API Key:** A free or paid key from [OpenRouter.ai](https://openrouter.ai/).

### 2. Configuration
Create a `settings.toml` file on your `CIRCUITPY` drive. **Do not share this file publicly!**

```toml
# Wi-Fi Settings
CIRCUITPY_WIFI_SSID = "Your_Network_Name"
CIRCUITPY_WIFI_PASSWORD = "Your_Password"

# AI & Time Settings
OPENROUTER_API_KEY = "your_key_here"
TZ = "Your_timezone"
UTC_OFFSET = Your_Offset
AI_PROMPT = "Describe this image in 5-10 simple words."
```
## 🚀 Installation

1. **Upload Code:** Copy the `code.py` file from this repository onto your MEMENTO's `CIRCUITPY` drive.
2. **Install Libraries:** Ensure your `lib` folder on the MEMENTO contains the necessary Adafruit libraries. 
   > **Note:** You can find these in the [Adafruit CircuitPython Library Bundle](https://circuitpython.org/libraries).
3. **Configure:** Make sure your `settings.toml` is set up with your Wi-Fi and API credentials.
4. **Restart:** Press the **Reset** button on the top of your MEMENTO to start the **Flex** software.

## 🕹️ Controls

| Button | Action |
| :--- | :--- |
| **Shutter (Click)** | Snap Photo / Record GIF / Capture Frame |
| **Shutter (Long)** | Trigger Autofocus |
| **OK Button** | **JPEG Mode:** Analyze with AI <br> **LAPS Mode:** Start/Stop Time-lapse |
| **D-Pad** | Navigate Settings (Resolution, Effects, Mode, etc.) |
| **Select Button** | Change Sub-modes (e.g., High/Low Power in LAPS) |

---

## 📜 Credits

* **Original Authors:** Jeff Epler& Limor Fried ([Adafruit Industries](https://www.adafruit.com/)).
* **Modifications & "Flex" Features:** [Gautham Chenoth Praveen](https://github.com/Gautham-8066).

---


# Real-Time EEG System using AD8232 + ADS1115 + ESP32 and Python

Team Electra — GSSS E-Minds Hackathon 2.0  
A complete low-cost, real-time EEG acquisition and visualization system.

## 🚀 Features
- Real-time EEG capture @ 500 Hz
- AD8232 biopotential sensor for EEG
- ADS1115 16-bit ADC for accurate microvolt readings
- ESP32 for wireless data streaming (Serial/WiFi)
- Python live plotting with bandpass filtering (1–40 Hz)
- Full-stack dashboard (frontend + backend included)

---

## 🔌 Hardware Connections

### Electrode Leads (via 3.5mm TRS Jack)
| Wire Color | AD8232 Pin | Placement |
|-----------|-------------|-----------|
| Yellow    | LA (IN+)    | Fp1 |
| Green     | RA (IN-)    | Fp2 |
| Red       | RL (RLD)    | Ear / Mastoid |

### AD8232 → ADS1115
- OUTPUT → A0  
- 3.3V → ESP32 3.3V  
- GND → ESP32 GND  

### ADS1115 → ESP32 (I²C)
- VCC → 3.3V  
- GND → GND  
- SDA → GPIO 21  
- SCL → GPIO 22  
- ADDR → GND  

---

## 📟 ESP32 Firmware
Firmware located in:

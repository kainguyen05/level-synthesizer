# Level Synthesiser (Tilt → Tone)

Converts board tilt into sound pitch using an **ADXL327** accelerometer → **OP27** (DC-offset removal + gain) → **AD654** voltage→frequency tone generator → **ZN3310A** speaker driver.  
Produces ~24–1100 Hz mapped to tilt.

---

## Artifacts
- [Project Report (PDF)](docs/Level-Synthesiser-Report.pdf)
- Scope screenshots: [Minimum Frequency](docs/Minimum-Frequency.jpg) · [Maximum Frequency](docs/Maximum-Frequency.jpg)
- **Demo Videos (hosted on GitHub Releases):**
  - [Accelerometer X-Direction](https://github.com/kainguyen05/level-synthesizer/releases/download/v2025.01.17/Accelerometer_Test_xdirection.mp4)
  - [Accelerometer Y-Direction](https://github.com/kainguyen05/level-synthesizer/releases/download/v2025.01.17/Accelerometer_Test_ydirection.mp4)
  - [Accelerometer Z-Direction](https://github.com/kainguyen05/level-synthesizer/releases/download/v2025.01.17/Accelerometer_Test_zdirection.mp4)
  - [Buffer + DC Offset Removal](https://github.com/kainguyen05/level-synthesizer/releases/download/v2025.01.17/Buffer_DC_Offset_Removal_Test.mp4)
  - [Tone Generator](https://github.com/kainguyen05/level-synthesizer/releases/download/v2025.01.17/Test_Audio_Frequency_Tone_Generator.mp4)
  - [Audio Driver Amplifier](https://github.com/kainguyen05/level-synthesizer/releases/download/v2025.01.17/Test_Audio_Driver_Amplifier.mp4)
  - [Complete Circuit Demo](https://github.com/kainguyen05/level-synthesizer/releases/download/v2025.01.17/Complete_Circuit_Test.mp4)

---

## Block Diagram
`ADXL327 → OP27 (DC-offset removal & gain) → AD654 (V/F) → ZN3310A driver → Speaker`

---

## Key Results
- Frequency range: **≈ 24 – 1100 Hz**  
- Behavior: Frequency ↑ with positive tilt, ↓ with negative tilt  
- Supply: ±5 V rails; 3.3 V LDO for sensor and analog stages

---

## License
Code & documentation: **MIT**  
Media (photos & videos): © 2025 Canh Thai Nguyen

# Level Synthesiser (Tilt → Tone)

Converts board tilt into sound pitch using an **ADXL327** accelerometer → **OP27** (DC-offset removal + gain) → **AD654** voltage→frequency tone generator → **ZN3310A** speaker driver.  
Produces ~24–1100 Hz mapped to tilt.

---

## Artifacts
- [Project Report (PDF)](docs/Level-Synthesiser-Report.pdf)
- Scope screenshots: [Minimum Frequency](docs/Minimum-Frequency.jpg) · [Maximum Frequency](docs/Maximum-Frequency.jpg)
- Demo videos hosted on GitHub Releases *(v1.0.0 example)*:
  - 🎥 [Accelerometer X-Direction](https://github.com/kainguyen05/level-synthesiser/releases/download/v1.0.0/Accelerometer_Test_xdirection.mp4)
  - 🎥 [Accelerometer Y-Direction](https://github.com/kainguyen05/level-synthesiser/releases/download/v1.0.0/Accelerometer_Test_ydirection.mp4)
  - 🎥 [Buffer + DC Offset Removal](https://github.com/kainguyen05/level-synthesiser/releases/download/v1.0.0/Buffer_DC_Offset_Removal_Test.mp4)
  - 🎥 [Tone Generator](https://github.com/kainguyen05/level-synthesiser/releases/download/v1.0.0/Test_Audio_Frequency_Tone_Generator.mp4)
  - 🎥 [Audio Driver Amplifier](https://github.com/kainguyen05/level-synthesiser/releases/download/v1.0.0/Test_Audio_Driver_Amplifier.mp4)
  - 🎥 [Complete Circuit Demo](https://github.com/kainguyen05/level-synthesiser/releases/download/v1.0.0/Complete_Circuit_Test.mp4)

> Replace **v1.0.0** with your actual release tag once published.

---

## Block Diagram
`ADXL327 → Diff Amp (OP27) → AD654 (V/F) → Driver (ZN3310A) → Speaker`

---

## Key Results
- Frequency range: **≈ 24 – 1100 Hz**
- Behavior: Frequency ↑ with positive tilt, ↓ with negative tilt  
- Supply: ±5 V rails; 3.3 V LDO for sensor and analog stages

---

## License
Code & Documentation: **MIT**  
Media (photos & videos): © 2025 Canh Thai Nguyen


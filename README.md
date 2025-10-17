# Level Synthesiser (Tilt → Tone)

Converts board tilt into sound pitch using an **ADXL327** accelerometer → **OP27** (DC-offset removal + gain) → **AD654** voltage→frequency tone generator → **ZN3310A** speaker driver. Produces ~24–1100 Hz mapped to tilt.

**Artifacts**
- [Report (PDF)](docs/Level-Synthesiser-Report.pdf)
- Scope screenshots: [Min freq](docs/Minimum-Frequency.jpg) · [Max freq](docs/Maximum-Frequency.jpg)
- Demo videos (compressed):  
  [Accelerometer X](media/Accelerometer_Test_xdirection.mp4) ·
  [Accelerometer Y](media/Accelerometer_Test_ydirection.mp4) ·
  [Buffer + DC Offset](media/Buffer%20+%20DC%20offset%20removal%20Test.mp4) ·
  [Tone Generator](media/Test_Audio_Frequency_Tone_Generator.mp4) ·
  [Audio Driver](media/Test_Audio_Driver_Amplifier.mp4) ·
  [Full System](media/Complete_Circuit_Test.mp4)

## Block Diagram
ADXL327 → Diff Amp (offset removal & gain) → AD654 (V/F) → Driver → Speaker

## Key Results
- Frequency range: **≈ 24–1100 Hz**
- Behavior: Frequency ↑ with positive tilt, ↓ with negative tilt
- Supply: ±5 V rails; 3.3 V LDO for sensor/analog stages

## License
Code/docs: **MIT** • © 2025 Canh Thai Nguyen

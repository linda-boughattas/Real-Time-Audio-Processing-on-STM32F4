# Real-Time Audio Processing on STM32F4

## Overview
This project implements **real-time audio signal processing** on the STM32F4 Discovery Board. It includes:
- Capturing audio via the **PDM microphone**.
- Processing audio using **PDM to PCM conversion**.
- Playback via the **CS43L22 Audio Codec** on headphones or integrated speakers.

---

## Project Requirements
- **Hardware**:
  - STM32F4 Discovery Board.
  - USB cable for power and programming.
- **Software**:
  - STM32CubeMX.
  - MDK-ARM (Keil µVision).

---

## Resources & References
Below are the resources that helped in building this project, organized by type:

### Video Tutorials
1. [I2S Audio Codec - CS43L22](https://www.youtube.com/watch?v=QIPQOnVablY)
2. [PDM Microphones - Audio DSP On STM32 (16 Bit / 48 kHz)](https://www.youtube.com/watch?v=JuXKeyFraF4)
3. [STM32 Microphone Audio Acquisition](https://www.youtube.com/watch?v=_YQSJJQUp-g&list=PLwqrqfRKpbeIxgnKq1_hTCULCaL7LBHmN&ab_channel=STMicroelectronics)

### Documentation & Datasheets
1. [MB997: Schematic Prints for STM32F4Discovery](https://www.st.com/resource/en/schematic_pack/mb997-f407vgt6-b02_schematic.pdf)
2. [CS43L22 Audio Codec Datasheet](https://datasheet.octopart.com/CS43L22-CNZ-Cirrus-Logic-datasheet-5397077.pdf)
3. [AN5027: Interfacing PDM Digital Microphones using STM32 MCUs and MPUs](http://bit.ly/AN5027-AppNote)
4. [UM2372: STM32Cube PDM2PCM Software Library](https://github.com/user-attachments/files/18081861/um2372-stm32cube-pdm2pcm-software-library-for-the-stm32f4f7h7series-stmicroelectronics.pdf)
5. [STM32 PDM Mic Documentation (stm32_pdm_mic_docu.pdf)](https://github.com/YetAnotherElectronicsChannel/STM32_PDM_Microphone/blob/master/stm32_pdm_mic_docu.pdf)

### Repositories
1. [STM32 Tutorials - I2S Audio Codec (CS43L22)](https://github.com/MYaqoobEmbedded/STM32-Tutorials/tree/master/Tutorial%2028%20-%20I2S%20Audio%20Codec%20-%20CS43L22)
2. [PDM Microphone on STM32](https://github.com/YetAnotherElectronicsChannel/STM32_PDM_Microphone/tree/master)

---

## How It Works
1. **Audio Acquisition**:
   - PDM microphone captures audio.
   - DMA transfers data to memory.
2. **PDM to PCM Conversion**:
   - The `PDM2PCM` library converts PDM data into PCM format.
3. **Audio Playback**:
   - The CS43L22 codec handles playback over I2S.

---

## License
This project is licensed under the MIT License.


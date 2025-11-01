# Home Assistant Integration for Logitech Z906 (via nforay/Z906Remote)

This project provides a **complete Home Assistant setup** to control and monitor the **Logitech Z906** speakers using the [nforay/Z906Remote](https://github.com/nforay/Z906Remote) API.

It includes:
- ✅ REST commands and sensors for two-way communication with Z906Remote  
- 🎚️ Template entities for cleaner integration in Home Assistant  
- ⚙️ Automations to sync power, input, and volume  
- 🖥️ A ready-to-use **Lovelace dashboard** (custom control panel)  

---

## 🧠 Overview

This setup allows you to **fully integrate the Logitech Z906** into your smart home ecosystem — controlling it from the Home Assistant dashboard, automating behavior, and monitoring its current state (input, volume, power, etc.).

The integration relies on the [Z906Remote API by nforay](https://github.com/nforay/Z906Remote), which exposes the Logitech Z906 over your network through a simple REST interface.

---

<img width="1612" height="706" alt="immagine" src="https://github.com/user-attachments/assets/c5ba4899-1a58-4c59-a60d-b6510d201c18" />



## 🧩 Features

- Power ON/OFF directly from Home Assistant  
- Change input source (Optical, Coaxial, Direct, etc.)  
- Adjust each channel's volume  
- Display current input and volume level  
- Button for input & effects that lights up according the input/effect selected (you can set a specif effects for each input)
- Sync volume with other devices (TV, media players, etc.)  
  

---
## ⚙️ Requirements

1. A working installation of [nforay/Z906Remote](https://github.com/nforay/Z906Remote)
   - Make sure the API is reachable from your Home Assistant instance 
2. Basic knowledge of YAML configuration
3. (Optional) Custom compoenents for the "UI" if you want replicate exactly how i did it:
  - [slider-entity-row](https://github.com/thomasloven/lovelace-slider-entity-row)
  - [multiple-entity-row](https://github.com/benct/lovelace-multiple-entity-row)
  - [button-card](https://github.com/custom-cards/button-card)

## 🚀 Installation

1. Copy the content of config.yaml and paste it in the right places of your 'config.yaml' file 
2. Adjust the IP of your Z906Remote instance inside the `config.yaml` file
3. Create thre required automation copying from mine. 
4. Reload your configuration or restart Home Assistant
5. (Optional) Import the included Lovelace dashboard (`z906-dashboard.yaml`)

That’s it! Your Z906 should now appear as controllable entities within Home Assistant.

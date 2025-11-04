# WSPR‑zero Raspberry Pi–Compliant WSPR HAT

A low‑cost, permanent WSPR transmit HAT created for and used by the **[WSPR‑zero](https://github.com/zinkwazi/wspr-zero)** project. Designed to be Raspberry Pi HAT–compliant and simple to build, it provides band‑specific low‑pass filtering for clean WSPR transmissions at very low power.

> Looking for the full software stack and images? Visit **[wspr-zero.com](https://wspr-zero.com)** and **[WSPR‑zero on GitHub](https://github.com/zinkwazi/wspr-zero)**.

---

## Highlights

- Raspberry Pi HAT–compliant footprint for Pi Zero, Pi 3, 4 and 5
- Low‑pass filter per band to suppress spurious harmonics
- **Pin‑compatible with TAPR WSPR Pi HATs**
- Interchangeable on a Pi running either **WWoT** or the **native WSPR‑zero image**
- Simple, robust hardware for 24/7 low‑power beacon operation

---

## What’s here

- `KiCad/` — schematic and PCB layout (generate Gerbers from here)
- `3D-cases/` — printable case options sized for SMA and header clearances
- `LICENSE` — see licensing terms for this hardware
- `README.md` — this file

---

## Quick build (hardware)

1. Open the project in **KiCad** and export fabrication files (Gerbers + drills).
2. Assemble the board, populating the **low‑pass filter** for your target band.
3. Inspect for shorts and correct orientation; clean flux residues.
4. Mount on a Raspberry Pi GPIO header; ensure SMA and standoffs clear.
5. Connect to a 50 Ω antenna system or a dummy load for bench checks.

> **RF compliance**: Use the **correct LPF** for the band you transmit on. Verify output with a spectrum analyzer if available.

---

## Getting on air (software paths)

Choose either approach:

- **WSPR‑zero image (recommended for a dedicated beacon)**  
  Grab the image and quick‑start at **[wspr-zero.com/downloads](https://wspr-zero.com/downloads)**, then configure callsign, grid, band, and schedule.

> **Time sync matters**: WSPR needs accurate UTC. Keep NTP locked or use a GPS‑disciplined source.

---

## Safety and legal

- Transmit only with an appropriate amateur radio license for your region.
- Operate **within band limits** 

---

## Credits & compatibility

- Pin‑compatible with **TAPR** WSPR Pi HATs.
- Built for seamless use with **WSPR‑zero** and works with **WWoT** on Raspberry Pi.

---

## Contributing

Issues and PRs for hardware tweaks, docs, and case improvements are welcome.

---

## Links

- **WSPR‑zero website**: https://wspr-zero.com  
- **WSPR‑zero GitHub**: https://github.com/zinkwazi/wspr-zero

---



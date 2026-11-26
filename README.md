# StegoChamber

> Optical & Audio Steganography Cryptographic Lab

![Node](https://img.shields.io/badge/Security-Steganography-10b981?style=flat-square) ![Crypto](https://img.shields.io/badge/Algorithm-AES--256--GCM-8b5cf6?style=flat-square) ![Audio](https://img.shields.io/badge/Web_Audio-Carrier_Modulation-06b6d4?style=flat-square) ![License](https://img.shields.io/badge/License-MIT-blue?style=flat-square)

![StegoChamber Official Banner](assets/banner.svg)

## 📌 Executive Overview
An interactive cryptographic workstation for concealing and extracting encrypted payloads inside digital media using spatial LSB manipulation, audio frequency carrier modulation, and AES-256-GCM encryption.

---

## 🏛 System Architecture
The following diagram highlights the internal computation pipeline, data transformations, and rendering passes:

![Architecture Diagram](assets/diagram.svg)

---

## 📷 Live Application Interface
Below is an authentic 1080p high-resolution capture of the live running interface:

![Live Interface](assets/screenshot.png)

---

## 🔬 Technical Deep-Dive
### Core Technical Specifications
- **Spatial Steganography Engine:** Embeds arbitrary binary data into the least significant bits of 24-bit canvas pixel buffers with minimal perceptual delta ($Delta E < 0.2$).
- **Audio Carrier Phase Encoding:** Utilizes Web Audio API to synthesize continuous 44.1 kHz PCM carrier waves with localized phase modulation representing bitstream payloads.
- **Security & Key Derivation:** Client-side PBKDF2 iterations producing 256-bit AES-GCM authenticated ciphertexts with randomized 96-bit initialization vectors.
- **Diagnostic Cryptanalysis:** Includes a multi-tier bitplane slicing utility (planes 0 through 7) and parity divergence visualizers for real-time steganalysis.

---

## 🚀 Quick Start Guide

### Zero-Dependency Launch
This project is built as a self-contained, high-performance HTML5 application with zero runtime dependencies.

1. **Clone the repository:**
   ```bash
   git clone https://github.com/royalodi/stego-chamber.git
   cd stego-chamber
   ```

2. **Launch directly in any modern browser:**
   ```bash
   # Windows (PowerShell)
   Start-Process index.html

   # macOS / Linux
   open index.html || xdg-open index.html
   ```

---

## 📄 License
This project is distributed under the **MIT License**.


---

## 👨‍💻 Author & Lead Maintainer

<table>
  <tr>
    <td align="center" width="150" valign="middle">
      <a href="https://github.com/royalodi">
        <img src="https://github.com/royalodi.png" width="105" height="105" style="border-radius: 50%;" alt="royalodi" />
      </a>
      <br /><br />
      <b>Royal Odi</b><br />
      <sub><i>Full-Stack Engineer</i></sub>
    </td>
    <td valign="top">
      <p>
        Designed, engineered, and maintained by <b>Royal Odi</b>. Full-Stack Engineer focused on building scalable web architectures, robust backend systems, and responsive, high-performance digital experiences.
      </p>
      <p>
        <a href="https://github.com/royalodi"><img src="https://img.shields.io/badge/GitHub-royalodi-181717?style=flat-square&amp;logo=github&amp;logoColor=white" alt="GitHub Profile" /></a>
        <a href="mailto:royalodi.dev@gmail.com"><img src="https://img.shields.io/badge/Email-royalodi.dev%40gmail.com-EA4335?style=flat-square&amp;logo=gmail&amp;logoColor=white" alt="Contact Email" /></a>
        <a href="https://github.com/royalodi?tab=repositories"><img src="https://img.shields.io/badge/Portfolio-Featured_Repositories-10b981?style=flat-square&amp;logo=codeforces&amp;logoColor=white" alt="Portfolio" /></a>
      </p>
    </td>
  </tr>
</table>


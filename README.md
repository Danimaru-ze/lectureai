# Lecture AI

**Lecture AI** is a desktop live lecture assistant for Windows featuring real-time speech transcription, floating Stealth overlay window protection (hidden from screen sharing and screen capture on Windows), integrated AI Assistant Browser panels, and automatic lecture note generation.

---

## Choose Your Edition

Lecture AI is distributed in two editions so you can pick between full GPU-accelerated **offline** transcription or an ultra-lightweight **Bring Your Own Key (BYOK)** cloud installer that runs smoothly even on older or 32-bit laptops.

| Installer | Edition | Architecture | Size | Speech Engine | Best For |
| :--- | :--- | :--- | :--- | :--- | :--- |
| **`Lecture-AI-1.3.1-Full-CUDA-Setup-x64.exe`** | **Full CUDA** | Windows 64-bit (`x64`) | 1518.3 MB | Bundled Faster-Whisper (CUDA + CPU) + Cloud Gemini / Groq | Maximum privacy and 100% offline transcription with no per-minute API cost |
| **`Lecture-AI-1.3.1-BYOK-Setup-x64.exe`** | **BYOK** | Windows 64-bit (`x64`) | 74.1 MB | Cloud Gemini Live & Groq Whisper APIs (via your own API key) | Modern 64-bit laptops with limited disk space or without a dedicated NVIDIA GPU |
| **`Lecture-AI-1.3.1-BYOK-Setup-ia32.exe`** | **BYOK** | Windows 32-bit (`ia32` / `x86`) | 68.7 MB | Cloud Gemini Live & Groq Whisper APIs (via your own API key) | Legacy 32-bit Windows systems and lightweight netbooks |
| **`Lecture-AI-1.3.1-BYOK-Setup-Universal.exe`** | **BYOK** | Universal (`x64` + `ia32`) | 143.6 MB | Cloud Gemini Live & Groq Whisper APIs (via your own API key) | Single installer that automatically installs the right binary on any Windows PC |

> Download installers from the [**GitHub Releases**](https://github.com/Danimaru-ze/lectureai/releases/latest) page.

---

## Edition Comparison

| Feature | Full CUDA Edition | BYOK Edition |
| :--- | :--- | :--- |
| **Offline Faster-Whisper Transcription** | Included (CUDA GPU + CPU fallback, `faster-whisper-small` model + Silero VAD pre-bundled) | Not included (Cloud APIs only) |
| **Gemini Live Real-Time STT** | Supported (BYOK API key) | Supported (BYOK API key) |
| **Groq Whisper Cloud STT** | Supported (BYOK API key) | Supported (BYOK API key) |
| **System Audio Loopback + Microphone** | Supported (Python WASAPI capture) | Supported (Native desktop loopback + microphone capture) |
| **Stealth Mode (Anti-Screen Capture)** | Included | Included |
| **Compact & Always-On-Top Floating UI** | Included | Included |
| **Integrated AI Browser & Lecture Notes** | Included | Included |
| **Python or CUDA Toolkit Pre-Installed?** | Not required (self-contained runtime bundled inside installer) | Not required |
| **Approximate Disk Size After Install** | ~2.6 GB | ~220 MB |

---

## System Requirements

### Minimum Requirements (BYOK Edition)
- **OS**: Windows 10 or Windows 11 (`x64` or 32-bit `x86` depending on installer; Universal works on both)
- **RAM**: 4 GB or higher
- **Storage**: 300 MB free disk space
- **Network**: Stable internet connection for cloud STT (Gemini Live / Groq Whisper) and license verification

### Recommended Requirements (Full CUDA Edition)
- **OS**: Windows 10 or Windows 11 (64-bit `x64`)
- **CPU**: Quad-core processor or better (also used automatically if no CUDA GPU is available)
- **GPU (Recommended for Offline Speed)**: NVIDIA GPU with updated drivers supporting CUDA
- **RAM**: 8 GB or higher
- **Storage**: 4 GB free disk space (installer download + extracted files)

---

## Installation & Quick Start

1. Download the `.exe` installer matching your system from [**Releases**](https://github.com/Danimaru-ze/lectureai/releases/latest).
2. Run the setup executable and follow the installation wizard.
   - *(Optional)* Verify your download integrity against [SHA256SUMS.txt](./SHA256SUMS.txt).
3. Launch **Lecture AI** and activate your **License Key** from [lectureai.web.id](https://lectureai.web.id/).
4. Open **Settings -> Speech-to-Text**:
   - **Full CUDA Edition**: **Offline / Local** works immediately out of the box using your NVIDIA CUDA GPU (with automatic CPU fallback). You can also add a **Gemini** or **Groq** API key to switch to Cloud STT anytime.
   - **BYOK Edition**: Enter your **Gemini API Key** (Google AI Studio) and/or **Groq API Key**, select your preferred audio source (**System Audio** or **Microphone**), and start recording.

---

## Verification (SHA-256 Checksums)

You can verify the integrity of downloaded installers in PowerShell with `Get-FileHash <filename>.exe -Algorithm SHA256`:

| File | SHA-256 |
| :--- | :--- |
| `Lecture-AI-1.3.1-Full-CUDA-Setup-x64.exe` | `0A02312BE8DDFBFD308B99B34843B419418CE06343E86B4B08A1C659E77E06EC` |
| `Lecture-AI-1.3.1-BYOK-Setup-Universal.exe` | `B24E73F61E76681C3BF5A35F53865AD2F672224283AF27E82609681D36BB5E71` |
| `Lecture-AI-1.3.1-BYOK-Setup-x64.exe` | `4F7256EBE095DB3D687098A8224052ED71D33D930F099D4E9CA397ADB6538043` |
| `Lecture-AI-1.3.1-BYOK-Setup-ia32.exe` | `360D9A23A35CB7EB46127B497593A8AF5334DFEAECA35F2B35ADCFDBC30D8D31` |

---

## License & Author

Created by **Dany Setiyawan**. Official license management portal: [https://lectureai.web.id/](https://lectureai.web.id/).

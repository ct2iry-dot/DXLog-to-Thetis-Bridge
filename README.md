DXLog ↔ Thetis Bridge



![icon](https://github.com/user-attachments/assets/836cd542-bb17-40c4-b23e-3d938343b45e)








A lightweight, high-performance bridge that connects DXLog with Thetis SDR, enabling real-time synchronization between logging software and SDR transceivers.


📸 Screenshots


<img width="898" height="651" alt="Screenshot 2026-03-30 172934" src="https://github.com/user-attachments/assets/a4ccf134-6c99-402b-8fe2-2ae2bbdd1551" />



📡 Overview

DXLog ↔ Thetis Bridge provides seamless communication between:

📝 DXLog (contest logging software)
📻 Thetis (OpenHPSDR SDR client)

It acts as a middleware layer, allowing both systems to stay synchronized in real time — improving efficiency for contesting, DXing, and SDR-based stations.

✨ Features
🔗 Real-time frequency and mode synchronization
📡 Band tracking between DXLog and Thetis
⚡ Low-latency communication layer
🧩 Simple and intuitive configuration
🪶 Lightweight and efficient (minimal CPU usage)
🛠 Optional advanced / Pro features support
🔄 Designed for multi-instance SDR workflows
🏗 Architecture
DXLog  ⇄  Bridge  ⇄  Thetis
          │
          ├── CAT
          ├── UDP
          └── TCI (optional)
🖥 Requirements
Windows 10 / 11
DXLog installed and configured
Thetis SDR software
(Optional) Hermes Lite 2 or OpenHPSDR-compatible hardware
🚀 Installation
Option 1 — Installer
Download the latest release from the Releases page
Run the installer
Launch the application
Option 2 — Manual
Clone the repository:
git clone https://github.com/ct2iry-dot/dxlog-thetis-bridge.git
Run the executable from /dist or build manually
⚙️ Configuration
DXLog
Enable CAT or UDP output
Set correct COM port / network settings
Thetis
Enable CAT or TCI interface
Configure port matching the bridge
Bridge
Set:
IP address (usually 127.0.0.1)
Ports for DXLog and Thetis
Protocol (CAT / TCI)
🧪 Usage
Start Thetis
Start DXLog
Launch DXLog ↔ Thetis Bridge
Verify synchronization:
Frequency changes
Mode updates
Band switching
🧰 Development
Build Requirements
Python 3.x (if applicable)
PyInstaller (if packaging to EXE)
Inno Setup (for installer)
Build EXE
pyinstaller --onefile main.py
🔄 Continuous Integration

This project uses GitHub Actions for:

✅ Build validation
✅ Packaging checks
✅ Release automation (optional)

Workflow file:

.github/workflows/build.yml
🗺 Roadmap
 Improved TCI support
 Advanced logging sync
 GUI enhancements
 Auto-discovery of services
 Linux support (experimental)
🤝 Contributing

Contributions are welcome!

Fork the project
Create your feature branch
Commit your changes
Open a Pull Request
🐛 Issues

Found a bug or want a feature?

👉 Open an issue:
https://github.com/ct2iry-dot/dxlog-thetis-bridge/issues

📄 License

This project is licensed under the MIT License.

👤 Author

CT2IRY

GitHub: https://github.com/ct2iry-dot

⭐ Support

If you find this project useful, consider giving it a ⭐ on GitHub!

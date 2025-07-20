
         



CamHack is a reconnaissance tool designed to help researchers and security enthusiasts check if an IP address is hosting an exposed CCTV camera. It scans common camera ports, checks for login pages, tests default credentials, and provides useful search links for further investigation.

⚠️ Disclaimer: This tool is intended for educational and security research purposes only. Unauthorized scanning of systems you do not own is illegal. Use responsibly.

☁️ Run It Instantly on Google Colab (No Installation Needed)
Open In Colab

🆕 What's New in v2.0.1
Massive port scan: Now scans 1000+ ports, including custom and high camera ports
CP Plus (CP-UVR-0401E1-IC2) and DVR/NVR detection
Enhanced live stream detection (RTSP/HTTP/RTMP/MMS, with real stream validation)
Multi-threaded authentication and password brute-force (much faster)
Improved camera indicator analysis (brand, model, login forms, titles)
Comprehensive IP/location info with Google Maps/Earth links
Improved error handling and progress reporting
🚀 Features
✔️ Scans all common CCTV ports
✔️ Detects exposed camera login pages
✔️ Checks if the device is a camera stream
✔️ Identifies camera brands & known vulnerabilities
✔️ Tests for default credentials on login pages
✔️ Provides manual search links (Shodan, Censys, Zoomeye, Google Dorking)
✔️ Google Dorking suggestions for deeper recon
✔️ Enhanced Camera Detection with detailed port analysis and brand identification
✔️ Live Stream Detection for RTSP, RTMP, HTTP, and MMS protocols
✔️ Comprehensive IP & Location Information with Google Maps/Earth links
✔️ Multi-threaded Port Scanning for faster results
✔️ Enhanced Error Handling and SSL support
✔️ Detailed Camera Brand Detection (Hikvision, Dahua, Axis, Sony, Bosch, Samsung, Panasonic, Vivotek, CP Plus)
✔️ ONVIF Protocol Support for standardized camera communication
✔️ Smart Brute-force Protection with rate limiting
✔️ Detailed Port Analysis showing server information and authentication types

📚 Supported Brands & Devices
Hikvision, Dahua, Axis, Sony, Bosch, Samsung, Panasonic, Vivotek, CP Plus, and most generic DVR/NVRs
CP Plus DVRs (e.g., CP-UVR-0401E1-IC2) with custom ports
Any device exposing RTSP, HTTP, RTMP, or MMS video streams
🛠️ Installation
1️⃣ Clone the Repository
git clone https://github.com/Cybersojib12/CamHack
cd CamHack
pip install -r requirements.txt
python CamHack.py
Enter the public IP address of the target device when prompted.

🔍 What It Does:
1️⃣ Scans open ports (Common CCTV ports)
2️⃣ Checks if a camera is present
3️⃣ If a camera is found, it:

Searches for login pages
Checks default credentials
Identifies camera brand & vulnerabilities
Detects live streams (RTSP, RTMP, HTTP, MMS)
Provides location information with maps
Shows server details and authentication types
4️⃣ Provides manual search URLs for deeper investigation
⚡ Usage Tips
Scanning all ports (1000+) may take several minutes, depending on your network and target.
The tool uses multi-threading for port, login, and password checks for speed.
If you see "No camera found" but you know a camera is present, check the open ports and look for custom ports in the output.
For best results, run as administrator/root to avoid local firewall issues.
📚 Troubleshooting
If no open ports are found, ensure the target is online and not behind a strict firewall.
If live streams are not detected, try accessing the URLs manually in VLC or a browser.
For best detection, ensure your Python version is 3.6+ and all dependencies are installed.

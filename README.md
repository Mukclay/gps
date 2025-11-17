
Unit]
Description GPS Service Autorun
After network.target

[Service]
ExecStart=/usr/bin/python3 /home/pi5/Dokumen/gps_cctv/gps.py
WorkingDirectory=/home/pi5/Dokumen/gps_cctv
StandardOutput=inherit
StandardError=inherit
Restart always
User=pi5

[Install]
WantedBy=multi-user.target

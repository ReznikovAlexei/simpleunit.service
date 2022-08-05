# simpleunit.service
Simple SystemD unit

[Unit]
Description=example systemd service unit file.

[Service]
ExecStart=/bin/bash /usr/sbin/example.sh

[Install]
WantedBy=multi-user.target

To reload systemd with this new service unit file, run:
systemctl daemon-reload

Finally to start the script on boot, enable the service with systemd:
systemctl enable test.service

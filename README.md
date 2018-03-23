# systemd unit file for Dropbox

I was having trouble finding a dropbox unit file that worked properly so I created this one that properly uses the PID file dropbox creates to manage the service.

## Install

1. Copy `dropbox@.service` to `/etc/systemd/system`
2. Reload systemd with `systemctl daemon-reload`
3. Enable the service for your user with `systemctl enable dropbox@<USER>`
4. Start the service for your user with `systemctl start dropbox@<USER>`

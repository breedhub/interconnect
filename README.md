# Work in progress

### Tracker

1. Install Node 6

2. npm install -g bhit

3. bhit install my.host.name

  Certificate will be generated as certs/my.host.name.cert

4. systemctl daemon-reload

  systemctl enable bhit

5. Edit /etc/bhit/bhit.conf if needed

6. systemctl start bhit

7. See the logs: journalctl -fu bhit

### Daemon

1. Install Node 6

2. npm install -g bhid

3. bhid install this-daemon-name

  Peer public key will be id/this-daemon-name.public.rsa

4. systemctl daemon-reload

  systemctl enable bhid

5. Edit /etc/bhid/bhid.conf

  Upload tracker .cert file to certs/ directory (only needed if using default self-signed certificate and do not copy .key file)
  
  Upload public key of your peer to peers/ directory (only .public.rsa file, .private.rsa should not be copied anywhere)

6. systemctl start bhid

7. See the logs: journalctl -fu bhid

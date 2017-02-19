# Work in progress

### Tracker

1. Install Node 6+, Postgres 9.4+, Redis 3+

2. apt-get install build-essential

3. npm install -g bhit --unsafe-perm

4. bhit install my.host.name

  Certificate will be generated as certs/my.host.name.cert

5. systemctl daemon-reload

  systemctl enable bhit

6. Edit /etc/bhit/bhit.conf

7. systemctl start bhit

### Daemon

1. Install Node 6+

2. apt-get install build-essential

3. npm install -g bhid --unsafe-perm

4. bhid install

5. systemctl daemon-reload

  systemctl enable bhid

 systemctl start bhid

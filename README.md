# MOTD

Customize your MOTD login message in Debian and Ubuntu

# Installation

1. We need to turn off (yes, off) SSH's PrintMotd option by editing /etc/ssh/sshd_config:

   ```bash
     PrintMotd no
   ```

   This stops printing from the plaintext /etc/motd and lets us print our own content.

2. Now we'll place our shell script into /etc/profile.d
   ```bash
   /etc/profile.d/welcome.sh
   ```
3. Give the file the necessary rights to execute
   ```
   chmod +x /etc/profile.d/welcome.sh
   ```
4. Restart the ssh service

   ```bash
    service ssh reload
    ```
<br>

#### © 2021 Panda-Network
> Webseite: [Panda-Network.de](https://panda-network.de) \
> Support [Discord-Server](https://discord.gg/z8ScRvf)



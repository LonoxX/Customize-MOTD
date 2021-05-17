# MOTD

Customize your MOTD login message in Debian and Ubuntu

# Installation

1. We need to turn off (yes, off) SSH's PrintMotd option by editing /etc/ssh/sshd_config:

   ```bash
     PrintMotd no
   ```

   This stops printing from the plaintext /etc/motd and lets us print our own content.

2. Now we'll place our shell script into /etc/profile
   ```bash
   /path_to_file/welcome.sh
   ```
3. give the file the necessary rights to execute
   ```
   chmod +x /path_to_file/welcome.sh
   ```
4. Restart the ssh service

   ```bash
    service ssh reload
    ```


## Support

Panda-Network Discord [Discord-Server](https://discord.gg/z8ScRvf)

#### © 2021 Panda-Network


# passupd
Password updater script for Linux

**NOTE: TAKE NOTICE THE NEW FORMAT OF THE PASSWORD BEFORE IMPLEMENTING OR YOU WILL BE LOCKED OUT**

1. `nano passupd` and replace {user} with user

2. locate `passupd` in `/usr/local/bin`

3. `chown root:root /usr/local/bin/passupd`

4. `crontab -e -u root`
```
key:
01 00 * * * /usr/local/bin/passupd
@reboot /usr/local/bin/passupd
```

5. reboot

6. {user} now has a new password updated at 0100 daily and reboot

**NOTE: TAKE NOTICE THE NEW FORMAT OF THE PASSWORD BEFORE IMPLEMENTING OR YOU WILL BE LOCKED OUT**

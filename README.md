# ubuntu-NTP-
Time was not in sync on ubuntu server and unable the start the service

timedatectl

systemctl status systemd-timesyncd.service

Error details :Apr 29 10:00:01 ip-172-31-47-214 systemd[1]: Failed to start Network Time Synchronization.




Installing ntp would fix the issue

sudo apt install ntp

service ntp start  

timedatectl

System clock synchronized: yes

systemd-timesyncd.service active: yes

RTC in local TZ: yes

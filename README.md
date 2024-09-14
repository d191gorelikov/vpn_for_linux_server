# vpn_for_linux_server
Service for connecting to a VPN on a Linux server


1.sudo systemctl enable xray
2.sudo systemctl start xray
3.1
Для конкретного пользователя

Откройте файл .bashrc
Добавьте в файл .bashrc следующие строки:

export http_proxy="http://127.0.0.1:1081"
export https_proxy="http://127.0.0.1:1081"

и выполнить source ~/.bashrc

3.2 

Для всех пользователей

Добавьте в файл  /etc/environment следующие строки:
 
http_proxy="http://127.0.0.1:1081"
https_proxy="http://127.0.0.1:1081"

и выполнить source /etc/environment

3.3 

Также можно добавить эти же переменные в файл /etc/profile, который загружается для всех пользователей при каждом входе в систему.

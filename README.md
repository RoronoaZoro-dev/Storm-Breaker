<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/648d564c-387e-485d-8eb3-423f6afde4d2" />

#Storm-Breaker

Storm-Breaker is a web-based tool designed for educational and research purposes, demonstrating how browser-based permissions and user interactions can expose device-level information.

It includes multiple templates, including a Zomato-style landing page, used to generate live interaction links.

🚀 Features

Obtain device information without explicit permissions

Access live location (smartphones)

Access webcam

Access microphone

Web-based control panel (GUI)

Multiple optimized templates

Downloadable logs

Clear logs option

Start / stop listener anytime

Can be hosted on localhost or personal domain

Redesigned and improved user interface

🆕 Update Log
Second (Latest) Update – November 4, 2022

Complete rewrite of the tool structure

Web panel introduced (previous versions were CLI-based)

Previous version bugs fixed

Auto-download Ngrok added

Templates optimized

Logs can now be downloaded (NEW)

Clear log option added

Can be uploaded on a personal host (no Ngrok dependency)

Listener can be started or stopped anytime

Beautified user interface (NEW)

Ngrok removed from default workflow

Tool now runs on localhost

User must manually start Ngrok if required

⚠️ Important Notes

This version can run on localhost or a personal hosting/domain

Recommended to use personal hosting if:

Ngrok is blocked in your country

Ngrok links appear suspicious to users

Ngrok service is unavailable

For full functionality, SSL is required, even on localhost

🔐 Default Login Credentials

Username: admin

Password: admin

You can change these in:

storm-web/config.php

📦 Dependencies

Storm-Breaker requires the following programs:

php

python3

git

ngrok

🖥 Platforms Tested

Kali Linux 2022

macOS Big Sur (M1)

Termux (Android)

Personal hosting (cPanel / Direct Admin)

🛠 Installation (Kali Linux)
git clone https://github.com/ultrasecurity/Storm-Breaker
cd Storm-Breaker
sudo bash install.sh
sudo python3 -m pip install -r requirements.txt

▶️ How to Run Storm-Breaker

After completing the installation, follow these steps to run Storm-Breaker and expose it using Ngrok.

1️⃣ Start Storm-Breaker

From the project root directory, run:

python st.py


This will start the Storm-Breaker service on localhost.

2️⃣ Install Ngrok (if not installed)
sudo apt install ngrok

3️⃣ Expose the Localhost Using Ngrok

Storm-Breaker runs on port 2525 by default.
Start Ngrok with:

ngrok http 2525

4️⃣ Use the Ngrok Link

Ngrok will generate a public HTTPS link

Copy the generated link

Open it in a browser or share it

The link will redirect users to the Storm-Breaker web interface

Once the link is opened, the selected template (for example, the Zomato-style landing page) will load and function as configured.

🌐 Running on Personal Hosting

Open the storm-web folder

Zip only the contents inside storm-web

Upload them to:

public_html/


⚠️ Do NOT upload the storm-web folder itself

Correct:

public_html/index.php


Wrong:

public_html/storm-web/index.php

⚠️ Additional Attention

SSL is mandatory for many features

On Termux, Ngrok requires:

Personal hotspot enabled

Cellular network active

If Ngrok is blocked in your country, use a personal hosting/domain instead

📌 Disclaimer

This project is developed strictly for educational, testing, and research purposes.
Any misuse, unauthorized tracking, or invasion of privacy is strictly prohibited.
The author takes no responsibility for misuse or illegal activity.

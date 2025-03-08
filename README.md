WebLock - Advanced Intrusion Detection System
-Team Sentinals

Project Structure

weblock/
│── app.py                      # Main Flask application
│── database.py                  # MongoDB integration
│── trap.py                      # Intruder monitoring system
│── model/
│   ├── algorithm.py             # Security logic (brute-force, SQLi, XSS detection)
│   ├── admin_settings.json      # Admin & Dashboard user credentials
│   ├── approved_ips.json        # List of authorized IP addresses
│   ├── brute_force_patterns.json # Brute-force detection settings
│   ├── data.json                # User credentials
│   ├── sql_injection_patterns.json # SQL Injection attack patterns
│   ├── xss_patterns.json        # XSS attack patterns
│── instance/
│   ├── database.py              # Data upload to MongoDB
│── static/
│   ├── adminstyle.css           # Stylesheet for admin dashboard
│   ├── adminscript.js           # JavaScript for admin dashboard
│── templates/
│   ├── login.html               # Login page
│   ├── admin.html               # Admin dashboard (Elastic-style)
│   ├── dashboard.html           # Intruder monitoring page
│   ├── server.html              # Main server page after login
│   ├── admindash.html           # Dashboard for dash_users
│── keylogger_logs/
│   ├── keystrokes.txt           # Logged keystrokes
│   ├── screenshots/             # Captured screenshots
│── capture/
│   ├── intruders/               # Images of detected intruders
│── intruder_log.csv             # Logs of detected intruders
│── employee_log.csv             # Employee login details
│── requirements.txt             # Python dependencies
│── README.md                    # Project documentation



WebLock is a powerful cybersecurity system that protects your application from unauthorized access. It monitors login attempts, detects brute-force attacks, prevents SQL/XSS injections, and tracks keystrokes. Any suspicious activity is logged and analyzed in a dedicated admin dashboard, providing real-time insights into potential security threats.
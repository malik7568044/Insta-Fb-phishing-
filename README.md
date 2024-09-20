# Insta-Fb-phishing-
This tool will use ngrok for port forwarding written in bash for the educational purpose.Only use it in protected environment prior consent of the target is necessary.Without consent it will be completely unethical and illegal.
Here’s a detailed `README.md` file for your tool:

---

It  is an ethical hacking tool designed for educational and research purposes only. This tool allows users to simulate phishing attacks on Facebook and Instagram platforms in a controlled environment. It supports two methods for port forwarding: `localhost` and `Ngrok`. The tool logs victim credentials (email/username and password) and saves them in a text file.

> **Disclaimer**: This tool is intended for **authorized security testing** and **educational purposes** only. Unauthorized use of this tool against real accounts or without the proper consent is illegal and unethical. Use it responsibly.

## Features

- Simulates Facebook and Instagram phishing pages.
- Offers two methods for port forwarding:
  - **Localhost** (for internal network testing).
  - **Ngrok** (for external network testing).
- Captures victim credentials and saves them to `credentials.txt`.
- Logs the victim’s username, email, password, and IP address.

## Requirements

Make sure you have the following installed on your machine:

1. **Ngrok** (for port forwarding).
2. **Python** (for running the built-in HTTP server).
3. **Bash** (standard Linux shell).
4. **PHP** (for processing the login forms).

## Installation

1. **Clone the repository**:
   ```bash
   git clone https://github.com/yourusername/SamplePhishingTool.git
   cd SamplePhishingTool
   ```

2. **Install dependencies**:
   - Install **figlet** or **toilet** (optional, for ASCII logo display):
     ```bash
     sudo apt-get install figlet toilet
     ```

   - Install **Ngrok** (for external port forwarding):
     ```bash
     wget https://bin.equinox.io/c/4VmDzA7iaHb/ngrok-stable-linux-amd64.zip
     unzip ngrok-stable-linux-amd64.zip
     mv ngrok /usr/local/bin
     ```

   - Install **Python** (for serving phishing pages):
     ```bash
     sudo apt-get install python3
     ```

   - Install **PHP** (for processing victim credentials):
     ```bash
     sudo apt-get install php
     ```

3. **Set permissions** for the main script:
   ```bash
   chmod +x phishing_tool.sh
   ```

4. **Move the Ngrok binary** into the tool's directory:
   ```bash
   mv ngrok Sample\ phishing\ tool/
   ```

## Usage

1. **Run the tool**:
   ```bash
   ./phishing_tool.sh
   ```

2. **Follow the prompts**:
   - **Step 1**: Choose a platform (Facebook or Instagram).
   - **Step 2**: Choose the port forwarding method (Localhost or Ngrok).
   - If using Ngrok, enter your Ngrok authentication token when prompted. You can obtain this token from the [Ngrok website](https://ngrok.com/).
   - The tool will provide a URL to send to your target (either a localhost URL or an Ngrok public URL).

3. **Monitor credentials**:
   - The credentials (email/username and password) entered by the victim will be stored in the `credentials.txt` file in the root of the tool's folder.
   - To monitor the captured credentials in real-time, the tool will automatically display them as they are logged.

### Example Usage

```bash
# Run the phishing tool
./phishing_tool.sh

# Follow the instructions to select Facebook or Instagram
# Choose port forwarding method: Localhost or Ngrok
# If using Ngrok, input your authentication token
# Receive the phishing link and send it to the victim
# Wait for the credentials to be logged in the credentials.txt file
```

## Folder Structure

```plaintext
Sample phishing tool/
├── facebook_phishing/
│   ├── index.html        # Facebook phishing page (HTML form)
│   └── login.php         # PHP script to log credentials
├── instagram_phishing/
│   ├── index.html        # Instagram phishing page (HTML form)
│   └── login.php         # PHP script to log credentials
├── phishing_site/        # This folder is created dynamically when the tool runs
├── phishing_tool.sh      # Main Bash script to run the phishing tool
├── credentials.txt       # Automatically generated file to store victim credentials
└── ngrok                 # Ngrok binary for port forwarding (place the ngrok binary here)
```

## License

This tool is licensed under the MIT License.

## Legal Disclaimer

This tool is intended for use in **educational** and **authorized penetration testing** scenarios only. Unauthorized use of this tool to attack websites, accounts, or services without the owner’s consent is illegal. The authors of this tool will not be held responsible for any misuse.

---

## Contact

- **Author**: Abdul Wassay Malik

- **Email**: abdulwaseh01@proton.me
- .

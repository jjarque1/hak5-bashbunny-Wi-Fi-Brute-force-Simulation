# Wi-Fi Brute-force Simulation

---

## Description

The **Wi-Fi Brute-force Simulation** is a payload designed to demonstrate how a brute-force attack can be performed on WPA/WPA2 Wi-Fi networks in a controlled and ethical environment. Using tools such as `aircrack-ng`, this payload captures the WPA/WPA2 handshake of a target network and attempts to crack it using a dictionary attack. The payload is meant to show the vulnerabilities of weak Wi-Fi passwords and highlight the importance of strong password policies.

## How it Works

1. The payload starts by enabling monitor mode on the Wi-Fi interface (wlan0).
2. It uses `airodump-ng` to capture the WPA/WPA2 handshake of the target network.
3. Once the handshake is captured, it attempts to crack the password using `aircrack-ng` with a predefined wordlist.
4. The captured handshake and cracking results are saved to the Bash Bunny's storage for further analysis.

## Requirements

- Target: Linux machine with wireless capabilities
- Installed tools: `aircrack-ng`, `airodump-ng`
- Bash Bunny in HID and storage mode
- A wordlist file for the brute-force attack
- Access to a test Wi-Fi network for ethical use

## Ethical Use Disclaimer

This payload is for educational and ethical hacking purposes only. Unauthorized use of this script to attack Wi-Fi networks is illegal and unethical. Ensure that you are using this script in a controlled environment and with permission from the network owner.

## Liability Disclaimer

The author of this payload assumes no responsibility for any illegal or unethical use of the code. This payload is provided as-is, and it is the user's responsibility to ensure its use complies with all applicable laws and regulations.

## Usage

1. Insert the Bash Bunny into the target machine.
2. The payload will automatically capture the WPA/WPA2 handshake and attempt to crack it.
3. Once the process is complete, the results will be saved in the `/wifi_bruteforce_handshake.cap` file on the Bash Bunny's storage.
4. Eject the Bash Bunny and analyze the captured handshake and results.

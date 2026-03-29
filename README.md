# Network Port Scanner GUI

A lightweight multi-threaded TCP port scanner developed in Python with a graphical user interface using Tkinter. This tool allows users to scan a target system for open ports within a given range and identify commonly used network services.

## Project Overview

The Network Port Scanner GUI is designed to demonstrate basic network security concepts such as port scanning, socket programming, and multi-threading. The application provides a simple interface where users can enter a target IP address or hostname and scan a range of ports to detect active services.

The scanner attempts TCP connections to each port and reports ports that accept connections as open. To improve performance, the tool uses concurrent threads to scan multiple ports simultaneously. The results are displayed in real time along with scan progress and elapsed time.

This project is mainly intended for educational purposes and basic network analysis.

## Features

- Simple GUI interface with minimal input fields
- Fast multi-threaded port scanning
- Detection of commonly known services (HTTP, FTP, SSH, etc.)
- Live scan progress display
- Option to stop scanning anytime
- Save scan results to a text file
- Works on Windows, Linux, and macOS
- Uses only Python standard libraries

## Technologies Used

- **Python 3**
- **Tkinter** (GUI development)
- **Socket Programming** (TCP connections)
- **Threading module** (parallel scanning)
- **Queue module** (thread communication)
- **Time module** (scan timing)

## Requirements

Make sure the following are installed:

- Python 3.7 or above
- Tkinter (comes preinstalled with Python)

Check Python version:
```
python --version
```

## Installation

Clone this repository:

```
git clone https://github.com/craftedBySravya/network-port-scanner-gui.git
```

Move into the project directory:

```
cd network-port-scanner-gui
```

## How to Run

Run the program using:

```
python portscanergui.py
```

## Usage Instructions

1. Enter the **Target IP address** or **Hostname**
   - Example: 192.168.1.1
   - Example: localhost

2. Enter **Start Port** and **End Port**
   - Default range: 1 – 1024

3. Click **Start Scan**

4. The program will:
   - Scan ports
   - Show progress
   - Display open ports

5. Click **Stop** if you want to cancel scanning.

6. Click **Save Results** to export open ports list.

## Detected Services

The scanner automatically identifies some common ports:

| Port | Service |
|------|---------|
| 21 | FTP |
| 22 | SSH |
| 23 | Telnet |
| 25 | SMTP |
| 53 | DNS |
| 80 | HTTP |
| 110 | POP3 |
| 143 | IMAP |
| 443 | HTTPS |
| 3306 | MySQL |
| 3389 | RDP |
| 5900 | VNC |
| 8080 | HTTP Alternate |

Ports not listed are shown as **Unknown**.

## Project Structure

```
network-port-scanner-gui/
│
├── portscanergui.py
├── README.md
```

## Applications

- Basic network security analysis
- Learning socket programming
- Cyber security practical demonstrations
- SOC monitoring basics
- Network troubleshooting
- Identifying exposed services

## Limitations

- Only TCP connect scanning is implemented
- Does not perform UDP scanning
- Cannot detect filtered ports
- Limited service detection
- Performance depends on system resources

## Future Improvements

- Add UDP scanning
- Add OS detection
- Add vulnerability detection
- Add scan report in PDF format
- Add advanced service fingerprinting
- Improve UI design
- Add dark mode interface

## Disclaimer

This project is created strictly for educational purposes.  
Do not scan systems or networks without proper authorization. Unauthorized scanning may violate laws or organizational policies.

## Author

Pagolu Sravya
BTech CSE (Cyber Security & Digital Forensics)  
National Forensic Sciences University

## License

This project is released under the MIT License.

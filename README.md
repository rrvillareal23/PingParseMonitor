# PingParseMonitor

PingParseMonitor is a Python-based tool for monitoring website connectivity and network performance. The tool pings a list of specified websites, parses the ping results, and logs key network statistics, including packet transmission, packet loss, and round-trip times. The results are saved in a human-readable `.txt` file for easy reference.

## Features

- Pings a set of predefined websites and captures network statistics
- Parses the ping results using the `pingparsing` library
- Handles connectivity issues gracefully by setting default values if ping results are unavailable
- Saves results to a `.txt` file for easy access

## Installation

Before running this script, ensure you have the required libraries installed. You can install them with:

pip install pingparsing numpy

# Usage
1. Edit the WEBSITES dictionary in the script to include the websites you want to monitor.

2. Run the script: python PingParseMonitor.py

3. The script will display the ping statistics in the console and save them to a file named ping_results.txt.

# Configuration
- Error Handling: If a website is unreachable, PingParseMonitor automatically sets round-trip times to -1 to indicate that the data is unavailable. This prevents the script from failing due to connection issues.

# License
This project is licensed under the MIT License. See the LICENSE file for details.

# Contributing
Feel free to submit issues or pull requests for additional features or improvements.

# Acknowledgements
Thanks to the pingparsing library for handling the parsing of ping results.

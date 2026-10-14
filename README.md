# CyberScope – Attack Surface Lookup Bot

## About the Project

CyberScope is a Telegram-based cybersecurity bot built using n8n and Shodan InternetDB. It checks an IP address for exposed ports, hostnames, and known vulnerabilities.

## Features

* Accepts IP addresses through Telegram commands.
* Retrieves information using Shodan InternetDB.
* Identifies watched ports: 110, 5432, and 5900.
* Assigns a HIGH risk level when a watched port is detected.
* Masks the last octet of the IP address before AI analysis.
* Provides security insights and hardening recommendations.
* Handles source API failures with a notification.

## Technologies Used

* n8n Cloud
* Telegram Bot API
* Shodan InternetDB
* AI Agent / Language Model
* HTTP Request and Code nodes

## How to Use

1. Open the Telegram bot.
2. Send `/ip <IP-address>`.
3. The workflow queries Shodan InternetDB.
4. The workflow analyses the results and returns a security report.

## Example

Command: `/ip 8.8.4.4`

The bot checks the IP address and reports its exposed ports and risk level.

## Project Screenshots

### 1. n8n Workflow
![CyberScope Workflow](screenshots/workflow.png)

### 2. Telegram Bot Results
![Telegram Bot Results](screenshots/telegram-results.png)

## Project Tag

NGP-047

## Disclaimer

This project is intended for educational and authorized cybersecurity analysis only.

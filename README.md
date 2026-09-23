# ipguard
IPGuard is a Python-based IP investigation tool that validates IP addresses, identifies IPv4/IPv6 and public/private classifications, retrieves geolocation and network ownership information, performs reverse DNS lookups, and generates structured JSON investigation reports.
# IPGuard

IPGuard is a Python-based IP investigation and network intelligence tool designed to collect and organize publicly available information about IP addresses.

The tool validates IP addresses, identifies their type and version, retrieves geographic and network ownership information, performs reverse DNS lookups, and generates structured JSON investigation reports.

## Features

* IPv4 and IPv6 validation
* IPv4/IPv6 identification
* Public/private IP classification
* Reserved, loopback, and multicast detection
* Reverse DNS lookup
* Country and region information
* City and postal code information
* ISP identification
* Organization information
* ASN information
* Domain information
* Geographic coordinates
* Timezone information
* Timestamped investigation reports
* JSON report generation
* Network error handling

## Technologies Used

* Python
* Requests
* IPaddress
* Socket
* JSON
* Public IP information API

## Project Structure

```text
ipguard/
│
├── ipguard.py
├── requirements.txt
├── README.md
└── .gitignore
```

## How It Works

1. The user enters an IP address.
2. IPGuard validates the address.
3. The application determines whether it is IPv4 or IPv6.
4. The address is classified as public, private, reserved, loopback, or another type.
5. For public IP addresses, IPGuard retrieves available network intelligence.
6. A reverse DNS lookup is performed.
7. The information is displayed as an investigation report.
8. The user can save the results as a JSON file.

## Installation

Clone the repository:

```bash
git clone https://github.com/YOUR_USERNAME/ipguard.git
```

Enter the project directory:

```bash
cd ipguard
```

Create a virtual environment:

```bash
python -m venv venv
```

Activate the environment on Windows:

```powershell
venv\Scripts\activate
```

Install the dependencies:

```bash
pip install -r requirements.txt
```

## Running the Tool

Start the application:

```bash
python ipguard.py
```

Enter a public IP address when prompted.

Example:

```text
8.8.8.8
```

## Example Output

```text
IPGUARD
IP INVESTIGATION REPORT

NETWORK INFORMATION
----------------------------------------------------------------------
IP Address    : 8.8.8.8
IP Version    : IPv4
IP Type       : PUBLIC
Reverse DNS   : ...

LOCATION INFORMATION
----------------------------------------------------------------------
Country       : ...
Region        : ...
City          : ...
Timezone      : ...

NETWORK OWNER
----------------------------------------------------------------------
ISP           : ...
Organization  : ...
ASN           : ...
Domain        : ...
```

## JSON Reports

IPGuard can save investigation results in JSON format.

Example:

```text
ipguard_report_20260923_091500.json
```

The report contains structured information including:

* Investigation timestamp
* IP address
* IP version
* IP classification
* Reverse DNS
* Geographic information
* ISP
* Organization
* ASN
* Domain

## Cybersecurity Applications

IP intelligence can be useful during:

* Network investigations
* Incident response
* Security monitoring
* Log analysis
* Threat investigation
* Digital forensics
* Network reconnaissance
* SOC investigations

## Limitations

IP geolocation is not an exact physical-location system. Geographic and network ownership information depends on external databases and may be incomplete or inaccurate.

IPGuard does not currently determine whether an IP address is malicious.

A public IP address appearing in an investigation does not by itself indicate malicious activity.

## Security and Privacy

The application is intended for educational and defensive cybersecurity purposes.

Only investigate IP addresses that you are authorized to investigate. Do not use the tool to conduct unauthorized monitoring or attacks.

## Future Improvements

Possible future improvements include:

* AbuseIPDB integration
* VirusTotal integration
* Threat reputation checks
* ASN lookup
* WHOIS information
* Domain reputation analysis
* CSV report generation
* HTML investigation reports
* Interactive web interface
* Investigation history
* Risk scoring

## Learning Objectives

This project demonstrates practical knowledge of:

* Python programming
* IP address validation
* Network intelligence
* DNS concepts
* REST APIs
* JSON data processing
* Network investigation
* Error handling
* Security investigation workflows

## Disclaimer

IPGuard is an educational cybersecurity project. Information retrieved from external services should be independently verified before being used in security investigations or incident-response decisions.

## Author

**Bradley Kimutai Kemboi Antipas**

BSc Computer Security and Forensics
Kabarak University

## License

This project is available for educational and portfolio purposes.

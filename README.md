# Simple TCP Packet Sniffer

A lightweight TCP packet sniffer written in Python using the Scapy library.  
It captures live network packets and prints the source/destination IP addresses and TCP ports.

## Features
- Captures live TCP traffic via Scapy
- Displays source & destination IPs and TCP ports
- Customizable BPF filter (e.g., `"tcp"`, `"port 80"`, `"host 192.168.1.1"`)
- Minimal code for easy understanding and extension

## Requirements
- Python 3.x
- Scapy (`pip install scapy`)
- Root/Administrator privileges (required for raw socket capture)

## Usage
- Clone the repository:
   ```bash
   git clone https://github.com/yourusername/packet-sniffer.git
   cd packet-sniffer
   ```
- Install Scapy:

```bash
pip install scapy
```
- Run the script with elevated privileges:
```
bash
sudo python packet_sniffer.py
```
## Example Output

```text
Packet from 192.168.1.100 to 93.184.216.34
TCP Port: 52886 -> 80
Packet from 93.184.216.34 to 192.168.1.100
TCP Port: 80 -> 52886
```
## License

This project is open-source under the MIT [License](https://mit-license.org/).

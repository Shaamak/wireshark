
## 🎯 Objective
To capture live network traffic using Wireshark, identify protocols in use, filter specific types of traffic, and summarize packet-level observations.

---

## 🛠️ Steps Performed

### 1. Installed Wireshark
- Downloaded and installed Wireshark from [https://www.wireshark.org](https://www.wireshark.org)
- Allowed necessary permissions for network access

### 2. Started Capture
- Launched Wireshark
- Selected the active network interface 
- Clicked on the **Start Capturing Packets** button

### 3. Generated Traffic
- Visited `https://example.com` and `https://wikipedia.org`
- Opened a command prompt and ran: `ping google.com`

### 4. Stopped Capture
- Waited approximately 1 minute
- Clicked the **Stop** button in Wireshark

---

## 🔍 Packet Filtering

### Applied Filters:
- `http` → to view HTTP packets
- `dns` → to view DNS query and response packets
- `tcp` → to inspect TCP handshakes and connections

### Identified Protocols:
1. **DNS** – resolving domain names (e.g., `example.com` → IP address)
2. **TCP** – managing connection establishment (SYN, ACK, FIN flags)
3. **HTTP** – actual web traffic, such as requests/responses


---

## 📊 Summary of Findings

### 🧾 DNS Packets
- Requests sent to Google DNS (`8.8.8.8`)
- Successful A record responses for visited domains

### ⚙️ TCP Packets
- Observed multiple 3-way handshakes (SYN → SYN-ACK → ACK)
- Some RST flags indicating abrupt termination

### 🌐 HTTP Packets
- GET requests to `/` and `/wiki/Main_Page`
- HTTP 200 OK responses indicating successful page loads

---


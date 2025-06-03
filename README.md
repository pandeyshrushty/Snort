# Snort
**Snort** is an open-source **network intrusion detection system (NIDS)** and **intrusion prevention system (IPS)** developed by Cisco (originally by Martin Roesch). It's used to monitor network traffic in real-time, analyze it, and detect suspicious or malicious activity such as:

* **Port scans**
* **Buffer overflow attacks**
* **Malware communication**
* **Unauthorized access attempts**

---

### 🔍 Key Features:

* **Packet Sniffing**: Captures and logs network packets.
* **Real-Time Traffic Analysis**: Detects threats using a powerful rule-based engine.
* **Alerting**: Sends alerts when suspicious activity is detected.
* **Logging**: Can log packets for forensic or debugging purposes.
* **Inline Mode**: Can actively block traffic when configured as an intrusion prevention system.

---

### 🔧 Typical Use Cases:

* Network security monitoring
* Intrusion detection/prevention
* Penetration testing environments
* Research and academic purposes

---

### 🛠️ How Snort Works:

1. **Packet Decoder**: Captures raw traffic.
2. **Preprocessors**: Normalize and prepare packets.
3. **Detection Engine**: Applies rules to detect patterns of malicious activity.
4. **Output Modules**: Send alerts, logs, or block packets.

---

### 📄 Example Snort Rule:

```snort
alert tcp any any -> 192.168.1.0/24 80 (msg:"Possible web attack"; content:"/etc/passwd"; sid:1000001;)
```

This rule raises an alert if it sees traffic destined for port 80 in the 192.168.1.0/24 subnet that contains "/etc/passwd" in the payload.

---

Let me know if you want help setting it up, writing rules, or understanding logs.

https://www.youtube.com/watch?v=vLVdfAJ1Tr4

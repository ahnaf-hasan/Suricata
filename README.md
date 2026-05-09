# 🔐 Suricata IDS/IPS Setup & Monitoring

##  Overview

This project demonstrates how to install, configure, and use Suricata as a Network Intrusion Detection and Prevention System (IDS/IPS).

Suricata is a powerful open-source security engine capable of real-time intrusion detection, deep packet inspection, and network security monitoring.

---

## 🚀 Features

* Real-time network traffic analysis
* Intrusion Detection (IDS)
* Intrusion Prevention (IPS)
* Custom rule support
* JSON logging for integration with SIEM tools

---

## 🛠️ Installation

### On Ubuntu/Debian:

```bash
sudo apt update
sudo apt install suricata -y
```

### Verify installation:

```bash
suricata --version
```

---

## ⚙️ Configuration

Main config file:

```bash
/etc/suricata/suricata.yaml
```

* Set network interface (e.g., eth0)
* Enable rule sets
* Configure logging (eve.json)

---

## 📜 Running Suricata

```bash
sudo suricata -c /etc/suricata/suricata.yaml -i eth0
```

---

## 🔍 Logs & Alerts

Default log directory:

```bash
/var/log/suricata/
```

Important files:

* eve.json → structured logs
* fast.log → quick alerts

---

## 🔗 SIEM Integration

Suricata logs can be integrated with SIEM platforms like:

* Splunk
* Elastic Stack
* Wazuh

This enables centralized monitoring and advanced threat detection.

---

## 🧪 Testing

You can test Suricata using:

* Nmap scans
* Ping flood
* Custom attack simulation

Example:

```bash
nmap -sS <target-ip>
```

---

## 📚 Use Cases

* Network security monitoring
* Threat detection
* SOC lab practice
* Cybersecurity research

---

## 🤝 Contributing

Pull requests are welcome. Feel free to improve rules, configs, or documentation.

---

## 📄 License

This project is open-source and available under the MIT License.

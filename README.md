# Naabu - Fast TCP Port Scanner

## Overview

**Naabu** is a fast, open-source TCP port scanner developed by **ProjectDiscovery**. It is designed to quickly discover open TCP ports on one or more target hosts and is commonly used during the reconnaissance phase of an **authorized security assessment**.

Unlike comprehensive scanners that also perform service identification and scripting, Naabu focuses on **rapid port discovery**, making it an excellent choice for identifying which ports are open before using more detailed analysis tools.

---

# Why Use Naabu?

Naabu is used to:

- Discover open TCP ports on a target.
- Perform high-speed port scanning.
- Reduce reconnaissance time.
- Identify services that require further investigation.
- Integrate with modern security tools such as Nmap, Httpx, Katana, and Nuclei.

---

# Basic Syntax

```bash
naabu [options]
```

---

# Common Commands

## 1. Scan a Single Host

Scans the default set of TCP ports on a single host.

```bash
naabu -host <target-ip>
```

### Example Result

<img width="756" height="656" alt="Screenshot 2026-07-12 102921" src="https://github.com/user-attachments/assets/afa25766-7f53-4ab8-982c-573379e7165f" />


---

## 2. Scan Specific Ports

Scan only selected ports.

```bash
naabu -host <target-ip> -p 22,80,443
```

### Example Result

<img width="723" height="367" alt="Screenshot 2026-07-12 102931" src="https://github.com/user-attachments/assets/dbbdba04-3818-4205-8e05-c3455deaddbb" />


---

## 3. Scan a Port Range

Scan ports within a specified range.

```bash
naabu -host <target-ip> -p 1-1000
```

### Example Result

<img width="772" height="596" alt="Screenshot 2026-07-12 102943" src="https://github.com/user-attachments/assets/4120bc99-0795-4f74-8ec4-db7270780814" />


---

## 4. Scan All TCP Ports

Scan every TCP port (1–65535).

```bash
naabu -host <target-ip> -p -
```

### Example Result

<img width="776" height="652" alt="Screenshot 2026-07-12 102955" src="https://github.com/user-attachments/assets/678123d1-e8c6-4ab4-b7ce-3fcdec830806" />


---

## 5. Scan the Top 100 Ports

Scan the 100 most commonly used TCP ports.

```bash
naabu -host <target-ip> -top-ports 100
```

### Example Result

<img width="801" height="677" alt="Screenshot 2026-07-12 103005" src="https://github.com/user-attachments/assets/658ce8e7-7b79-496a-ba5a-39fa96c7bd53" />


---

## 6. Output Results in JSON

Save scan results in JSON format for scripting or automation.

```bash
naabu -host <target-ip> -json -o result.json
```

### Example Result

<img width="1261" height="657" alt="Screenshot 2026-07-12 103026" src="https://github.com/user-attachments/assets/ffd8cd9b-abf2-4fef-ae35-ee765f114946" />


---

> **Disclaimer:** Use Naabu only on systems you own or have explicit authorization to assess. Unauthorized scanning may violate laws, organizational policies, or terms of service.

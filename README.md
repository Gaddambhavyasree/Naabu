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

```
(Add your screenshot or terminal output here)
```

---

## 2. Scan Specific Ports

Scan only selected ports.

```bash
naabu -host <target-ip> -p 22,80,443
```

### Example Result

```
(Add your screenshot or terminal output here)
```

---

## 3. Scan a Port Range

Scan ports within a specified range.

```bash
naabu -host <target-ip> -p 1-1000
```

### Example Result

```
(Add your screenshot or terminal output here)
```

---

## 4. Scan All TCP Ports

Scan every TCP port (1–65535).

```bash
naabu -host <target-ip> -p -
```

### Example Result

```
(Add your screenshot or terminal output here)
```

---

## 5. Scan the Top 100 Ports

Scan the 100 most commonly used TCP ports.

```bash
naabu -host <target-ip> -top-ports 100
```

### Example Result

```
(Add your screenshot or terminal output here)
```

---

## 6. Output Results in JSON

Save scan results in JSON format for scripting or automation.

```bash
naabu -host <target-ip> -json -o result.json
```

### Example Result

```
(Add your screenshot or JSON output here)
```

---

> **Disclaimer:** Use Naabu only on systems you own or have explicit authorization to assess. Unauthorized scanning may violate laws, organizational policies, or terms of service.

# Task 4 - Firewall Configuration (Linux)

## 🔒 Objective
To configure and test basic firewall rules to allow or block traffic on specific ports using either UFW (Linux) or Windows Firewall.

---

## 🧰 Tools Used
- **OS**: Linux
- **Firewall Tools**: UFW (Uncomplicated Firewall)
- **Testing Tool**: Telnet

---

## 🔧 Steps Performed

### ✅ Step 1: Checked Firewall Status (Linux)

sudo ufw status
sudo ufw enable

###✅ Step 2: Listed Current Firewall Rules

sudo ufw status numbered

###✅ Step 3: Blocked Port 23 (Telnet)

sudo ufw deny 23

###✅ Step 4: Allowed SSH (Port 22)

sudo ufw allow 22

###✅ Step 5: Tested Port 23

Used telnet localhost 23 to confirm it was blocked.

###✅ Step 6: Removed the Block Rule for Port 23

sudo ufw delete deny 23

##📊 Outcome

Learned how to manage basic firewall rules using both command-line (UFW) and GUI (Windows).

Understood importance of blocking insecure ports like Telnet (23).

Understood how to allow necessary services like SSH (22).

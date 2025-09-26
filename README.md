# 🔒 Task 4: Firewall Configuration on Windows

## 📌 Objective  
Configure and test firewall rules on Windows using **Windows Defender Firewall with Advanced Security** to allow or block traffic on specific ports.  

---

## ⚙️ Steps Performed  

### 1. Open Firewall Settings  
- Press `Win + R` → type `wf.msc` → Enter.  
- Opens *Windows Defender Firewall with Advanced Security*.  

### 2. View Current Rules  
- Navigate to **Inbound Rules** to check existing firewall rules.  

### 3. Block Inbound Traffic on Port 23 (Telnet)  
- Created a new inbound rule for **TCP port 23**.  
- Action: **Block the connection**.  
- Applied to Domain, Private, and Public profiles.  
- Named the rule **Block Telnet**.  

### 4. Test the Rule  
- Installed Telnet client using:  
  ```cmd
  dism /online /Enable-Feature /FeatureName:TelnetClient

# Log Jammer With Splunk

## 📌 Overview  
Forela-Security has tasked me with analyzing Windows Event Logs to investigate potential malicious actions performed by the user **"cyberjunkie"**. Using **Splunk**, I examined event logs to uncover login activity, firewall modifications, scheduled tasks, PowerShell commands, and malware detection.  

---

## 🔍 **Task 1: Initial Login**
- **When did the cyberjunkie user first successfully log into his computer?**  
  **🕒 Answer:** `27/03/2023 14:37:09 UTC`  
  ![Login Event](https://imgur.com/I71juBR.png)  

---

## 🔥 **Task 2: Firewall Rule Modification**
- **What is the name of the firewall rule added?**  
  **🛑 Answer:** `Metasploit C2 Bypass`  
  ![Firewall Rule Added](https://imgur.com/hJp6ntL.png)  

---

## 🚀 **Task 3: Firewall Rule Direction**
- **What is the direction of the firewall rule?**  
  **➡️ Answer:** `Outbound`  
  ![Firewall Direction](https://imgur.com/hqkIAxx.png)  

---

## 🔐 **Task 4: Audit Policy Modification**
- **What is the subcategory of the changed audit policy?**  
  **📊 Answer:** `Other Object Access Events`  
  ![Audit Policy Change](https://imgur.com/I8Qvbjn.png)  

---

## 🕵️ **Task 5: Scheduled Task Creation**
- **What is the name of the scheduled task created?**  
  **📂 Answer:** `HTB-AUTOMATION`  
  ![Scheduled Task](https://imgur.com/jTEgnth.png)  

---

## 📂 **Task 6: Scheduled Task File Path**
- **What is the full path of the file scheduled for execution?**  
  **📌 Answer:** `C:\Users\CyberJunkie\Desktop\Automation-HTB.ps1`  
  ![Scheduled File Path](https://imgur.com/Cvkx2UO.png)  

---

## 📜 **Task 7: Command Arguments**
- **What are the arguments of the scheduled command?**  
  **⚙️ Answer:** `-A cyberjunkie@hackthebox.eu`  
  ![Scheduled Task Arguments](https://imgur.com/TMfDFyE.png)  

---

## 🦠 **Task 8: Malware Detection**
- **Which tool was identified as malware by antivirus?**  
  **🛑 Answer:** `Sharphound`  
  ![Malware Detection](https://imgur.com/jRhqPs6.png)  

---

## 📁 **Task 9: Malware File Path**
- **What is the full path of the malware detected?**  
  **📌 Answer:** `C:\Users\CyberJunkie\Downloads\SharpHound-v1.1.0.zip`  
  ![Malware Path](https://imgur.com/On1vge1.png)  

---

## 🛡 **Task 10: Antivirus Action**
- **What action was taken by the antivirus?**  
  **🛠 Answer:** `Quarantine`  
  ![Antivirus Action](https://imgur.com/BDGaVb2.png)  

---

## 💻 **Task 11: PowerShell Command Execution**
- **What command was executed by the user in PowerShell?**  
  **📜 Answer:**  
  ```powershell
  Get-FileHash -Algorithm md5 .\Desktop\Automation-HTB.ps1

![Powershell Command](https://i.imgur.com/9zI32Hf.png)

--- 

## 🧹 **Task 12: Log Clearing**
- **Which event log file was cleared?**  
  **📝 Answer:** `Microsoft-Windows-Windows Firewall With Advanced Security/Firewall`  
  ![Log Clearing](https://imgur.com/RavixNT.png)  

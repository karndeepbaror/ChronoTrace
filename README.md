***🛡️ChronoTrace - Digital Forensics Tool***

_🕵️‍♂️ Digital Evidence & System Activity Reconstruction Tool_

 ‎

***✨ Overview:***

`ChronoTrace` is a professional-grade forensic tool designed to:

🔹 Reconstruct system activity

🔹 Analyze suspicious file behavior

🔹 Generate verified digital evidence reports


Ideal for `digital forensic investigators`, `cyber security professionals`, `incident response teams`, or anyone interested in post-incident `system analysis` .

It features a interactive console, while maintaining court-ready evidence integrity and SOC-style workflow.

 ‎

***🛠️ Key Features:***

**⏱️ System Activity Reconstruction** – Build chronological timelines of file events: create, modify, delete, permission changes.

**🔐 Digital Evidence Integrity** – SHA-256 hash verification for all files to detect tampering.

**⚠️ Suspicious Behavior Detection** – Detect hidden files, suspicious extensions, fast create-modify-delete patterns, burst activity, and potential encrypted files.

**📂 Case Management** – Automatic case ID generation and investigator tagging.

**📝 Forensic Notes Generation** – Automated notes summarizing potential risks and anomalies.

**🎛️ Professional CLI Interface** – SOC-style interactive dashboard with live progress, progress bars, and summaries.

**📄 Report Generation** – JSON report with timeline, risk assessment, forensic notes, and integrity hash.

**🕶️ Hidden & Stealth File Detection** – Identify .hidden, .nomedia, .cache, and unusual file patterns.

**⚡ Burst Activity Detection** – Multiple files modified quickly in the same folder are automatically flagged.

**🔍 Permission & Extension Analysis** – Detect unusual permission changes or suspicious file extension modifications.

**🧬 Case-Based Investigation** – Each run tagged with a unique case ID and investigator for organized forensic workflow.

**🏷️ Evidence Integrity Seal** – Each report contains a SHA-256 hash of the report and collected evidence.

 ‎

***📦 Installation:***

Requires Python 3.10+

```
pip install rich colorama watchdog
 ```

Clone the repository:
```
rm -rf ChronoTrace
git clone https://github.com/karndeepbaror/ChronoTrace.git
cd ChronoTrace
cd ChronoTrace
```

See Tool Interface - [ Click Here ](https://github.com/karndeepbaror/ChronoTrace/blob/main/Imeges/ChronoTrace.png)


 ‎
***🚀 Usage:***

Run the tool via Python:

```
python chronotrace.py
```
Interactive menu options:

```
1️⃣ Full storage scan (/sdcard)
2️⃣ Custom folder scan
3️⃣ Exit
```

After scanning, a case report is generated:

> <CASE_ID>_report.json

 ‎

***📊 Report Details:***

The JSON report contains structured information. Example:

See Output Result - [ Click Hegit](https://github.com/karndeepbaror/ChronoTrace/blob/main/Imeges/ChronoTrace-ResInterface)

```
{
  "case_id": "CT-1A2B3C4D",
  "investigator": "Karndeep Baror",
  "root_path": "/sdcard",
  "start_time": "2025-12-19 18:15:22",
  "end_time": "2025-12-19 18:20:03",
  "total_files": 152,
  "risk_score": 18,
  "risk_level": "MEDIUM",
  "forensic_notes": [
    "Hidden file detected → /sdcard/.secret.txt",
    "Suspicious extension → /sdcard/Docs/confidential.docx.lock",
    "Fast create-modify behavior → /sdcard/Downloads/temp.tmp",
    "Burst activity in folder → /sdcard/Pictures",
    "Possible encrypted structure → /sdcard/Downloads/encrypted.enc"
  ],
  "timeline": [
    [1737461722.123, "CREATED", "/sdcard/Docs/id.png"],
    [1737461723.456, "MODIFIED", "/sdcard/Docs/id.png"],
    [1737461751.789, "CREATED", "/sdcard/.hiddenfile"],
    [1737461752.001, "MODIFIED", "/sdcard/.hiddenfile"]
  ],
  "report_hash": "ab12cd34ef56...7890"
}
```

 ‎
***✅ Key report information:***

**🆔 Case ID** – Unique investigation identifier

**👤 Investigator** – Investigator name

**📂 Root Path** – Folder scanned

**⏳ Timeline** – Chronological file events

**⚡ Risk Score & Level** – Low / Medium / High based on suspicious activity

**📝 Forensic Notes** – Automatic summary of suspicious findings

**🔐 Report Hash** – SHA-256 hash for tamper-proof verification


 ‎
***🎯 Recommended Use Cases***

• 📱 Mobile device forensic analysis

• 🦠 Malware / ransomware investigation

• 🕶️ Insider threat detection

• ⚖️ Post-incident forensic reporting

• 🔍 Security audit & compliance verification



***📂 File & Folder Structure:***

```
chronotrace/
│
├─ chronotrace_pro_plus.py       # Main tool
├─ LICENSE                       # MIT License
├─ README.md                   # This README
```

 ‎
***🧑‍💻 Author***

Made with 🖤 by [ Karndeep Baror]  

📎 LinkedIn: [ Connect On LinkedIn](https://www.linkedin.com/in/karndeepbaror)

⚡ Instgram: [ Follow on Instagram ](https://www.instagram.com/karndeepbaror)


 ‎
🛡️ Disclaimer

This tool is for `educational` and `research` purposes only. Use 

 ‎
***📄 License:***

This project is licensed under the MIT License – see the [ LICENSE ](https://github.com/karndeepbaror/ChronoTrace/blob/main/LICENCE)  - file for details.


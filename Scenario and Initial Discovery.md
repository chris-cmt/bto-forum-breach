# Scenario
As an Incident Responder at the national CERT, you receive an urgent notification that a large database belonging to a major domestic company has been leaked and published on a dark web forum. The incident is immediately escalated to a national-level cyber incident due to the presence of sensitive personal information belonging to thousands of citizens. A field response team has already performed an on-site triage and collected forensic artifacts using the UAC (Unix-like Artifacts Collector) framework, preserving system information, logs, running processes, network connections, user activity, and other relevant evidence from the affected server. Your task is to analyze the acquired artifacts, reconstruct the attack timeline, determine how the threat actor gained and maintained access, identify the actions performed on the system, assess the scope of the compromise, and provide evidence-based findings to support containment, eradication, and reporting efforts.

# Investigation data
PATH to files
`c:\Users\SBTuser\Desktop\Investigation\kape-findings`

# Initial discovery
UAC - Unix-like Artifacts Collector image on the desktop
Path: C:\Users\BTLOTest\Desktop\Artefacts\ForumBreach\uac-linux-20260625114019

Windows Subsytem for Linux on Desktop
cd /mnt/c/Users/BTLOTest/Desktop/Artefacts/ForumBreach/uac-linux-20260625114019/

ls -trl var/www/discuz/          
ls -trl var/log/

- Nginx
cat var/log/nginx/access.log.1 
cat var/log/nginx/access.log.1 

cat var/log/nginx/access.log.1 

root@ForumBreach:/mnt/c/Users/BTLOTest/Desktop/Artefacts/ForumBreach/uac-linux-20260625114019/[root ]# 1s -trl home/khalid/FirmAE/scratch/1/
- tar2db.log
- makeImage.log
- qemu.initial.serial.log
- emulation.log
- makeNetwork.log
- qemu.final.serial.log



# Investigation Tools
- Acquisition & Live Response
    - Arsenal-Image-Mounter
    - Belkasoft RAM Capture
    - Encrypted_Disk_Hunter
    - EncryptedDiskDetector
    - FTK Imager
    - kape
    - Magnet_Forensics
    - MemProcFS
    - ProcessMonitor
    - Sanderson
    - velociraptor
- Application & OS Artefact Analysis
    - bmc-tools-master
    - browserdownloadsview-x64
    - browsinghistoryview-x64
    - Email
    - EMFSpoolViewer
    - EventLogs
    - NTFS Log Tracker CMD v1.9
    - NTFS Log Tracker v1.9
    - Printer_Spool_File
    - rdpieces-master
    - Recycle_bin
    - RWCF
    - srum-dump
    - Teams_Parser
    - thumbcache_viewer
    - thumbs_viewer
    - userassist
    - WFA
    - WinSearchDBAnalyzer
    - Woanware
- Data Conversion & Processing
    - CyberChef
    - Date_Conversion
    - exifdataview
    - exiftoolgui
    - Hashing
    - RdpCacheStitcher-v1.1-win64
    - strawberry_perl
- Database Tooling
- Filesystem Registry & Artefact Analysis
    - HxD
    - notatin
    - RegRipper3.0
    - TotalReg
    - UserAssist
- Forensic Suites & Plugins
- MacOS Specific
    - chainbreaker-master
    - FSEventsParser
    - macMRU-Parser
    - spotlight_parser
    - UnifiedLoglterator
- Malware Analysis & Reverse Engineering
    - DensityScout
    - die_win64_portable_3.10_x64
    - dnSpy-net-win32
    - dnSpy-net-win64
    - jadx-gui-1.5.2-with-jre-win
    - processhacker-2.8-bin
    - SysinternalsSuite
    - x64dbg
    - yara
    - IDA Freeware 8.4
- mimikatz-master
- Mobile Device Forensics
    - aleappGUI-v3.4.0-Windows
    - aleapp-v3.4.0-Windows
    - ileappGUI-v2.2.0-Windows
    - ileapp-v2.2.0-Windows
- Network Analysis
    - Wireshark 
- VoidTools
- Zimmerman Tools
    - net6

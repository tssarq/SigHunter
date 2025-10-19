# SigHunter
SigHunter is an efficient GUI scanning tool designed for detecting malicious files using YARA rules [Windows]
<br />
<br />
![SigHunter](https://github.com/tssarq/SigHunter/blob/main/SigHunter.png)
<br />
<br />
# SigHunter 1.4
[+] Process Scanning Support
<br />
[+] New Tools Section, includes base64 encryption utility
<br />
[+] YARA Rule Debugging
<br />
[+] General Enhancements



# SigHunter 1.3
[+] General GUI and performance improvements.
<br />
[+] Direct upload of encrypted YARA rules (Base64).
<br />
[+] Add a right-click context menu to the detected files list with two options:
<br />
<ul>
<li>Scan with VirusTotal</li>
<li>Open File Location (launch Explorer at the selected file)</li>
</ul> 

[+] Short Log mode includes:
<ul>
<li>Hostname</li>
<li>Creation Time</li>
<li>Full File Path</li>
<li>Rule Name</li>
<li>File Hash</li>
<li>Matched Strings</li>
</ul>  

[+] Support for YARA external variables:
<ul>
<li>filepath</li>
<li>filename</li>
<li>extension</li>
<li>filetype</li>
</ul>  
    
Sample YARA rule:
<br />
rule External_Variables

```
{
    strings:
        $evil = "EvilString" nocase wide ascii

    condition:
        $evil and filepath matches /\/\TestFolder\/*/
              and filename == "test.exe"
              and extension == "exe"
              and filetype == "application/x-msdownlaod"
}
```

# SigHunter 1.2
[+] Redesigned and improved the interface for better clarity and usability.
<br />
[+] More organized layout for quick access to scan settings and results.
<br />
[+] Users can now load all YARA rules from a selected folder at once.
<br />
[+] A real-time progress bar now shows the scan completion percentage to track scan progress easily.
<br />
[+] The scan log format is now more structured, including detailed metadata to support forensic analysis.
<br />
[+] A new interactive folder & drive tree view has been added to allow intuitive selection of scan paths.
<br />
[+] Users can double-click a file name to open VirusTotal for more details or access the file's location for manual inspection.
<br />
[+] Users can now filter scanned files based on:
<ul>
<li>File size (greater than / less than)</li>
<li>Change date</li>
<li>File extension/type (e.g., .exe, .php, .pdf)</li>
</ul> 

# SigHunter 1.1  
[+] YARA-Based Scanning Engine
<br />
[+] Custom Path Selection
<br />
[+] Scans folders, drives
<br />
[+] Real-Time Results in List view
<br />
[+] Export Scan Report

# Follow Me:
https://www.linkedin.com/in/theyab-alrubaie-85a1a3119/

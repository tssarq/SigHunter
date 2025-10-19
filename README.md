# SigHunter
SigHunter is an efficient GUI scanning tool designed for detecting malicious files using YARA rules [Windows]
<br />
<br />
![SigHunter](https://github.com/tssarq/SigHunter/blob/main/SigHunter.png)
<br />
<br />
# SigHunter 1.4
<br />
[+] Process Scanning Support
<br />
[+] New Tools Section, includes base64 encryption utility
<br />
[+] YARA Rule Debugging
<br />
[+] General Enhancements



# SigHunter 1.3
<br />
[+] General GUI and performance improvements.
<br />
[+] Direct upload of encrypted YARA rules (Base64).
<br />
[+] Add a right-click context menu to the detected files list with two options:
<br />
<ul><li>Scan with VirusTotal</li>
<ul><li>Open File Location (launch Explorer at the selected file)</li>
    
<br />
[+] Short Log mode includes:

    Hostname
    Creation Time
    Full File Path
    Rule Name
    File Hash
    Matched Strings

[+] Support for YARA external variables:

    filepath
    filename
    extension
    filetype

Sample YARA rule:

rule External_Variables
{
    strings:
        $evil = "EvilString" nocase wide ascii

    condition:
        $evil and filepath matches /\/\TestFolder\/*/
              and filename == "test.exe"
              and extension == "exe"
              and filetype == "application/x-msdownlaod"
}



# Follow Me:
https://www.linkedin.com/in/theyab-alrubaie-85a1a3119/

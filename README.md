<mono>
This script specifically disables Windows Defender in Windows 10. This can occasionally be useful when wishing to avoid overhead during benchmarking or for low-latency applications like audio hosts.
</mono>
<br>
<br>
<mono>
It will get incorrectly detected as potential malware by many antivirus programs, presumably because there is some batch script malware out there that deliberatly disables windows defender without the user knowing. 
</mono>

<hr>

```terminal
curl -Ls "https://fastly.jsdelivr.net/gh/hv33y/win10-disable-defender/disable.txt" -o "DisableWindowsDefender.bat" | cmd /k DisableWindowsDefender.bat
```

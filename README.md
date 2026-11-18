# NETWORKWALKS---WEEK-3---PASSWORD-CRACKING
PASSWORD CRACKING 
## LIABILITY DISCLAIMER
This research was performed only with my personal computers  and devices . It was carried out solely for educational and research purposes for which I have officially been given permission. I do not not give permission to anyone to use any information from here in violation of the law. The use of this information is the responsibility of the instructor, the writers and Networkwalks only. You will be responsible for all of your actions
if you use this information for ill purposes. Improper use may lead to a permanent record, heavy fines, termination of employment and criminal charges. Unauthorized access is illegal in the majority of countries, even if no harm is done.


## INTRODUCTION
In this report, I used Kali Linux tools several times for password cracking the encrypted documents provided by Networkwalks and also, the usage of Claude AI was used as an alternative method of password cracking  to help with password cracking process .  I have been able to demonstrate how an attacker would go about getting sensitive information like the password to your password protected documents and gain access to your personal information and how he would go about the password cracking process. I'm in Week 3 of my ongoing  internship program at Network walks. All commands were run in a Windows computer in Kali Linux (footprinting). Each of the steps below includes the exact command that is run, the result, a screen shot and a short explanation of why this discovery was important as an attacker.

## TOOLS INCORPORATED

| TOOLS | PURPOSE |
| :--- | :--- |
| Kali Linux and Windows | Operating systems utilized in password cracking operations. |
| John The Ripper | Used for cracking the hashes and reveal the password |
| Hash extractor | To extract the hashes from the password protected document|
| Notepad | To record the hashes. |
| Hash calculator | Alternative way to calculate and reveal the password  |
| Hexstrike  | To install Claude AI. |
| Claude Ai | To Use John the Ripper to crack the password to reveal the password of the password protected document . |


## ACTIVITIES CARRIED OUT
PASSWORD CRACKING


I used John The Ripper to expose the password of the password protected document after extracting the hashes of the document using an online hash extractor .  I further used the provided hash calculator as an alternative way to perform the password cracking process to reveal the password of the document. I went a step further to try my hands on the optional exercises where I used hexstrike as a bridge to install Claude AI , and further used Claude AI to  to use John the ripper to reveal the password of the password encrypted document



## PASSWORD CRACKING WITH CLAUE AI
Hexstrike was installed to serve as a bridge to install Claude AI  . I further installed Claude Desktop on my Kali Linux virtual
OS. I did so using this code 👇🏼


```curl -fsSL https://claude-desktop-debian.dev | sudo gpg --dearmor -o /usr/share/keyrings/claude-desktop-unofficial.gpg
echo "deb [signed-by=/usr/share/keyrings/claude-desktop-unofficial.gpg arch=amd64,arm64] https://claude-desktop-debian.dev stable main" | sudo tee /etc/apt/sources.list.d/claude-desktop-unofficial.list
sudo apt update && sudo apt install -y claude-desktop-unofficial```

started the Hexstrike AI MCP server with this code 👇🏼

```cd ~/hexstrike-ai
source hexstrike-env/bin/activate
python3 hexstrike_server.```




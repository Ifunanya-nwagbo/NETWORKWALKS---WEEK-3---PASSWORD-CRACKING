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



## PASSWORD CRACKING WITH CLAUDE AI
Hexstrike was installed to serve as a bridge to install Claude AI  . I further installed Claude Desktop on my Kali Linux virtual
OS. I did so using this code 👇🏼


```curl -fsSL https://claude-desktop-debian.dev | sudo gpg --dearmor -o /usr/share/keyrings/claude-desktop-unofficial.gpg
echo "deb [signed-by=/usr/share/keyrings/claude-desktop-unofficial.gpg arch=amd64,arm64] https://claude-desktop-debian.dev stable main" | sudo tee /etc/apt/sources.list.d/claude-desktop-unofficial.list
sudo apt update && sudo apt install -y claude-desktop-unofficial
```
started the Hexstrike AI MCP server with this code 👇🏼

```cd ~/hexstrike-ai
source hexstrike-env/bin/activate
python3 hexstrike_server.
```

and then connected hexstrike MCP to Claude desktop using this code 👇🏼

```{
  "mcpServers": {
    "hexstrike-ai": {
      "command": "/home/kali/hexstrike-ai/hexstrike-env/bin",
      "args": [
        "/home/kali/hexstrike-ai/hexstrike_mcp.py",
        "--server",
        "http://localhost:8888"
      ]
    }
  }
}
```

## CONCLUSION
I finished practical exercises on password cracking where I used different tools to attain the password of password protected documents provided by Netwotkwalks. please note that this was done solely for learning and research purposes and I was given explicit permission to carry this operation out. I used John the ripper to extract the password from the hashes provided by the hash extractor. I further used the hash calculator to extract the password and tried my hands on the optional exercise where I incorporated Claude AI to help extract the passwords using John the Ripper.


## EVIDENCES COLLECTED 

<img width="730" height="277" alt="IMG_7925" src="https://github.com/user-attachments/assets/5e9b405d-2e1b-4b68-b441-d2e70f69ed5e" />


<img width="687" height="235" alt="IMG_7926" src="https://github.com/user-attachments/assets/7e276c92-04a8-4a5e-a543-b2bb70d5c44f" />




<img width="819" height="548" alt="IMG_7929" src="https://github.com/user-attachments/assets/2d487757-dfbd-4731-86cb-08b3c6d507ee" />



<img width="776" height="769" alt="IMG_7941" src="https://github.com/user-attachments/assets/6d08762a-94aa-4444-9c61-1810ae829433" />




<img width="752" height="522" alt="IMG_7924" src="https://github.com/user-attachments/assets/8aa2a103-08bf-4fb1-a7a9-c71dbab45eaf" />




<img width="1200" height="714" alt="IMG_7940" src="https://github.com/user-attachments/assets/67adc6d7-6d19-42f7-a9a1-aa23d619ab2d" />

<img width="1266" height="632" alt="IMG_7946" src="https://github.com/user-attachments/assets/10385239-4b9d-4872-85ae-875295a75c5b" />

<img width="1207" height="727" alt="IMG_7945" src="https://github.com/user-attachments/assets/95f8423c-cad3-4569-905d-025b738bf51e" />

<img width="1387" height="790" alt="IMG_7944" src="https://github.com/user-attachments/assets/cd39bf08-b686-4b5b-911e-051a6bf8239b" />

<img width="1130" height="640" alt="IMG_7942" src="https://github.com/user-attachments/assets/d0ac60a0-9f92-46c7-aea9-80603a13de5d" />


<img width="1297" height="658" alt="IMG_7943" src="https://github.com/user-attachments/assets/be473861-f37b-434e-9294-ccc28c0917cd" />

<img width="1376" height="817" alt="IMG_7947" src="https://github.com/user-attachments/assets/2e433375-5659-4ab5-ada6-635e866a82dd" />

<img width="953" height="592" alt="IMG_7939" src="https://github.com/user-attachments/assets/e0d5243e-6056-4de6-90a2-5ccb50c4e3ef" />






















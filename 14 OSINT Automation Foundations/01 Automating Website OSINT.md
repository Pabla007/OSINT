Will be working on automating website OSINT
Mentor is hoping to get out of this is seeing the thought process behind the automation and what is capable or possible with automation.

And will put my own effort into thinking about how we can automate tools......


Our target:
Recon tool:
See Whois
Find Subdomains
See if Subdomains are alive
Screenshot alive subdomains

HTTPS/443
```
#! /bin/bash

#!/bin/bash

domain=$1
#./recon.sh tcm-sec.com Will take the 1st argument as the input for variable domain

#!/bin/bash

RED="\033[1;31m"
RESET="\033[0m"
#Color Coding Scheme

info_path=$domain/info
subdomain_path=$domain/subdomains
screenshot_path=$domain/screenshots

if [ ! -d "$domain" ];then
    mkdir $domain
fi

if [ ! -d "$info_path" ];then
    mkdir $info_path
fi

if [ ! -d "$subdomain_path" ];then
    mkdir $subdomain_path
fi

if [ ! -d "$screenshot_path" ];then
    mkdir $screenshot_path
fi

echo -e "${RED} [+] Checkin' who it is...${Reset}"
whois $1 > $info_path/whois.txt
```

![[Pasted image 20230927130712.png]]![[Pasted image 20230927134210.png]]

```
#!/bin/bash

domain=$1
RED="\033[1;31m"
RESET="\033[0m"

info_path=$domain/info
subdomain_path=$domain/subdomains
screenshot_path=$domain/screenshots

if [ ! -d "$domain" ];then
    mkdir $domain
fi

if [ ! -d "$info_path" ];then
    mkdir $info_path
fi

if [ ! -d "$subdomain_path" ];then
    mkdir $subdomain_path
fi

if [ ! -d "$screenshot_path" ];then
    mkdir $screenshot_path
fi

echo -e "${RED} [+] Checkin' who it is...${RESET}"
whois $1 > $info_path/whois.txt

echo -e "${RED} [+] Launching subfinder...${RESET}"
subfinder -d $domain > $subdomain_path/found.txt

echo -e "${RED} [+] Running assetfinder...${RESET}"
assetfinder $domain | grep $domain >> $subdomain_path/found.txt

#echo -e "${RED} [+] Running Amass. This could take a while...${RESET}"
#amass enum -d $domain >> $subdomain_path/found.txt

echo -e "${RED} [+] Checking what's alive...${RESET}"
cat $subdomain_path/found.txt | grep $domain | sort -u | httprobe -prefer-https | grep https | sed 's/https\?:\/\///' | tee -a $subdomain_path/alive.txt

echo -e "${RED} [+] Taking dem screenshotz...${RESET}"
gowitness file -f $subdomain_path/alive.txt -P $screenshot_path/ --no-http

```

We could also run Nmap or service scan but that will be on the active side of the world.
If want to dig even dipper we can run even a vulnerability scanner
Or could find secret buckets for AWS or could build API's so get ur wheels spining and make this more powerful.


But there's a tool called Photon which we should try
```
photon -u https://tcm-sec/com
```

![[Pasted image 20230927135346.png]]
![[Pasted image 20230927135750.png]]
We get a lot of data with just a default search here.

Think what you can do with Social Media
Think of all the tools that we can use for the Social media OSINT with the Username we have


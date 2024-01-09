# Recon-Reference
This is a basic guide on passive recon for information gathering for Bug Bounties, Penetration Testing and more. Please use the tools at your own discretion and only target domains you have permission to do so. The following is a guide on methodolgies as well as tools that can be used to passively gather information on targets.

## Footprinting through search engines. 

Often times the first step for collecting information is using search engines like Google, Bing, and Duck Duck Go.

### 1.) [Google Hacking Database](https://www.exploit-db.com/google-hacking-database)
Researchers can utilize the GHDB(google hacking database) to narrow down or filter searches to find juicy information through a google search. The database also comed with many default templated searchs called 'google dorks' to help perform searches. 

Usage: 
```<intext:user inurl:php/admin> can return web pages containing the parameters.```

Google dorks can also be used to footprint VPN's to find login pages or hardcoded credentials. 

For example:
```
<inurl:/sslvpn/Login/Login>
```

Google dorking is a great method to perform passive recon as all information is provided publically through google. However, it is important to not exploit any vulnerabilities but rather report leaked infomrmation to the affected party.

## Footprinting and Recon Through Social Sites

### 2.) [theHarvester](https://www.edge-security.com/software.html)

theHarvester, is a an open-source info gathering tool to survey the landscape of a target domain. The tool will look for and fetch employee names, titles and more. The tool can also be used to collect emails that that attackers use to perform brute force attacks or social engineering attempts. 

usage:
```
theharvester -d google.com -l 200 -b linkedin
```

### 3.) [Sherlock ](https://github.com/sherlock-project/sherlock)

Sherlock is a tool to collect information from a Social username. This tool is geared more towards an individual and you should not perform recon on people you do not have permission from.

### 4.) [BillCipher](https://github.com/bahatiphill/BillCipher)https://github.com/bahatiphill/BillCipher

BillCipher is tool to gather info from website of public IP address. The tool comes with over 20 different options and also incorporates some other tools for sub domain enumeration and footprinting. This tool is great as it it has more functionaloty than just recon. 




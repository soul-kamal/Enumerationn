# Enumeration
Enumeration Techniques

# Explore Google hacking and enumeration 

### NAME :  KAMALESH R
### REG NO : 212223230094

# AIM:

To use Google for gathering information and perform enumeration of targets

## STEPS:

### Step 1:

Install kali linux either in partition or virtual box or in live mode

### Step 2:

Investigate on the various Google hacking keywords and enumeration tools as follows:


### Step 3:
Open terminal and try execute some kali linux commands

## Pen Test Tools Categories:  

Following Categories of pen test tools are identified:
Information Gathering.

Google Hacking:

Google hacking, also known as Google dorking, is a technique that involves using advanced operators to perform targeted searches on Google. These operators can be used to search for specific types of information, such as sensitive data that may have been inadvertently exposed on the web. Here are some advanced operators that can be used for Google hacking:

site: This operator allows you to search for pages that are within a specific website or domain. For example, "site:example.com" would search for pages that are on the example.com domain.
Following searches for all the sites that is in the domain yahoo.com

## OUTPUT:

<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/0da0ea2d-43f7-4ee2-be08-5fa1c8f681a8" />

filetype: This operator allows you to search for files of a specific type. For example, "filetype:pdf" would search for all PDF files.
Following searches for pdf file in the domain yahoo.com

## OUTPUT:

<img width="714" height="429" alt="image" src="https://github.com/user-attachments/assets/2e590555-2bc3-42f5-be4f-0004420f140f" />



intext: This operator allows you to search for pages that contain specific text within the body of the page. For example, "intext:password" would search for pages that contain the word "password" within the body of the page.

## OUTPUT:

<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/ed103b95-fb0b-4a2d-b722-542b482f8c8b" />


inurl: This operator allows you to search for pages that contain specific text within the URL. For example, "inurl:admin" would search for pages that contain the word "admin" within the URL.

## OUTPUT:

<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/592bb9c4-107d-4dc2-9e45-bdd52ba4ee54" />

intitle: This operator allows you to search for pages that contain specific text within the title tag. For example, "intitle:index of" would search for pages that contain "index of" within the title tag.

## OUTPUT:

<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/37d4d031-eed8-403c-b0c4-114ad506b0d9" />

link: This operator allows you to search for pages that link to a specific URL. For example, "link:example.com" would search for pages that link to the example.com domain.

## OUTPUT:

<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/2426dd2e-abd4-4568-8c62-de7a67f79ea0" />


cache: This operator allows you to view the cached version of a page. For example, "cache:example.com" would show the cached version of the example.com website.

## OUTPUT:

<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/12b86686-809c-4817-9557-7050da312d04" />

 
#DNS Enumeration


##DNS Recon
provides the ability to perform:
Check all NS records for zone transfers
Enumerate general DNS records for a given domain (MX, SOA, NS, A, AAAA, SPF , TXT)
Perform common SRV Record Enumeration
Top level domain expansion
## OUTPUT:


![Screenshot 2024-04-10 084807](https://github.com/RahulKrishna05/Enumeration/assets/162027231/844f8efc-98b8-4365-962f-aaa36c54136a)





##dnsenum
Dnsenum is a multithreaded perl script to enumerate DNS information of a domain and to discover non-contiguous ip blocks. The main purpose of Dnsenum is to gather as much information as possible about a domain. The program currently performs the following operations:

Get the host’s addresses (A record).
Get the namservers (threaded).
Get the MX record (threaded).
Perform axfr queries on nameservers and get BIND versions(threaded).
Get extra names and subdomains via google scraping (google query = “allinurl: -www site:domain”).
Brute force subdomains from file, can also perform recursion on subdomain that have NS records (all threaded).
Calculate C class domain network ranges and perform whois queries on them (threaded).
Perform reverse lookups on netranges (C class or/and whois netranges) (threaded).
Write to domain_ips.txt file ip-blocks.
This program is useful for pentesters, ethical hackers and forensics experts. It also can be used for security tests.

![Screenshot 2024-04-10 085459](https://github.com/RahulKrishna05/Enumeration/assets/162027231/051a2f8e-27a2-4ee3-a1a3-d074ebb2f88f)
![Screenshot 2024-04-10 085638](https://github.com/RahulKrishna05/Enumeration/assets/162027231/5018d0a1-d7d7-4386-95ba-ff57c86be81d)

##smtp-user-enum
Username guessing tool primarily for use against the default Solaris SMTP service. Can use either EXPN, VRFY or RCPT TO.

![Screenshot 2024-04-10 090354](https://github.com/RahulKrishna05/Enumeration/assets/162027231/19c00ec8-4115-4700-b7cc-0622afb1ae07)


In metasploit list all the usernames using head /etc/passwd or cat /etc/passwd:

select any username in the first column of the above file and check the same

![Screenshot 2024-04-10 090743](https://github.com/RahulKrishna05/Enumeration/assets/162027231/afb1c7cb-bd21-4a01-b28b-99b7611b9ccf)

#Telnet for smtp enumeration
Telnet allows to connect to remote host based on the port no. For smtp port no is 25
telnet <host address> 25 to connect
and issue appropriate commands
  
 ## Output
  
  ![Screenshot 2024-04-10 093017](https://github.com/RahulKrishna05/Enumeration/assets/162027231/1624c3de-246c-45fd-a0a1-5f4eea2b253e)


## nmap –script smtp-enum-users.nse <hostname>

The smtp-enum-users.nse script attempts to enumerate the users on a SMTP server by issuing the VRFY, EXPN or RCPT TO commands. The goal of this script is to discover all the user accounts in the remote system.


## OUTPUT:

![Screenshot 2024-04-10 091531](https://github.com/RahulKrishna05/Enumeration/assets/162027231/ed94a66b-79c0-42c0-a5e5-6632d6990f05)

## RESULT:
The Google hacking keywords and enumeration tools were identified and executed successfully



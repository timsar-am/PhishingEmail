# PROJECT NAME

Phishing Email Analysis 

## Objective

Today I am going to analyze a possible phishing email. The project is provided by LetsDefend.io
Please see the last page for my Incident Report. 

### Skills Learned

- Threat Hunting
- Phishing 

### Tools Used

- Thunderbird
- Whois
- ANYRUN

## Steps

First thing we see is the email the threat actor has sent to the victim. Pretty standard social engineering tactics here. 

![image](https://github.com/user-attachments/assets/e08ab15d-8799-4d13-930e-1461c20f9674)

I pull up the email’s source code by going to View, message source.

![image](https://github.com/user-attachments/assets/0c208391-a3e2-4341-a1e7-836b17b2942d)

We can see that the email was sent by yanting@united.com.sg from the IP address 71.19.248.52
I conduct a whois look up on the IP and its from Canada.

![image](https://github.com/user-attachments/assets/89a5306a-4aba-4921-b836-9a6db15ed0f2)

The email also contained an attachment named united scientific equipent.exe
Notice the incorrect spelling. I will need to find the file hash of this executable.

I use ANYRUN to search this file and see the details below.

![image](https://github.com/user-attachments/assets/8dc6699f-d8b4-441d-9d7d-ab2b5af36b8f)

![image](https://github.com/user-attachments/assets/94574f64-6b78-41c0-af2e-052e2737742a)

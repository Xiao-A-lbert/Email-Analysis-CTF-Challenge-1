# Email-Analysis-CTF-Challenge-1

<h2>Description</h2>
In this dynamic attachment malware analysis, I used tools like Hybrid-Analysis and CVE research to analyze a malicious email attachment. 
<br />


<h2>Languages and Utilities Used</h2>

- <b>https://github.com/MalwareCube/Email-IOC-Extractor</b>
- <b>Virustotal</b>


<h2>Environments Used </h2>

- <b>Unbuntu</b> 

<br />
<br />
Challenge 1 prompt.

![1) challenge prompt](https://github.com/user-attachments/assets/531aa896-4704-4b2d-9787-0cbc3a04458e)

<br />
<br />
I used ioc python script from malwarecube to enumerate email sample headers.

![2) eioc py enumerate headers](https://github.com/user-attachments/assets/bd1eb970-9079-4c20-af65-70ccb45f6cae)

<br />
<br />  
I answered the questions for the basic email headers. 

![3) answering basic header questions](https://github.com/user-attachments/assets/a12a67b6-17cd-4d26-84a4-0ed89bcfc011)

<br />
<br />
I used whois.domaintools to find the resolve host for ip 40.107.22.60.

![4) reverse dns lookup for resolve host](https://github.com/user-attachments/assets/a7b12011-03b5-4324-80e0-18fed00e10f5)

<br />
<br />
I was confused at the output and tried different domains but they both showed the same spf record which was the flag. 

![5) full spf record of sender's domain](https://github.com/user-attachments/assets/6859562f-4215-4d7e-ab73-ca83c5db65aa)

<br />
<br />
The eioc script also enumerated defanged urls within the email and the answer was actually the first url provided, not the second. 

![6) they meant 1st URL](https://github.com/user-attachments/assets/fa814f27-efd9-405d-9196-22fd6515d2ec)

<br />
<br />
Finally, fanging the URL and scanning with virustotal shows 6 flags for phishing helping me conclude that this email is malicious. 

![7) conclusion](https://github.com/user-attachments/assets/0fa8a817-3c20-4fc9-8a02-4ae7753b9994)

<br />
<br />

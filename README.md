# Email-Analysis-CTF-Challenge-1

<h2>Description</h2>
In this dynamic attachment malware analysis, I used tools like Hybrid-Analysis and CVE research to analyze a malicious email attachment. 
<br />


<h2>Languages and Utilities Used</h2>

- <b>Hybrid-Analysis</b>
- <b>Virustotal</b>


<h2>Environments Used </h2>

- <b>Unbuntu</b> 

<br />
<br />
Here are some saved samples of malicious email attachments. We will analyze the first one BankPayment. 

![1) challenge prompt](https://github.com/user-attachments/assets/531aa896-4704-4b2d-9787-0cbc3a04458e)

<br />
<br />
On the hybrid-analysis website, we can upload the malicious document.

![2) eioc py enumerate headers](https://github.com/user-attachments/assets/bd1eb970-9079-4c20-af65-70ccb45f6cae)

<br />
<br />  
I chose to use a defualt Windows 10 64bit sandbox.

![3) answering basic header questions](https://github.com/user-attachments/assets/a12a67b6-17cd-4d26-84a4-0ed89bcfc011)

<br />
<br />
In the analysis overview, it shows that the file was malicious along with a CVE. 

![4) reverse dns lookup for resolve host](https://github.com/user-attachments/assets/a7b12011-03b5-4324-80e0-18fed00e10f5)

<br />
<br />
Looking into CVE-2017-0199, we can see that it allows remote attackers to execute arbitrary code in a MS Office/Wordpad remnote code execution vulnerability. 

![5) full spf record of sender's domain](https://github.com/user-attachments/assets/6859562f-4215-4d7e-ab73-ca83c5db65aa)

<br />
<br />
Continuing with the report, we see CrowdStrike and Metadefender flag this file as malicious. 

![6) they meant 1st URL](https://github.com/user-attachments/assets/fa814f27-efd9-405d-9196-22fd6515d2ec)

<br />
<br />
Here we can see previously generated sandboxes on differed environments of the malicious file. 

![7) conclusion](https://github.com/user-attachments/assets/0fa8a817-3c20-4fc9-8a02-4ae7753b9994)

<br />
<br />

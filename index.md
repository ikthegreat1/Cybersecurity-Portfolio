


# Cybersecurity & Java Portfolio

Welcome! This site showcases compact, working projects that demonstrate API design, incident response skills, and practical automation.

> **Certifications**: •Security+ • CySA+ •CSAP •CCNA • AWS Cloud Practitioner
> **Focus**: SOC Analyst • IT Audit • Risk/Compliance • Blue Team

---

## 🔹 Project 1 — Apply Filters to SQL Queries


Category: Cybersecurity / Data Analysis



Project Description


This project demonstrates how I applied SQL queries with filters to investigate potential security incidents and update employee systems. I worked with system log and employee data to identify unusual login activity and determine which employee machines required updates.

Key Tasks & Examples


🔹 Investigated After-Hours Failed Logins


Wrote SQL queries to filter failed login attempts that occurred after 18:00. This allowed me to identify suspicious after-hours access patterns.

![IMG_8746](https://github.com/user-attachments/assets/535f7796-d0a5-4faa-a9ca-870ae3ebb7f1)

🔹 Analyzed Logins on Specific Dates


Queried login data for suspicious events that occurred on 2022-05-08 and 2022-05-09. I used logical operators (OR) to filter for multiple dates at once.

![Open Portfolio Apply filters to SQL queries](https://github.com/user-attachments/assets/daa398de-011c-4df7-a575-22c0e9554b71)

🔹 Detected Foreign Login Attempts


Retrieved all login attempts that occurred outside of Mexico using a NOT LIKE 'MEX%' filter. This helped isolate unusual geographic login activity.

![IMG_8748](https://github.com/user-attachments/assets/2ec4d114-be3d-4a70-9341-507504b6377c)

🔹 Identified Employees for Security Updates
Pulled employee machines from the Marketing department (East building).

Retrieved employees in Finance OR Sales departments.

Retrieved employees not in IT to apply specialized updates.



![IMG_8749](https://github.com/user-attachments/assets/4d486891-1caf-42cf-9e48-8a7cdb027977)

SQL Techniques Used
Filtering with WHERE clauses

Logical operators: AND, OR, NOT

Pattern matching with LIKE and wildcards (%)

Querying across multiple tables: log_in_attempts, employees

Outcome


This project highlights my ability to apply SQL to real-world cybersecurity use cases such as:

Investigating failed login attempts

Detecting abnormal login activity

Supporting IT teams with system updates


It demonstrates both technical SQL query skills and practical security problem-solving. 

## 🔹 Project 2 — IP Allow List Automation Project


Description:

I developed a Python algorithm to automate management of restricted content access by updating the allow_list.txt file. This script ensures that outdated or unauthorized IP addresses are removed, maintaining secure access controls.



Key Steps

1. Open the allow list file

Used with open(import_file, "r") to safely read the file.
Ensured the file was automatically closed after reading.


<img width="1026" height="180" alt="image" src="https://github.com/user-attachments/assets/09193e44-1b3f-46cd-9101-cb8f8301956e" />

2. Read file contents



Applied .read() to convert the IP addresses into a string.
Stored results in a variable for further processing.




<img width="1026" height="180" alt="image" src="https://github.com/user-attachments/assets/31c966e6-205f-4ac9-a152-96c99cc1c6da" />




3. Convert string to list



Used .split() to separate the IP addresses into list format.
Allowed easy removal of specific IPs later.




<img width="929" height="180" alt="image" src="https://github.com/user-attachments/assets/3c660d7e-6b42-496a-9a20-2b147c01ff66" />





4. Iterate through the remove list



Implemented a for loop to check each IP address in remove_list.
Conditional logic ensured only valid entries were processed.




<img width="682" height="274" alt="image" src="https://github.com/user-attachments/assets/9850ff7c-89ad-4ff3-a092-832252d7f2f2" />





5. Remove unauthorized IPs



Applied .remove() method to delete IPs from the allow list.
Prevented access for flagged addresses.




<img width="936" height="307" alt="image" src="https://github.com/user-attachments/assets/db275d82-1feb-4fab-b325-053cee75a5d7" />


6. Update and overwrite file

Converted list back into a string using .join().
Rewrote the allow_list.txt file with updated IPs using open(..., "w").




<img width="1052" height="180" alt="image" src="https://github.com/user-attachments/assets/fe0611be-0bbb-402e-b8d3-1d45f6ac5714" />



<img width="710" height="213" alt="image" src="https://github.com/user-attachments/assets/42460fc4-f412-49c3-bcd7-e94cdd61c4c3" />


Final Outcome

This project automated the process of maintaining a secure allow list. The script successfully:

Removed unauthorized IP addresses.
Rewrote the file with updated entries.
Ensured restricted content is only accessible to approved IPs 


🔹 Project 3 — Packet Analysis (Wireshark) 


🔹Capture of all my devices pinged (network topology consists of three servers (webserver, fileserver, utilserver) and a workstation (h1).)  

#Looking at ARP traffic.A good way to discover all live hosts on a network. Close analysis of these packets can lead to discoveries of nefarious behaviors such as MAC spoofing, MITM attacks, and NAC (Network Access Control) failures.

<img width="1223" height="770" alt="image" src="https://github.com/user-attachments/assets/f6ec2a2f-eaaa-46e7-b57a-d236de610a50" />

🔹Hunted for unsecured protocols and found telnet being used which contained a username and password in plain text. :) 

<img width="1083" height="480" alt="image" src="https://github.com/user-attachments/assets/05878295-d80e-4dee-885f-ffd4566cbcd1" />


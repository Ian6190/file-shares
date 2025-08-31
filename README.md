# File Shares and Permissions 

## Summary
In this lab, I created shared folders on a domain controller, set different permissions, tested access from a client, and verified that permissions worked correctly.  

### Steps

- **Step 1: Create Folders**
  - On DC-1, created four folders on the C:\ drive:  
    - read-access 
    - write-access  
    - no-access 
    - accounting

    <img width="1226" height="220" alt="image" src="https://github.com/user-attachments/assets/0122d6b1-1c59-43a6-bbf1-ed16e37c3b26" />

- **Step 2: Set Read Access**
  - Gave the Domain Users group **Read** permission to the read-access folder.
 
    <img width="1184" height="868" alt="image" src="https://github.com/user-attachments/assets/b698fba4-8819-4e27-954a-667e115b9db7" />

- **Step 3: Set Write Access**
  - Gave the Domain Users group **Read/Write** permission to the write-access folder.
 
    <img width="1270" height="1324" alt="image" src="https://github.com/user-attachments/assets/95ac7bd9-d898-47bc-9df9-24ff50d1cc1f" />

- **Step 4: Set Admin-Only Access**
  - Gave the Domain Admins group **Read/Write** permission to the no-access folder.

    <img width="1212" height="1278" alt="image" src="https://github.com/user-attachments/assets/883dde77-3bb7-44cc-bf41-91f612ba9d86" />

- **Step 5: Verify Denied Access**
  - Logged into Client-1 as a normal user and confirmed that folders without permission could not be accessed.
 
    <img width="1280" height="520" alt="image" src="https://github.com/user-attachments/assets/678b7132-7d40-42dc-9e70-89ea47deefbb" />

- **Step 6: Allow Permission to User**
  - Added the normal user to the ACCOUNTANTS group and assigned **Read/Write** access to the accounting folder.
 
    <img width="1722" height="1156" alt="image" src="https://github.com/user-attachments/assets/8a2b3373-88cc-4232-b3ee-9f0a9dd82c90" />

- **Step 7: Verify Permission Worked**
  - Logged back into Client-1 as the user and confirmed that access to the accounting
 folder was now allowed.
<img width="1634" height="1056" alt="image" src="https://github.com/user-attachments/assets/ffbf4677-ced7-44cd-9eec-b2324bd1ef2a" />

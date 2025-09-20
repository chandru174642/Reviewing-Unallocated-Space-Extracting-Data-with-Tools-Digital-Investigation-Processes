NAME: CHANDRU.P




REG NO:212223110007


# Reviewing-Unallocated-Space-Extracting-Data-with-Tools-Digital-Investigation-Processes
## AIM:
To review unallocated space in a disk image, extract data using forensic tools, and understand the digital investigation process.
## REQUIREMENTS
- Autopsy or FTK Imager
- Sleuth Kit (TSK)
- Hex Editor (e.g., HxD)
- Operating System: Windows 10/11 or Linux (Kali preferred)
## ARCHITECTURE DIAGRAM
```mermaid
flowchart TD
    A[Disk Image / Physical Drive] --> B[Load into Autopsy or Sleuth Kit]
    B --> C[Identify Unallocated Space]
    C --> D[Scan for Data Signatures]
    D --> E[Carve and Recover Files]
    E --> F[Analyze Recovered Data]
    F --> G[Document Findings in Report]
```
## DESIGN STEPS:
### Step 1 (Acquire Evidence Image):
- Obtain the disk image in ```.dd``` or ```.E01``` format from a trusted forensic acquisition process.
- Verify hash values (MD5/SHA256) to maintain integrity.

### Step 2(Load Image into Forensic Tool):
- Open Autopsy or FTK Imager.
- Create a new case and add the evidence image.

### Step 3(Locate Unallocated Space):
- Navigate to the partition structure view.
- Identify sectors not assigned to any partition (unallocated).
### Step 4(Analyze & Carve Data):
- Use built-in data carving tools to search for file signatures (JPEG, DOCX, PDF, etc.).
- Preview carved files for relevance.
  
## PROGRAM:
| Step | Action                     | Tool Used                   | Output                       |
| ---- | -------------------------- | --------------------------- | ---------------------------- |
| 1    | Load disk image            | Autopsy / FTK Imager        | Partition & unallocated view |
| 2    | Identify unallocated space | Autopsy File System View    | Sector ranges                |
| 3    | Data carving               | Autopsy Data Carving Module | Recovered files              |
| 4    | Export evidence            | Autopsy Export Option       | File copies for analysis     |


## OUTPUT:
Unallocated Space Analysis and Extracted Data Report



 <img width="1412" height="733" alt="Screenshot 2025-09-20 184047" src="https://github.com/user-attachments/assets/76efdc8c-b226-4ffc-b12a-cf952b250b4c" />

 <img width="475" height="367" alt="Screenshot 2025-09-20 184249" src="https://github.com/user-attachments/assets/0ea5b242-cdc8-4f3f-9de7-646a65807c2c" />


 <img width="1696" height="896" alt="Screenshot 2025-09-20 185012" src="https://github.com/user-attachments/assets/90dae20c-2fb7-481c-a20a-d5b522eefb2b" />



 <img width="852" height="522" alt="Screenshot 2025-09-20 185048" src="https://github.com/user-attachments/assets/64ae6e16-65df-4033-8d2a-36ab302b0b7e" />


 <img width="1704" height="909" alt="Screenshot 2025-09-20 185157" src="https://github.com/user-attachments/assets/5a700f84-f260-4cc6-ab06-4a87e16d7ba2" />


 <img width="1860" height="891" alt="Screenshot 2025-09-20 185359" src="https://github.com/user-attachments/assets/d828b5a9-3b14-4ec7-8fe6-03ac2e082171" />







## RESULT:
The unallocated space was successfully analyzed, data was extracted, and the digital investigation process was followed effectively.


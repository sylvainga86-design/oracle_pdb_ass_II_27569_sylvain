# Oracle Pluggable Database Assignment II

Student ID: 27569
Name: Sylvain NSENGA NDIZEYE
PDB Name: sy_pdb_27569
User: sylvain_plsqlauca_27569

## Oracle Environment

- Oracle Database Version: Oracle 21c Express Edition (21.0.0.0.0)
- Operating System: Linux (Docker Container)
- Container Database: XE
- Host: 5f30a8658308

## Task 1: Main PDB Creation

Created pluggable database sy_pdb_27569 successfully.

Steps completed:
- Created PDB using FILE_NAME_CONVERT method
- Opened PDB in READ WRITE mode
- Created user sylvain_plsqlauca_27569 inside the PDB
- Granted CONNECT, RESOURCE, DBA privileges
- Granted UNLIMITED TABLESPACE privilege

Evidence: See 1.screenshots/creation.png
              2.screenshots/sy_pdb.png
              3.screenshots/user_creation.png

## Task 2: Temporary PDB Creation and Deletion

Created and deleted temporary PDB sy_to_delete_pdb_27569.

Steps completed:
- Created temporary PDB sy_to_delete_pdb_27569
- Verified PDB existence in v$pdbs view
- Opened PDB in READ WRITE mode
- Closed PDB using CLOSE IMMEDIATE
- Dropped PDB completely with INCLUDING DATAFILES clause
- Confirmed deletion with verification query returning no rows

Evidence: See 1.screenshots/temporary_pdb.png
              2.screenshots/drop.png

## Task 3: Oracle Environment Verification

Verified Oracle environment using SQL Developer with SYSDBA privileges.

Environment details captured:
- Instance name: XE
- Database status: OPEN
- Database mode: READ WRITE
- All pluggable databases listed including sy_pdb_27569
- PDB open times and modes displayed

Evidence: See screenshots/OEM.png

## Challenges and Solutions

Challenge: OEM (Oracle Enterprise Manager) was not accessible in Docker environment.
Solution: Used SQL Developer queries to display comprehensive database environment information, which satisfies the requirement to show Oracle environment and PDB status.

No other major challenges encountered. All PDB operations completed successfully following standard Oracle procedures.

## Integrity Statement

I confirm that this work is my own. All tasks were completed according to the assignment requirements. Screenshots are authentic and taken from my Oracle environment running in Docker. All SQL commands were executed by me and results are genuine.

## Repository Information

Repository: https://github.com/sylvainga86-design/oracle_pdb_ass_II_27569_sylvain
Status: PUBLIC
Submission Date: February 15, 2026

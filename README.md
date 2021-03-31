# IBMi
DB2 queries and other tools for IBMi

## DTASRCSP.sql - Get the list of Tables/Programs referenced by a Stored Procedure in Order as it appears in the Library List of the job
*Uses output from DSPPGMREF to determine the objects referred by the Program Object and then use a Stored Procedure to retreive the list of Tables/Programs referenced by a Stored Procedure in the same order as it appears in the Library List. This helps determine which LIBRARY.TABLE is being referenced by your Stored Procedure versus what LIBRARY.TABLE is available to it as per the Job Library List.*  
**Program Type: Stored Procedure**
([Link](https://gist.github.com/AbrahamReuben/e5854a184ec3704f0f9a52479e5f8ed0))

## search.sh - Find source physical file members with multiple keywords
*Shell script to search inside source physical file for members that has multiple keywords (both inclusive). This helps to look for a specific source that contains two (or more) terms. Find string function in IBMi limits you to a single string that can be searched.*  
**Progrm Type: Shell Script**
([Link](https://gist.github.com/AbrahamReuben/287c3b9603f89a35bfb473f95f8592d7))

## STR2ARR.SQLRPGLE - Parse a string and populate an array with the elements
*Program to parse a string, delimited by a specific character into an array. Uses the SYSTOOLS.SPLIT function, to parse the input string instead of going with a looping approach.*  
**Program Type: SQLRPGLE**
([Link](https://gist.github.com/AbrahamReuben/d4bdad7bf631c7fb45e3608bb4259fe5))

## TABLESINSP.sql - Get the list of Tables referenced by a Stored Procedure in the Order as it appears in the Library List of the job
*Stored Procedures with Static SQL - Uses QSYS2.SYSROUTINEDEP to determine which tables are used in the Stored Procedure  
Stored Procedures with Dynamic SQL - Reads the source of the Stored Procedure and determines the tables by mapping it to SYSIBM.TABLES  
Once the tables are determined, it is mapped against the library list of the job to determine what table is available in the Libraries as indicated by the Library List for the Stored Procedure. This helps determine which LIBRARY.TABLE is being referenced by your Stored Procedure versus what LIBRARY.TABLE is available to it as per the Job Library List.  
Note: Check DTASRCSP.sql that uses a different approach on this same requirement*  
**Program Type: SQL**
([Link](https://gist.github.com/AbrahamReuben/5b625300b203f1ebbf3d88b1679a2c43))

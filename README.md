# IBMi
DB2 queries and other tools for IBMi

## DTASRCSP.sql - Get the list of Tables/Programs referenced by a Stored Procedure in Order as it appears in the Library List of the job ##
*Uses output from DSPPGMREF to determine the objects referred by the Program Object and then use a Stored Procedure to retreive the list of Tables/Programs referenced by a Stored Procedure in the same order as it appears in the Library List. This helps determine which LIBRARY.TABLE is being referenced by your Stored Procedure versus what LIBRARY.TABLE is available to it as per the Job Library List.*<br/><br/>
**Program Type: Stored Procedure**
([Link](https://gist.github.com/AbrahamReuben/e5854a184ec3704f0f9a52479e5f8ed0))

## SEARCH.sh - Find source physical file members with multiple keywords ##
*Shell script to search inside source physical file for members that has multiple keywords (both inclusive). This helps to look for a specific source that contains two (or more) terms. Find string function in IBMi limits you to a single string that can be searched.*<br/><br/>
**Progrm Type: Shell Script**
([Link](https://gist.github.com/AbrahamReuben/287c3b9603f89a35bfb473f95f8592d7))

## STR2ARR.SQLRPGLE - Parse a string and populate an array with the elements ##
*Program to parse a string, delimited by a specific character into an array. Uses the SYSTOOLS.SPLIT function, to parse the input string instead of going with a looping approach.*<br/><br/>
**Program Type: SQLRPGLE**
([Link](https://gist.github.com/AbrahamReuben/d4bdad7bf631c7fb45e3608bb4259fe5))

## TABLESINSP.sql - Get the list of Tables referenced by a Stored Procedure in the Order as it appears in the Library List of the job ##
*Stored Procedures with Static SQL - Uses QSYS2.SYSROUTINEDEP to determine which tables are used in the Stored Procedure<br/>
Stored Procedures with Dynamic SQL - Reads the source of the Stored Procedure and determines the tables by mapping it to SYSIBM.TABLES<br/><br/>
Once the tables are determined, it is mapped against the library list of the job to determine what table is available in the Libraries as indicated by the Library List for the Stored Procedure. This helps determine which LIBRARY.TABLE is being referenced by your Stored Procedure versus what LIBRARY.TABLE is available to it as per the Job Library List.<br/><br/>
Note: Check DTASRCSP.sql that uses a different approach on this same requirement*<br/><br/>
**Program Type: SQL**
([Link](https://gist.github.com/AbrahamReuben/5b625300b203f1ebbf3d88b1679a2c43))

## WHRISOBJ.sql - Find which version of an Object is seen by the Job in accordance to the Library List set up ##
*While executing IBMi commands/programs from an external source, it gets difficult to determine if an object is present in the Library List of the Job or which version 
of the Object is seen by the Job in accordance with the Library List set up of the job.<br/>The idea behind this script is to get the Library Listing of the Job and use it 
to determine which version of the Object is seen by the job.*<br/><br/>
**Program Type: SQL**
([link](https://gist.github.com/AbrahamReuben/503c15cb6a8991b8f57da268a30646da))

## DeepSearch.sql - Get the list of Source Physical file Members with a specific keyword ##
*The idea behind this script is to find that one source in the system, which you know exists but you just don't know the source physical file which houses that source. 
This SQL does the same function as a Find String with a difference that this can be used to search into All Source Physical Files in a Libarary or into All Source Physical Files in the system.
<br/><br/>
Note: Check SEARCH.sh that does a multi-layered search using a shell script.
<br/><br/>
NB: This script alters the Find String command parameters to print the results. Flip the parameters back as required*<br/><br/>
**Program Type: SQL**
([link](https://gist.github.com/AbrahamReuben/8f7bfbc9e7b22a39cbbe96298a78bcc6))

## FindString.sql - Do the equivalent of Find String from the Run SQL ##
*Do the equivalent of Find String from the Run SQL window. This Stored Procedure also lets you search for multiple SRCPFs for a keyword in a single go.*<br/><br/>
**Program Type: SQL**
([link](https://gist.github.com/AbrahamReuben/f5d64be764116e4afaeb46e72c275601))

## TextCleanUp.sql - Clean up characters in a string by replacing from a list of characters ##
*Clean up non-printable or other characters in a string by replacing each character from a substitution list.* <br/><br/>
**Program Type: SQL**
([link](https://gist.github.com/AbrahamReuben/48f48c42ca94fc1f2e63e11e4079148f))

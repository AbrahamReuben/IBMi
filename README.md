# IBMi
DB2 queries and other tools for IBMi

## DTASRCSP.sql - Get the list of Tables/Programs referenced by a Stored Procedure in Order as it appears in the Library List
*Stored Procedure to fetch the list of Tables/Programs referenced by a Stored Procedure in the same order as it appears in the Library List. This helps determine which LIBRARY.TABLE is being referenced by your Stored Procedure versus what LIBRARY.TABLE is available to it as per the Job Library List.*
([Link](https://gist.github.com/AbrahamReuben/e5854a184ec3704f0f9a52479e5f8ed0))

## search.sh - Find source physical file members with multiple keywords
*Shell script to search inside source physical file for members that has multiple keywords (both inclusive). This helps to look for a specific source that contains two (or more) terms. Find string function in IBMi limits you to a single string that can be searched.*
([Link](https://gist.github.com/AbrahamReuben/287c3b9603f89a35bfb473f95f8592d7))

## STR2ARR.SQLRPGLE - Parse a string and populate an array with the elements
*SQLRPGLE program to parse a string, delimited by a specific character into an array. Uses the SYSTOOLS.SPLIT function, to parse the input string instead of going with a looping approach.*
([Link](https://gist.github.com/AbrahamReuben/d4bdad7bf631c7fb45e3608bb4259fe5))

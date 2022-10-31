```
[cs15lfa22ga@ieng6-203]:skill-demo1:154$ find ./technical -name pmed.0020281.txt
./technical/plos/pmed.0020281.txt
```
Using the find command -name option to find the specific file with the name of pmed.0020281.txt

```
[cs15lfa22ga@ieng6-203]:skill-demo1:157$ find ./technical -name "*.txt"
./technical/plos/pmed.0020073.txt
...
./technical/plos/pmed.0020278.txt
./technical/plos/pmed.0020281.txt
```
Using the find command -name option to find every file that end with .txt file

```
[cs15lfa22ga@ieng6-203]:skill-demo1:157$ find ./technical -name *.*.txt
./technical/911report/chapter-13.1.txt
./technical/911report/chapter-13.2.txt
...
./technical/plos/journal.pbio.0020001.txt
./technical/plos/journal.pbio.0020010.txt
...
./technical/plos/pmed.0020278.txt
./technical/plos/pmed.0020281.txt
```
Using the find command -name option to find every files that has the pattern of something.somthing.txt

```
[cs15lfa22ga@ieng6-203]:skill-demo1:164$ find ./technical/government/About_LSC/ -print
./technical/government/About_LSC/
./technical/government/About_LSC/CONFIG_STANDARDS.txt
./technical/government/About_LSC/Comments_on_semiannual.txt
./technical/government/About_LSC/LegalServCorp_v_VelazquezDissent.txt
./technical/government/About_LSC/LegalServCorp_v_VelazquezOpinion.txt
./technical/government/About_LSC/LegalServCorp_v_VelazquezSyllabus.txt
./technical/government/About_LSC/ODonnell_et_al_v_LSCdecision.txt
./technical/government/About_LSC/ONTARIO_LEGAL_AID_SERIES.txt
./technical/government/About_LSC/Progress_report.txt
./technical/government/About_LSC/Protocol_Regarding_Access.txt
./technical/government/About_LSC/Special_report_to_congress.txt
./technical/government/About_LSC/State_Planning_Report.txt
./technical/government/About_LSC/State_Planning_Special_Report.txt
./technical/government/About_LSC/Strategic_report.txt
./technical/government/About_LSC/commission_report.txt
./technical/government/About_LSC/conference_highlights.txt
./technical/government/About_LSC/diversity_priorities.txt
./technical/government/About_LSC/reporting_system.txt
```
Using the find command -print option to print out the pathway of all files in given directories

```
[cs15lfa22ga@ieng6-203]:skill-demo1:167$ find ./technical -name pmed.0020281.txt -print
./technical/plos/pmed.0020281.txt
```
Using the find command -print to print out the pathway of specific file

```
[cs15lfa22ga@ieng6-203]:skill-demo1:175$ find ./technical/plos/pmed.0020281.txt -print
./technical/plos/pmed.0020281.txt
```
When you give out a specific file location, it will only print the path to that location

```
[cs15lfa22ga@ieng6-203]:skill-demo1:174$ find ./technical -type d
./technical
./technical/911report
./technical/biomed
./technical/government
./technical/government/About_LSC
./technical/government/Alcohol_Problems
./technical/government/Env_Prot_Agen
./technical/government/Gen_Account_Office
./technical/government/Media
./technical/government/Post_Rate_Comm
./technical/plos
```
Using -type d to print out all the derectories underneath in that given derectory

```
[cs15lfa22ga@ieng6-203]:skill-demo1:176$ find ./technical/plos -type f
./technical/plos/journal.pbio.0020001.txt
./technical/plos/journal.pbio.0020010.txt
...
./technical/plos/pmed.0020275.txt
./technical/plos/pmed.0020278.txt
./technical/plos/pmed.0020281.txt
```
Using -type f to print out all the files in the given directory.

```
[cs15lfa22ga@ieng6-203]:skill-demo1:177$ find ./technical/plos -type l
[cs15lfa22ga@ieng6-203]:skill-demo1:178$ 
```
Using -type options to print out all the links it has in current given directory, however there isn't any
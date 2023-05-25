# Lab Report 3 - Researching Commands

<br>

## Command Line Options
- find -type
- find -size
- find -perm
- find -mtime

<br>

## Command Line Example find `-type`
```
Command:
find technical/ -type f

Output:
technical/biomed/1471-2350-2-2.txt
technical/biomed/1471-2350-2-8.txt
technical/biomed/1471-2350-3-1.txt
technical/biomed/1471-2350-3-12.txt
technical/biomed/1471-2350-3-7.txt
technical/biomed/1471-2350-3-9.txt
technical/biomed/1471-2350-4-2.txt
technical/biomed/1471-2350-4-3.txt
technical/biomed/1471-2350-4-4.txt
technical/biomed/1471-2350-4-6.txt
technical/biomed/1471-2369-3-1.txt
...
```
- The command `find -type f` allows you to search for regular files. This command is useful because it allows you to to search specificly for the regular files in a directory tree, it makes it easier when working with those files. Source: ChatGPT The prompt I gave ChatGPT was asking it "Give me commands for the command `find -type`" The output gave me multiple commands such as `find . -type f` `find ~ -type d` `find . -type p` and more. I used this output in order to find specific examples I could use and then I used the prompt "what does the command `find -type f` do" and it outputted "The command `find -type f` searches the current directory and its subdirectories for regular files and lists them." I used this information outputted here to discuss how this command could be useful.



---

```
Command:
find technical/ -type d

Output:
technical/
technical/911report
technical/biomed
technical/government
technical/government/About_LSC
technical/government/Alcohol_Problems
technical/government/Env_Prot_Agen
technical/government/Gen_Account_Office
technical/government/Media
technical/government/Post_Rate_Comm
technical/plos
```
- The command `find -type d` allows you to search for directories. This command is useful because it allows you to search specificly for directories, it is useful when you are looking for specific directories within any directory. Source: ChatGPT The prompt I gave ChatGPT was asking it "Give me commands for the command `find -type`" The output gave me multiple commands such as `find . -type f` `find ~ -type d` `find . -type p` and more. I used this output in order to find specific examples I could use and then I used the prompt "what does the command `find -type d` do" and it outputted "The command `find -type d` searches the current directory and its subdirectories for directories and lists them." I used this information outputted here to discuss how this command could be useful.

<br>

## Command Line Example find `-size`
```
Command:
find technical/ -size -10k

Output:
technical/
technical/911report
technical/biomed
technical/biomed/1471-2334-3-13.txt
technical/biomed/1471-2490-3-2.txt
technical/government
technical/government/About_LSC
technical/government/About_LSC/LegalServCorp_v_VelazquezSyllabus.txt
technical/government/About_LSC/ODonnell_et_al_v_LSCdecision.txt
technical/government/Alcohol_Problems
technical/government/Env_Prot_Agen
technical/government/Gen_Account_Office
technical/government/Gen_Account_Office/d01121g.txt
technical/government/Gen_Account_Office/Letter_WalkerJan30-2001.txt
technical/government/Gen_Account_Office/og96009.txt
...
```
- The command `find -size -` allows you to search for files and directories that are smaller than a certain size. This command is useful because it allows you to easily find files that are below a certain size (in this case 10kb), it is useful when you want to delete certain files below a size threshold. Source: ChatGPT The prompt I gave ChatGPT was asking it "Give me commands for the command `find -size`." The output gave me multiple commands such as `find . -size +1M` `find ~ -size 50m` `find . -size +10k` `find . -size -50k` and more. I used this output in order to find specific examples I could use and then I used the prompt "what does the command `find -size -10k` do" and it outputted "The command `find -size -10k` searches for files that are smaller than 10 kilobytes." I used this information outputted here to discuss how this command could be useful.

---

```
Command: 
find technical/ -size +100K

Output:
technical/911report/chapter-13.4.txt
technical/911report/chapter-13.5.txt
technical/911report/chapter-3.txt
technical/government/About_LSC/commission_report.txt
technical/government/Env_Prot_Agen/bill.txt
technical/government/Gen_Account_Office/d01591sp.txt
technical/government/Gen_Account_Office/GovernmentAuditingStandards_yb2002ed.txt   
technical/government/Gen_Account_Office/pe1019.txt
technical/government/Gen_Account_Office/Statements_Feb28-1997_volume.txt
```
- The command `find -size +` allows you to search for files and directories that are bigger than a certain size. This command is useful because it allows you to easily find files that are above a certain size (in this case 100kb), it is useful when you want to delete certain files above a size threshold to free up lots of space. Source: ChatGPT The prompt I gave ChatGPT was asking it "Give me commands for the command `find -size`." The output gave me multiple commands such as `find . -size +1M` `find ~ -size 50m` `find . -size +10k` `find . -size -50k` and more. I used this output in order to find specific examples I could use and then I used the prompt "what does the command `find -size +100k` do" and it outputted "The command `find -size +100k` searches for files that are larger than 100 kilobytes." I used this information outputted here to discuss how this command could be useful.

<br>

## Command Line Example find `-perm`
```
Command:
find technical/ -perm /o+r

Output:
technical/biomed/1471-2350-4-4.txt
technical/biomed/1471-2350-4-6.txt
technical/biomed/1471-2369-3-1.txt
technical/biomed/1471-2369-3-10.txt
technical/biomed/1471-2369-3-6.txt
technical/biomed/1471-2369-3-9.txt
technical/biomed/1471-2369-4-1.txt
technical/biomed/1471-2369-4-5.txt
technical/biomed/1471-2377-1-2.txt
technical/biomed/1471-2377-2-4.txt
technical/biomed/1471-2377-2-6.txt
technical/biomed/1471-2377-3-4.txt
technical/biomed/1471-2407-1-13.txt
...
```
- The command `find -perm /o+r` allows you to search for files and directories that have read permission for everyone. This command is useful because it allows you to find files that you have permission to read therefore avoiding the ones that you are not allowed to read saving you time. Source: ChatGPT The prompt I gave ChatGPT was asking it "Give me commands for the command `find -perm`." The output gave me multiple commands such as `find . -perm 644` `find . -perm /g+x` `find . -perm /o+r` and more. I used this output in order to find specific examples I could use and then I used the prompt "what does the command `find -perm /o+r` do" and it outputted "The command `find -perm /o+r` searches for files that have read permissions for others." I used this information outputted here to discuss how this command could be useful.

---

```
Command:
find technical/ -perm /g+x

Output:
technical/
technical/911report
technical/biomed
technical/government
technical/government/About_LSC
technical/government/Alcohol_Problems
technical/government/Env_Prot_Agen
technical/government/Gen_Account_Office
technical/government/Media
technical/government/Post_Rate_Comm
technical/plos
```
- The command `find -perm /g+x` allows you to search for files and directories that have execute permission for the group. This command is useful because it allows you to check if a file or directory has the correct group execute permissions, it is useful when you are troubleshootings and you need to check if it has the correct group execute permissions. Source: ChatGPT The prompt I gave ChatGPT was asking it "Give me commands for the command `find -perm`." The output gave me multiple commands such as `find . -perm 644` `find . -perm /g+x` `find . -perm /o+r` and more. I used this output in order to find specific examples I could use and then I used the prompt "what does the command `find -perm /g+x` do" and it outputted "The command `find -perm /g+x` searches for files that have execute permissions for the group." I used this information outputted here to discuss how this command could be useful.

<br>

## Command Line Example find `-mtime`
```
Command:
find technical/ -mtime +10
 
Output:
technical/biomed/1471-2350-4-4.txt
technical/biomed/1471-2350-4-6.txt
technical/biomed/1471-2369-3-1.txt
technical/biomed/1471-2369-3-10.txt
technical/biomed/1471-2369-3-6.txt
technical/biomed/1471-2369-3-9.txt
technical/biomed/1471-2369-4-1.txt
technical/biomed/1471-2369-4-5.txt
technical/biomed/1471-2377-1-2.txt
technical/biomed/1471-2377-2-4.txt
technical/biomed/1471-2377-2-6.txt
technical/biomed/1471-2377-3-4.txt
technical/biomed/1471-2407-1-13.txt
...
```
- The command `find -mtime +` allows you to search for files and directories that were last modified above a certain amount of days (in this case 10 days). This command is useful because it allows you to find files that have not been modified recently, it is useful when wanting to delete files that are no longer needed. Source: ChatGPT The prompt I gave ChatGPT was asking it "Give me commands for the command `find -mtime`." The output gave me multiple commands such as `find -mtime 0` `find -mtime +10` `find -mtime -15` `find -mtime -0.5` and more. I used this output in order to find specific examples I could use and then I used the prompt "what does the command `find -mtime +10` do" and it outputted "The command `find -mtime +10` searches for files that were modified more than 10 days ago." I used this information outputted here to discuss how this command could be useful.

---

```
Command:
find technical/ -mtime -20

Output: 
technical/biomed/1471-2350-4-4.txt
technical/biomed/1471-2350-4-6.txt
technical/biomed/1471-2369-3-1.txt
technical/biomed/1471-2369-3-10.txt
technical/biomed/1471-2369-3-6.txt
technical/biomed/1471-2369-3-9.txt
technical/biomed/1471-2369-4-1.txt
technical/biomed/1471-2369-4-5.txt
technical/biomed/1471-2377-1-2.txt
technical/biomed/1471-2377-2-4.txt
technical/biomed/1471-2377-2-6.txt
technical/biomed/1471-2377-3-4.txt
technical/biomed/1471-2407-1-13.txt
technical/biomed/1471-2407-1-15.txt
technical/biomed/1471-2407-1-19.txt
...
```
- The command `find -mtime -` allows you to search for files and directories that were last modified below a certain amount of days (in this case 20 days). This command is useful because it allows you to find files that have been modified recently, it is useful when wanting to use files you have been working on recently. Source: ChatGPT The prompt I gave ChatGPT was asking it "Give me commands for the command `find -mtime`." The output gave me multiple commands such as `find -mtime 0` `find -mtime +10` `find -mtime -15` `find -mtime -0.5` and more. I used this output in order to find specific examples I could use and then I used the prompt "what does the command `find -mtime -20` do" and it outputted "The command `find -mtime -20` searches for files that were modified within the last 20 days." I used this information outputted here to discuss how this command could be useful.

 




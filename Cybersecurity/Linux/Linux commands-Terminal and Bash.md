Linux commands-Terminal and Bash
mkdir Internal_Investigation_Employee_A
ls
cd /03-student/day1/
pwd 
touch email_evidence log_evidence web_evidence
rm  web_evidence
clear
mv /03-student/day1/take_5/Internal_Investigation_Employee_A/email_evidence /03-student/day1/take_5/Internal_Investigation_Employee_B/
cp /03-student/day1/take_5/Internal_Investigation_Employee_A/log_evidence /03-student/day1/take_5/Internal_Investigation_Employee_B/
head do.txt
more do.txt
tail do.txt
cat  emailA sd.txt  email1 email4 log1 log2     recipe_for_sugarplum  recipe_for_sweetums > Wonka-evidence.txt
man wc
wc -w *
wc -w * > Connections_by_website
find -type d -iname *secret*   lets you find all directories
find -type f -iname *recipe*
find -type f -iname *recipe* -a  -iname *peanut*
grep -i guavaberries *
grep -il slugworth * > slugworth_email_evidence
grep -il slugworth * | wc -l >> slugworth_email_evidence
mv ./Gathering_Evidence/email/slugworth_email_evidence ./Gathering_Evidence/Slugworth_evidence/
cat slugworth_email_evidence slugworth_web_evidence > Slugworth_evidence_for_authorities
find -type f -iname *0719*
mv ./WEBACCESS/*0719* ./subpoena_request/
grep '212-555-2732\|212-555-2733\|212-555-2734' ./DIRECTORIES/*
cat Admin_logA.txt Admin_logB.txt > Combined_Access_logs.txt
sed s/INCORRECT_PASSWORD/ACCESS_DENIED/ Combined_Access_logs.txt > Update1_Combined_Access_logs.txt
awk '{print $4, $6}' Update1_Combined_Access_logs.txt
more Update2_Combined_Access_logs.txt
nano Log_analysis.sh
sh Log_analysis.sh
curl -s http://ipinfo.io/104.223.95.86
curl -s http://ipinfo.io/104.223.95.86 | grep country
curl -s http://ipinfo.io/104.223.95.86 | grep country | awk -F: '{print $2}'
sudo bash /home/instructor/Documents/setup_scripts/instructor/landmarks_review.sh
top
ps
kill
ps aux >> ~/currently_running_processes
sudo killall -u jack.
sudo apt install <package>
sudo chown sysadmin:sysadmin shadow_copy
sudo john shadow_copy
 whoami
 sudo -l
 sudo -lU <username>  >> ~/research/sudo_access.txt
 sudo su max
 sudo less shopping_list.txt
 q
 !bash
 exit
 grep less /etc/sudoers
 visudo
 id
 sudo usermod -G jack jack
 sudo delgroup hax0rs
 sudo deluser --remove-home jack
 tar [option(s)] [archive_filename] [objects_to_archive]
 tar cvvWf 20190505epscript.tar epscript/ > 20190505epscript.txt
 ls -lat
 mkdir ~/research && cp -r /var/log/* /etc/passwd /etc/shadow /etc/hosts ~/research
 sudo cp -r 
 ps aux --sort -%mem | awk {'print $1, $2, $3, $4, $11'} | head > ~/research/top_processes.txt
 cat /etc/passwd | awk -F ":" '{if ($3 >= 1000) print $0}'
 echo "alias lsa='ls -a'" >> ~/.bashrc
 #!/bin/bash
echo "DNS Servers: "
execs=$(find /home -type f -perm 777)

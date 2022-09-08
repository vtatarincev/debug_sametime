# debug_sametime
Utility to gather logs for sametime

for HCL Support, created small shell file that collects all needed information and also does local backup of configuration. 



[root@meet sametime]# ./debug_sametime.sh
*******************************************
welcome to CYONE  HCL Sametime debug utility
*******************************************
1/7. Debug filename: HCL_TECHNICAL_SUPPORT/sametime_logs_2022_09_08_12_58.txt
2/7. Running docker-compose logs
3/7. Gathering Netstat output, adding to debug information
4/7. Generating MD5 hashes of files, so support can verify. This may take 20-30 sec
4/7. Gathering server network config.
5/7. Zipping files, please wait 1 sec
  adding: HCL_TECHNICAL_SUPPORT/sametime_logs_2022_09_08_12_58.txt (deflated 97%)
  adding: custom.env (deflated 54%)
  adding: .env (deflated 56%)
  adding: docker-compose.yml (deflated 84%)
  adding: HCL_TECHNICAL_SUPPORT/netstat_2022_09_08_12_58.txt (deflated 90%)
  adding: HCL_TECHNICAL_SUPPORT/md5sum.txt (deflated 71%)
  adding: HCL_TECHNICAL_SUPPORT/network.txt (deflated 61%)
Lets backup important files. Dont forget to backup them outside this server!
6/7. Backuping .env docker-compose.yml custom.env to HCL_TECHNICAL_SUPPORT with timestamp 2022_09_08_12_58
7/7. Information: Size of debug directory:  HCL_TECHNICAL_SUPPORT
928K	HCL_TECHNICAL_SUPPORT/BACKUP
81M	HCL_TECHNICAL_SUPPORT
*********
File /opt/hcl/sametime/HCL_TECHNICAL_SUPPORT/sametime_logs_2022_09_08_12_58.zip has all information to debug issue.
Powered by CYONE.EU. Check out www for great products for Notes/Domino/Traveler/Sametime
use following command to download ZIP to your local PC
           scp root@meet.acme.local:/opt/hcl/sametime/HCL_TECHNICAL_SUPPORT/sametime_logs_2022_09_08_12_58.zip sametime_logs_2022_09_08_12_58.zip

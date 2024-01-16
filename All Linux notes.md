hi welcome <br/>

16/1 <br/>

### scoop is developed by google at 2002.
it has mapper and reuducer. mapper is to copy the files from one area to the another area. Reducer is to do opertions on the analytical data on the mapper on hdfs.<br/>
# just general overview,, i am not sure, but i try.... 
# walk by faith not by sight.<br/>

### ping commands
in linux <br/>
ping 8.8.8.8 - used to see the latency for the google server <br/>   
in windows <br/>
ping 8.8.8.8 -t <br/>

### task manager in linux

ps -ef <br/>
ps -ef | grep-v root  - means it will ignore the root user values... <br/>

### SUDO KILL COMMANDS 

sudo kill -9 process_id <br/>
here, while running a processes in a shell script , the 1st number represents the particular child processes <br/>
the 2nd no represents the parent process , be careful if u fill 2n no then it may forcely shut down the terminal also <br/>


ctrl+c is used to kill the current processes <br/>

while u are in the current user , then u need to give chmod to the 1st no as 7, then u can execute... <br/>

sample program <br/>

echo samuel <br/>
sleep 1000 <br/>
echo success <br/>


### LS COMMANDS 

ls -lsrt * - means view the files and folders.<br/>
ls -lsrt samuel - means view that particular folder contents only <br/>

ls - used to see list of all files<br/>
ls -a used to see all the hidden files<br/>
ls -lart used to see all the hidden files along with the file size<br/>
ls -lrt used to see all the files<br/>
using ls -a cat the .bash_history file to see all the recently typed files, .bashrc files is to view the vriables tht are declred globally..<br/>

### head and tail are used to view the first and the last contents of the file<br/>

for eg, grep sam ss.csv | head -4 <br/>
grep sam ss.csv | tail -3 <br/>
| - is use to pass the values from one area to another area. <br/>
for eg, grep sam ss.csv | wc as raw <br/>
### wc Here, the numbers represent the wc -l line count, wc -w word count, and wc -c character count, respectively.<br/>


### grep commands are used to see the searched word along with the files.
<br/>
grep Master ss.csv
remember at starting grep is case sensitive, for normal grep
now we see the grep types,,,,
grep -i is to ignore the case sensitive
grep -c is to count how many times that word occurs
grep -v is not match things
grep -w will take only the exact word only.
grep -l will give the line no
<br/>

### mkdir is used to create a folder
### rmdir is used to remove a folder
### rm filename is used to remove a file
### copy 
cp is used to copy a file from one area to another area. <br/>
for eg, cp /home/hduser/ss.csv /home/hduser/ss/<br/>
cp /home/hduser/ss.csv /home/hduser/ss/dd.csv<br/>

it will rename and then save <br/>

cp -p is used to preserve the file details and then save {like time nd date are same} <br/>
## make directory 
mkdir /home/hduser/samuel<br/>

mkdir /home/hduser/samuel/ss if the folder does not exist then it will create a folder for us<br/>
mkdir -p /home/hduser/samuel/ss , antha madri folder iruntha create panu, ilana vituru<br/>

### echo commands
generally echo used to print <br/>
echo $? is to see whether the file is sucessfully execute or not ! <br/>

to set echo value in shell script , for eg, <br/>
### program
echo hello<br/>
exit 1<br/>


using if, we do now  <br/>

echo sam<br/>
status_1=$?<br/>

ec gsryhrdyh<br/>
status_2=$?<br/>

# Check the exit status of each command and set custom exit statuses<br/>
if [ "$status_1" -eq 0 ]; then<br/>
    echo "Command 1 succeeded with exit status $status_1"<br/>
else<br/>
    echo "Command 1 failed with exit status $status_1"<br/>
    exit 1<br/>
fi<br/>

if [ "$status_2" -eq 127 ]; then<br/>
    echo "Command 2 succeeded with exit status $status_2"<br/>
else<br/>
    echo "Command 2 failed with exit status $status_2"<br/>
    exit 2<br/>
fi<br/>

# Continue with the rest of your script<br/>



0 is success and 1 is error<br/>

mv is used to move the files from one are to another area,,,,<br/>

mv ss.csv /home/hduser/samuel<br/>
there file is absent bec it is already moved like cut and paste. again i copied from samuel to hduser now i move with another name,, its also working!!!<br/>
mv ss.csv /home/hduser/samuel/dd.csv<br/>

:w - is used to write to a file<br/>
:q - is used to quit the file<br/>
:q! - is used to forcely quit that file<br/>
:wq! - is used to forcely write and quit that file <br/>
! may require sudo password../..<br/>

su username - used to change the user , for eg su root, the default password for root is root<br/>

su -i is also used to go to the root.<br/>

cd /home/hduser/Desktop/ss.csv is  absolute path<br/>

[localhost@hduser Desktop] - cd hello  - its an relative path,,, from a path we are going to another area<br/>

cd itself (if not mentioned path_) is used to come back to the previous folder,<br/>

## permissions

chmod we use <br/>

chmod 000 means no permission <br/>

### 0 - no access
### 1 - only execute access
### 2 - only write
### 4 - only read

we combine this numbers to show the permisiions , for eg, chmod 777 ss.csv means all permissions for all users <br/>

1st no means root user <br/>
2nd no means current user <br/>
3rd no means group user <br/>

here, we see that , <br/>

chmod o+r <br/>
chmod u+rw <br/>
chmod G-rwx <br/>

here + to give access, - to revoke permissions, r -read , w- write, x -execute. <br/>

# ADD USERS
sudo is just like run as administrator in windows <br/>
it is used to providing powwer to execute things <br/>












lets see for ss.csv file<br/>


shell script are a combination of all the linux commands, once executed it will be an automated process...<br/>
2 ways to start a shell script. one is using ./   , another one is by using bash bashfile.sh<br/>






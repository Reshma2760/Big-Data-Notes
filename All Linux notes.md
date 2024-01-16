hi welcome

16/1

### scoop is developed by google at 2002.
it has mapper and reuducer. mapper is to copy the files from one area to the another area. Reducer is to do opertions on the analytical data on the mapper on hdfs.<br/>
just general overview,, i am not sure, but i try.... walk by faith not by sight.

ls - used to see list of all files
ls -a used to see all the hidden files
ls -lart used to see all the hidden files along with the file size
ls -lrt used to see all the files
using ls -a cat the .bash_history file to see all the recently typed files, .bashrc files is to view the vriables tht are declred globally..

head and tail are used to view the first and the last contents of the file

for eg, grep sam ss.csv | head -4
grep sam ss.csv | tail -3
| - is use to pass the values from one area to another area.
for eg, grep sam ss.csv | wc as raw 
wc Here, the numbers represent the wc -l line count, wc -w word count, and wc -c character count, respectively.


grep commands are used to see the searched word along with the files.
grep Master ss.csv
remember at starting grep is case sensitive, for normal grep
now we see the grep types,,,,
grep -i is to ignore the case sensitive
grep -c is to count how many times that word occurs
grep -v is not match things
grep -w will take only the exact word only.
grep -l will give the line no

mkdir is used to create a folder
rmdir is used to remove a folder
rm filename is used to remove a file

cp is used to copy a file from one area to another area.
for eg, cp /home/hduser/ss.csv /home/hduser/ss/
cp /home/hduser/ss.csv /home/hduser/ss/dd.csv

it will rename and then save 

cp -p is used to preserve the file details and then save {like time nd dateare same}

mkdir /home/hduser/samuel

mkdir /home/hduser/samuel/ss if the folder does not exist then it will create a folder for us
mkdir -p /home/hduser/samuel/ss , antha madri folder iruntha create panu, ilana vituru

echo commands
generally echo used to print 
echo $? is to see whether the file is sucessfully execute or not ! 

to set echo value in shell script , for eg, 

echo hello
exit 1


using if, we do now  

echo sam
status_1=$?

ec gsryhrdyh
status_2=$?

# Check the exit status of each command and set custom exit statuses
if [ "$status_1" -eq 0 ]; then
    echo "Command 1 succeeded with exit status $status_1"
else
    echo "Command 1 failed with exit status $status_1"
    exit 1
fi

if [ "$status_2" -eq 127 ]; then
    echo "Command 2 succeeded with exit status $status_2"
else
    echo "Command 2 failed with exit status $status_2"
    exit 2
fi

# Continue with the rest of your script



0 is success and 1 is error

mv is used to move the files from one are to another area,,,,

mv ss.csv /home/hduser/samuel
there file is absent bec it is already moved like cut and paste. again i copied from samuel to hduser now i move with another name,, its also working!!!
mv ss.csv /home/hduser/samuel/dd.csv

:w - is used to write to a file
:q - is used to quit the file
:q! - is used to forcely quit that file
:wq! - is used to forcely write and quit that file 
! may require sudo password../..

su username - used to change the user , for eg su root, the default password for root is root

su -i is also used to go to the root.

cd /home/hduser/Desktop/ss.csv is  absolute path

[localhost@hduser Desktop] - cd hello  - its an relative path,,, from a path we are going to another area

cd itself (if not mentioned path_) is used to come back to the previous folder,





lets see for ss.csv file


shell script are a combination of all the linux commands, once executed it will be an automated process...
2 ways to start a shell script. one is using ./   , another one is by using bash bashfile.sh






# HI WELCOME TO SCOOP

## SEE THE DATABASES

sqoop list-databases --connect jdbc:mysql://localhost --username root --password Root123$; <br/>

sqoop list-tables --connect jdbc:mysql://localhost/custdb --username root --password Root123$; <br/>

# TO MOVE DATA FROM SQL TO HDFS

sqoop import --connect jdbc:mysql://localhost/custdb --username root --password Root123$ \--query " select custid,age,transactamt from customer where (city ='banglore' or age>33) and\$CONDITIONS " \--target-dir /hello --delete-target-dir -m 2 --split-by custid; <br/>

Using 1 mapper <br/>

sqoop import   --connect jdbc:mysql://localhost/custdb --username root --password Root123$ --table customer --target-dir /hello --delete-target-dir --num-mappers 1; <br/>

### TO MOVE FROM HDFS TO SQL WE USE <BR/>

CREATE CRT TABLE ON SQL THEN USE THE BELOW COMMAND <br/>

sqoop export --connect jdbc:mysql://localhost/custdb --username root --password Root123$ --table customer_hdfs1 \--export-dir /hello; <br/>

### TO VIEW JOB LIST <BR/>

sqoop job -list <br/>

### TO CREATE A JOB LIST <br/>

sqoop job --create myjob1 -- import --connect jdbc:mysql://localhost/custdb --username root --password Root123$ \--table customer --target-dir \hello --delete-target-dir -m 1; <br/>

sqoop job --create myImportJob \-- import \--connect jdbc:mysql://localhost/custdb \--username root \--password Root123$ \--table customer \--target-dir /hello \--fields-terminated-by ',' \--lines-terminated-by '\n' \--num-mappers 1;<br/>

while executing it will ask password, use the password <br/>
## Root123$ <br/>

### TO RUN Sqoop JOBS <br/>
sqoop job --exec myjob1 <br/>












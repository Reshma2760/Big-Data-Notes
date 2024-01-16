using sql connector i tried to use the sting called mydb = sql.connect(host="127.0.0.1",
                   user="root",
                   password="1234",
                   database= "phonepedata",
                   port = "3307"
                  )
mycursor = mydb.cursor(buffered=True)

but it thrown mwe an ssh encryption error. I solved it by installing correct pip along with that... let see the crt pip using the comman called pip freeze.

mysql-connector==2.2.9
mysql-connector-python==8.0.28

install this 2 pip , then u will definitely rectify the sql db connection problems.
 python --version to see the current python version..
 always use 3.9.0
 here, i use pip install jupyter notebook to install it, after installing dont forget to trust to notebook to run it.
 if u dont trust then it will not run.
 ctrl+enter to execute a single cell
 shift+enter to execute all the cells.
 always dont forget to use / while specifying a path, otherwise it will lead to a unicode escape character error.
 for eg, D:/AIII MY DATA/GUVIPROJECTS/Phonepe_Pulse_Data_Visualization/Data/ICN.png

ha i forgotten to tell u all onething, that is dont forget to add the environment variables , for python add the python folder and its scripts folder, an then move it to the top of the env variables.

if u done this after that also if u get an error , dont forget to uninstall the previous python launcher from apps, and then dont forget to delete the python folder of previous installation... and then open the new python installation use modify, and click the add to path . now the python 3.9 is installled.... mostly, python 3.9 only supports the older syntaxes , so dont forget to use it instead of python 3.12
 



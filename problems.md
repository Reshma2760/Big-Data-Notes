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

sometimes change the streamlit version as older one, it may also help u.

now !pip install will forcely install all the libraries..
if u get any error like pyhthjfm.py is missing means uninstall that lib, then install older or relevent to that, it my have that script files.

lastly, to install php use the XAMPP server. there u run as administrator that program, so that no errors may occur...
sometimes u may get an permission error . that time go to that folder and change the respective file sharing settings and for user allow all, then all will be done....

if u want to install all your files in local disk d then, do it go to windows registry entry and then go here.|

Computer\HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Windows\CurrentVersion 

change commonfilesdir , common files dir x86, commonw6432dir, progrmfilesdir, progrmfilesir x86, programw6432dir files change it to D:\ folder, and dont forget to copy this files to the :\folder from C:\

if u want to move an app, go to apps and feathes there click on : of app ,nd click on move, only supported apps may work



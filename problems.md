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


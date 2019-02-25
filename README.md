# server_issues
collection of server related issues, in progress

1. File transfer between remote (Ubuntu) servers:
   A file on source server is to be copied to a remote server. So on source server, input this
   scp -r file_dir+file user_name@target_server:destin_dir
   For instance, file pyodbc.tar.gz is copied to dir /x/z/des/ on server 10.xx.xx.xx, it's
   scp -r /x/j/pyodbc.tar.gz user_name@10.xx.xx.xx:/x/z/des/

2. File transfer from Windows to (Ubuntu) server:
   Via Putty.
   1) open cmd in windows, change directory to Putty, e.g. "cd C:\Program Files (x86)\Putty\", and type "pscp"
   2) upload file via Putty as the following command, make change as necessary.
   "pscp C:\files_directory\the_file.txt login_name@server_ip:/x/des_dir", then password.
   3) the file stays in /x/des_dir now.
   
3. install Teradata driver on Ubuntu server:
   
   apt remove nslcd, then everything is ok.

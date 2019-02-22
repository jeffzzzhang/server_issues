# server_issues
collection of server related issues, in progress

1. File transfer between remote servers:
   A file on source server is to be copied to a remote server. So on source server, input this
   scp -r file_dir+file user_name@target_server:destin_dir
   For instance, file pyodbc.tar.gz is copied to dir /x/z/des/ on server 10.xx.xx.xx, it's
   scp -r /x/j/pyodbc.tar.gz user_name@10.xx.xx.xx:/x/z/des/


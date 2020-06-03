![Untitled-2](https://user-images.githubusercontent.com/52716203/83064761-3b437980-a05a-11ea-96f6-49ad539c5cf3.png)

# file_transfer
 Python Network Programming - Basic Server 

  File transfer is the process of copying or moving a file from a computer to another over a network or Internet connection.
  
  The basic idea is to create a server that listens on a particular port, this server will be responsible for receiving files (you can make the server sends files as well).
  On the other hand, the client will try to connect to the server and send a file of any type.

  We are going to use socket module which comes built-in with Python and provides us with socket operations that are widely used on the Internet, as they are behind of any connection to any network.
  
  # Output on a local server:
        Server listening....
        Got connection from ('192.168.56.10', 62854)
        ('Server received', "'Hello server!'")
        ('Sent ', "'1 1234567890\\n
        ...
        ('Sent ', "'4567890\\n105
        ...
        ('Sent ', "'300 1234567890\\n'")
        Done sending
        
 # Output on a local client:
         file opened
        receiving data...
        data=1 1234567890
        2 1234567890
        ...
        103 1234567890
        104 123
        receiving data...
        data=4567890
        105 1234567890
        106 1234567890
        ...
        299 1234567890

        receiving data...
        data=300 1234567890
        Thank you for connecting
        receiving data...
        data=
        Successfully get the file
        connection closed

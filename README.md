# Echoserver
Echo server and client using python socket

# AIM:

To develop a simple webserver to serve html programming pages.

## DESIGN STEPS:

### Step 1:

Design of echo server and client using python socket

### Step 2:

Implementation using Python code

### Step 3:

Testing the server and client 

## PROGRAM:
## CLIENT:
```
import socket
HOST, PORT = '127.0.0.1', 65432
with socket.create_connection((HOST, PORT)) as s:
    s.sendall(b'VIJAY , 2122223230223')
    print(f'Received: {s.recv(1024)!r}')
 ```
## SERVER :
```
import socket
host,port='127.0.0.1',65432
with socket.create_server((host,port))as s:
    conn,addr=s.accept()
    with conn:
        print(f'connected by {addr}')
        while data :=conn.recv(1024):
            conn.sendall(data)
```


## OUTPUT:
![Screenshot 2025-03-06 113149](https://github.com/user-attachments/assets/dfbf27da-dd0c-4e15-9a51-68ca9cea03f4)

![Screenshot 2025-03-06 113200](https://github.com/user-attachments/assets/74d19c5f-15d7-4b45-9593-26414971f2aa)


## RESULT:
The program is executed successfully

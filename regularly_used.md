Port Open or Not

   ```bash
   sudo ss -tulnp
   ```
Explanation of the flags used:

- `-t: Displays TCP sockets.`
- `-u: Displays UDP sockets.`
- `-l: Shows only listening sockets.`
- `-n: Shows numerical addresses instead of resolving them to hostnames.`
- `-p: Shows the process using the socket.`

```bash
sudo lsof -i -P -n | grep LISTEN
```
Explanation of the flags used:

`-i: Selects the listing of files any of whose Internet address matches the address specified in the netstat command.`
`-P: Inhibits the conversion of port numbers to port names for network files.`
`-n: Shows numerical addresses.`
`grep LISTEN: Filters the output to display only listening ports.`



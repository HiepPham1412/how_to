1. ssh to remote server
2. In the remotew server trigger jupyter notebook run
```
jupyter notebook --no-browser --port 8889'
```
3. In the local machine, do ssh local port forward
```
ssh -N -L local-address:local-port:remote-address:remote-port remote-user@remote-host
```
"-N": don't execute any commands after the "tunnel" is established

"-L" a Local port forward to the remote machine (-R goes the other way).

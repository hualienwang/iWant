#iWant
##CLI based decentralized peer to peer file sharing


###Server
Run the server to spawn 3 daemon process
1. Server daemon = Interacts with filemonitoring daemon, client and Election daemon.
2. Election daemon = Election daemon is the heart of consensus among peers and  updates the server as soon as there is a leader change.
3. Filemonitor daemon = Filemonitor daemon looks for any changes in the folder you are sharing and informs the server daemon. The server daemon in turn updates the changes to the main Leader.

Then run client in another shell


To run server
```python
sudo python main.py
```

###Client 
To run instant search on filenames in the network
```python
python ui.py --search avengers
```

To download files 
```python
python ui.py --download <hash value of avengers>
```

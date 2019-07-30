# PY-KCP
1. python binding of kcp
2. simple tunnel implementation based asyncio module

### description
[KCP: A Fast and Reliable ARQ Protocol](https://github.com/skywind3000/kcp)

### platform
- python3.7
- arch linux

### install
```shell script
git clone https://github.com/yukityan/kcp-py.git
cd kcp-py
python3 setup.py install
```

### uninstall
```shell script
pip uninstall py_kcp
```

### usage

#### console_scripts
- kcp_local
```console
foo@bar:~$ kcp_local -h
usage: kcp_local [-h] -s SERVER -p SERVER_PORT -l LOCAL -t LOCAL_PORT [-m MTU]
                [-i {30,40,50}] [--nodelay] [-r {0,1,2}] [--nc] [-c CONFIG]

Python binding KCP tunnel.

optional arguments:
 -h, --help            show this help message and exit
 -s SERVER, --server SERVER
                       Host name or IP address of your remote server.
 -p SERVER_PORT, --server_port SERVER_PORT
                       Port number of your remote server.
 -l LOCAL, --local LOCAL
                       Host name or IP address your local server
 -t LOCAL_PORT, --local_port LOCAL_PORT
                       Port number of your local server.
 -m MTU, --mtu MTU     Maximum Transmission Unit for UDP packets (default:
                       1350)
 -i {30,40,50}, --interval {30,40,50}
                       Interval of KCP update (ms)
 --nodelay             KCP ack nodelay or delay
 -r {0,1,2}, --resend {0,1,2}
                       Fast resend
 --nc                  enable net control
 -c CONFIG, --config CONFIG
                       config file path
```
- kcp_server
```console
foo@bar:~$ kcp_server -h
usage: kcp_local [-h] -s SERVER -p SERVER_PORT -l LOCAL -t LOCAL_PORT [-m MTU]
                [-i {30,40,50}] [--nodelay] [-r {0,1,2}] [--nc] [-c CONFIG]

Python binding KCP tunnel.

optional arguments:
 -h, --help            show this help message and exit
 -s SERVER, --server SERVER
                       Host name or IP address of your remote server.
 -p SERVER_PORT, --server_port SERVER_PORT
                       Port number of your remote server.
 -l LOCAL, --local LOCAL
                       Host name or IP address your local server
 -t LOCAL_PORT, --local_port LOCAL_PORT
                       Port number of your local server.
 -m MTU, --mtu MTU     Maximum Transmission Unit for UDP packets (default:
                       1350)
 -i {30,40,50}, --interval {30,40,50}
                       Interval of KCP update (ms)
 --nodelay             KCP ack nodelay or delay
 -r {0,1,2}, --resend {0,1,2}
                       Fast resend
 --nc                  enable net control
 -c CONFIG, --config CONFIG
                       config file path
```
 


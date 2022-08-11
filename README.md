# Scripts using the Orange Livebox REST API

## Installation

```shell
python3 -m venv env
. env/bin/activate
pip install sysbus
sysbus -config
```

It will store the parameters to access the API in `~/.sysbusrc`.

## add-pinhole - Add an IPv6 firewall entry

### Add IPv6 firewall entry for a service for current host

```shell
./add-pinhole ssh
./add-pinhole https
./add-pinhole 443
.
```

### Add IPv6 firewall entry for a different host

```shell
./add-pinhole ssh 2a01:cb15:be:9999::1
```

### Add a name in Livebox web GUI

```shell
./add-pinhole ssh 2a01:cb15:be:9999::1 my-ssh
```

### Specify a different protocol (tcp or udp)

```shell
./add-pinhole 12345 2a01:cb15:be:9999::1 my-port udp
```


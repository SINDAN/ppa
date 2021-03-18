 ![SINDAN Project](https://raw.githubusercontent.com/SINDAN/sindan-docker/screenshot/logo.png)

# ppa

PPA owned by [@SINDAN](https://github.com/SINDAN) project - see [ppa branch](https://github.com/SINDAN/ppa/tree/ppa) for published packages.

## Getting started with your Raspberry Pi

Note that current PPA is only available for **Raspberry Pi OS Lite (buster) running on ARMv8**.
Import GPG key, add sources.list and update package lists by:

```
$ curl -fsSL https://dl.sindan-net.com/sindan.key | sudo apt-key add -
$ echo "deb https://dl.sindan-net.com $(lsb_release -cs) main" |\
  sudo tee /etc/apt/sources.list.d/sindan.list > /dev/null
$ sudo apt update
```

Make sure you can see some SINDAN products from our PPA.

```
$ apt search sindan
Sorting... Done
Full Text Search... Done
sindan-client/stable 2.3.3-1 armhf
  Wi-Fi monitoring solution - client

sindan-client-camp2103/stable 2.3.3-7 armhf
  Wi-Fi monitoring solution for WIDE-CAMP 2103 - client

sindan-manager-agent/stable 0.1-8 armhf
  Wi-Fi monitoring solution - local management agent (SINDAN Manager)

sindan-manager-agent-camp2103/stable 0.1-15 armhf
  Wi-Fi monitoring solution for WIDE-CAMP 2103 - local management agent (SINDAN Manager)
```

Then you can install packages as usual.

```
$ sudo apt upgrade -y
$ sudo apt install -y sindan-manager-agent
```

## Maintainers

- **Taichi MIYA** - [@mi2428](https://github.com/mi2428)


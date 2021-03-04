 ![SINDAN Project](https://raw.githubusercontent.com/SINDAN/sindan-docker/screenshot/logo.png)

# ppa

PPA owned by [@SINDAN](https://github.com/SINDAN) project - see [ppa branch](https://github.com/SINDAN/ppa/tree/ppa) for published packages.

## Getting started with your Raspberry Pi

Note that current PPA is only available for **Raspbian (buster) running on ARMv7**.
Import GPG key, add sources.list and update package lists by:

```
$ curl -fsSL https://dl.sindan-net.com/sindan.key | sudo apt-key add -
$ echo "deb https://dl.sindan-net.com $(lsb_release -cs) main" |\
  sudo tee /etc/apt/sources.list.d/sindan.list > /dev/null
$ sudo apt update
```

Make sure you can see some packages from our PPA.

```
$ apt search sindan-manager-agent
Sorting... Done
Full Text Search... Done
sindan-manager-agent/stable 0.1-5 armhf
  Local management agent for SINDAN Manager

sindan-manager-agent-camp2103/stable 0.1-6 armhf
  Local management agent for SINDAN Manager customized for WIDE-CAMP 2103
```

Then you can install packages as usual.

```
$ sudo apt upgrade -y
$ sudo apt install -y sindan-manager-agent
```

## Maintainers

- **Taichi MIYA** - [@mi2428](https://github.com/mi2428)


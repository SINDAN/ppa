# ppa

PPA owned by [@SINDAN](https://github.com/SINDAN) project - see [ppa branch](https://github.com/SINDAN/ppa/tree/ppa) for published packages.

## Getting started with your Raspberry Pi

Note that current PPA is only available for **Raspbian (buster) running on ARMv7**.
Import GPG key, add sources.list and update package lists by:

```
$ curl -s https://sindan.github.io/ppa/sindan.key | sudo apt-key add -
$ echo "deb https://sindan.github.io/ppa buster main" | sudo tee /etc/apt/sources.list.d/sindan.list
$ sudo apt update
```

Make sure you can see some packages from our PPA.

```
$ apt search sindan-manager-agent
Sorting... Done
Full Text Search... Done
sindan-manager-agent/stable 0.1-3 armhf
  Local management agent for SINDAN Manager
```

Then you can install packages as usual.

```
$ sudo apt install -y sindan-manager-agent
```

## Maintainers

- **Taichi MIYA** - [@mi2428](https://github.com/mi2428)


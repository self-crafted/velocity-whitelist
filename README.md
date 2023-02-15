# velocity-whitelist

[![standard-readme compliant](https://img.shields.io/badge/standard--readme-OK-green.svg?style=flat-square)](https://github.com/RichardLitt/standard-readme)
[![GitHub](https://img.shields.io/github/license/self-crafted/velocity-whitelist?style=flat-square&color=b2204c)](https://github.com/self-crafted/velocity-whitelist/blob/master/LICENSE)
[![GitHub Repo stars](https://img.shields.io/github/stars/self-crafted/velocity-whitelist?style=flat-square)](https://github.com/self-crafted/velocity-whitelist/stargazers)
[![GitHub forks](https://img.shields.io/github/forks/self-crafted/velocity-whitelist?style=flat-square)](https://github.com/self-crafted/velocity-whitelist/network/members)
[![GitHub release (latest SemVer)](https://img.shields.io/github/v/release/self-crafted/velocity-whitelist?style=flat-square)](https://github.com/self-crafted/velocity-whitelist/releases/latest)
[![GitHub all releases](https://img.shields.io/github/downloads/self-crafted/velocity-whitelist/total?style=flat-square)](https://github.com/self-crafted/velocity-whitelist/releases)

Dead simple player whitelist for Minecraft Velocity proxy.

velocity-whitelist is built for my private network, so it may or may not fit your needs.
It adds no commands to interface with it. 
All attempts on joining the proxy are blocked, unless the players UUID is in a textfile named `whitelist.txt`.

## Table of Contents

- [Install](#install)
- [Usage](#usage)
- [Maintainers](#maintainers)
- [Contributing](#contributing)
- [License](#license)

## Install
You could either just download a [release](https://github.com/self-crafted/velocity-whitelist/releases) or you compile the server yourself using the following commands under Linux
```shell
git clone https://github.com/self-crafted/velocity-whitelist.git
cd velocity-whitelist
./gradlew build
```
The server jar will be located at `build/libs/velocity-whitelist-<VERSION>.jar`.

Note that for compiling you need to use a JDK 17.

## Usage
To use this plugin you need to run Java 17.
The file `whitelist.txt` is read every 10 seconds. So simply drop the UUIDs of friends and family in there.
You can write comments starting the line with `#` or `//`.
Player names can't be used. The plugin will accept UUIDs only.

```
# valid comment
<valid UUID>
// another valid comment
  <valid UUID>
```

## Maintainers

[@offby0point5](https://github.com/offby0point5)

## Contributing

PRs accepted.

Small note: If editing the README, please conform to the [standard-readme](https://github.com/RichardLitt/standard-readme) specification.

## License

This project is licensed under the [MIT license](LICENSE).

# hypriot-rpi-noip

Helper scripts to run the NoIP client on Raspberry Pi.

### Assumptions

- You have `docker` installed and working on Raspberry Pi
  - [HypriotOS][hypriot-os]
  - [ResinOS][resin-os]
  - [Rasbpian + Docker][raspbian-docker]
- Your no-ip config files will be mounted from the host at: `/mnt/data/no-ip`
- You always want this container running (`--restart=always`)

### Usage

```
./bin/configure.sh
# Enter your no-ip user and password, select an update interval
./bin/start.sh
```

### Docs

Uses docker image:

- [`hypriot/rpi-noip`](https://hub.docker.com/r/hypriot/rpi-noip/)
- [`Dockerfile`](https://github.com/hypriot/rpi-noip/blob/master/Dockerfile)

For more help using this image, please see upstream documentation:

 - [`hypriot/rpi-noip` README](https://github.com/hypriot/rpi-noip)

# License

MIT

[hypriot-os]: https://blog.hypriot.com/about/#hypriotos:6083a88ee3411b0d17ce02d738f69d47
[resin-os]: https://resin.io/
[raspbian-docker]: https://github.com/umiddelb/armhf/wiki/Get-Docker-up-and-running-on-the-RaspberryPi-(ARMv6)-in-four-steps-(Wheezy)

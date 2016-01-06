# Transmission

This is a fork of github.com/dperson/transmission with a simple change for my use case (alow modification of settings.json). All credits to dperson and the team maintaining this image.

Supports docker stop and start.

> Usage:
> docker pull surenot/transmission
> docker run -d surenot/transmission -p 9091:9091 \
>    [--name <container_name>] \
>    [-v <host_settings_path>:/var/lib/transmission-daemon/info] \
>    [-v <host_download_path>:/var/lib/transmission-daemon/downloads]

This image supports `docker stop`, `docker start`, and `docker restart` without erasing custom settings.

Options supported by dperson/transmission are also supported with a slight change in behavior regarding to the default username and password, for these refer to transmission documentation (transmission/transmission as of this 2016/01/06).


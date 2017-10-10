# Minerva Project

Minerva, daughter of Jupiter and Metis, goddess of wisdom and strategic warfare and sponsor
of **arts**, **trade** and **strategy**.

She was the virgin goddess of music, poetry, medicine, wisdom, commerce, weaving and the
crafts.

*Trivia courtesy of [Wikipedia]*

----

Minerva is my HTPC project. It's a work in progress, so you are welcome to suggest
improvements!

# About the project

:construction: This area is under construction

# Requirements

Minerva is a docker configuration that aims to provide you everything you need to set up your own
HTPC. This is far from perfect and I'll be updating this as I work on my own settings.

# Included Software

 - [Transmission] - For torrent downloading
 - [Sonarr] - For TV shows management
 - [Radarr] - For Movies Management
 - [Plex] - The media server solution

# Requirements

You'll need an updated [docker] installed on your computer to run Minerva. Currently I'm
running `Docker CE Version 17.09-0`.

You'll need to edit your `hosts` file, so you can point Minerva Containers to their hostnames.

This should be enough to make Minerva ready for you to set up.

# Default Settings

I've included default settings for Sonarr and Raddar, that already have Transmission configured as
their download clients. You can manually copy them files to their location before starting or you
can use the included scripts to perform these tasks. Please, note, if you run the scripts after
adding your own configuration, it will be overwritten by a fresh database containing only the
Transmission Client configured. So run this before you start configuring your Sonarr and Radarr
instances.

# Set up

 - Copy the file `docker-env.example` to `.env` and edit accordingly. The only thing you really need to
care about in this file are the `PGID` and `PUID`. Ensure they are the same as the user you wish to
run the containers as. You may create a user just for this or you can use your own user. You can use
the command `id $(whoami)` to find you user id. Linux boxes usually have `1000` as your UID and
macOS usually 501 (it may vary).

 - Clone this repository, cd into it and run `docker-compose up -d`

 - Add the following to your hosts file:

```
# Minerva
127.0.0.1 transmission.minerva
127.0.0.1 plex.minerva
127.0.0.1 sonarr.minerva
127.0.0.1 radarr.minerva
```

 - I recommend you run both scripts so Transmission will be configured before anything else:

```
$ ./scripts/radarr-default
```

```
$ ./scripts/sonarr-default
```

 - Now point your browser to [http://sonarr.minerva:8989][sonarr-minerva] and make sure you see the
Sonarr home screen.

# Configuring included software

:construction: This area is under construction

 - Sonarr URL: http://sonarr.minerva:8989
 - Radarr URL: http://radarr.minerva:7878
 - Plex URL: http://plex.minerva:32400/web
 - Transmission URL: http://transmission.minerva:9091

# TO-DO

 - [ ] Add [Organizr][organizr] or some other friendly front-end
 - [ ] Add an NGINX Proxy to drop ports on hostnames
 - [ ] Make a better README
 - [ ] Check if this is the best docker configuration that we should use
 - [ ] Make a logo for this
 - [ ] Move this TO-DO list to a proper issue

[wikipedia]: https://en.wikipedia.org/wiki/Minerva
[sonarr]: http://sonarr.tv
[radarr]: http://radarr.tv
[transmission]: https://transmissionbt.com/
[plex]: http://plex.tv
[docker]: http://docker.com
[organizr]: https://github.com/causefx/Organizr
[sonarr-minerva]: http://sonarr.minerva:8989

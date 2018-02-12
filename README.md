# docker-adblock

## About
A simple container based adblocker with daily automatic blocklist updates. 

## Docker Hub
The following images are utilised:
- [rossbannerman/dnsmasq](https://hub.docker.com/r/rossbannerman/dnsmasq/)
- [rossbannerman/adblock_blocklist_updater](https://hub.docker.com/r/rossbannerman/adblock_blocklist_updater/)

## Usage
1. Add your upstream nameservers of choice to `${PWD}/conf/resolv.conf` (eg. 8.8.8.8, 8.8.4.4)
2. Run `docker-compose up -d`
3. Point the DNS config of your host(s) to the IP of your docker host (and/or localhost if using locally)

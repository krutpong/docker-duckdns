# docker-duckdns

This is a simple Docker container for running the [Duck DNS](http://duckdns.org) dynamic DNS update script. It will keep your domain.duckdns.org DNS alias up-to-date as your home IP changes. The script runs every 5 minutes.

## Usage

This docker image is available as a [trusted build on the docker index](https://index.docker.io/u/coppit/duckdns/).

Run:

`sudo docker run --name=duckdns --restart always -d -e "ENV_DOMAIN=domain" -e "ENV_TOKEN=token" robinwl/duckdns`

To check the status, run `docker logs duckdns`.

## Credits

[Duck DNS](http://duckdns.org)
[httpbin](http://httpbin.org/)

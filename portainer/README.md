# Portainer

[Portainer](https://www.portainer.io/) is a web-based continer management solution. 

Follow the steps in the [deploying section of the main README](../README.md#deploying) to create the stack on Portainer, using the compose path and environment variables below.

> [!IMPORTANT]
> The name you set as the *stack* name, will be used as the subdomain of the domain you set with the environment variable `DOMAIN`.
 
## Compose path

The compose path for this stack is:
```
portainer/docker-compose.yml
```

## Environment variables

### `IP_WHITELIST`

This environment variable is used to set the allowed IPs (or ranges of allowed IPs by using CIDR notation).

Example values: `127.0.0.1/32, 192.168.1.7`

> Read more about it in the [Traefik documentation](https://doc.traefik.io/traefik/middlewares/http/ipwhitelist/).

### `SERVER_TYPE`

For a test server, we recomment to use `tst` and for a production server, `prd`. 

### `DOMAIN`

Specify the domain that will be used; for a test server we recomend to prefix this with `tst.`, so:

* for a test  server, set e.g. `DOMAIN=tst.energietransitiewindesheim.nl`
* for a production server, set e.g. `DOMAIN=energietransitiewindesheim.nl`

So, if you  specified  `portainer` as the stack name, the fully qualified domains will become:

* test server: `https://portainer.tst.energietransitiewindesheim.nl`
* production server: `https://portainer.energietransitiewindesheim.nl`


## First time log in

\<TO BE DOCUMENTED\>

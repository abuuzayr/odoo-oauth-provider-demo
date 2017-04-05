# odoo-oauth-provider-demo/odoo-client

This set up the odoo instance under docker: `odoo-client`.

# Pre-requisites

1. The latest version of `docker` is installed.
2. The latest version of `docker-compose` is installed.
3. [smecen/nginx](https://git.groventure.com/smecen/nginx) is running.
4. [smecen/test-certs](https://git.groventure.com/smecen/test-certs)
   cloned in the same parent directory as this project.
5. An entry in your `hosts` file with the mapping: `127.0.0.1
   odoo.oauth-client`.

# Instructions

1. `cd` into this directory.
2. Run `docker-compose up`.

You should see an odoo login page at 'http://odoo.oauth-client/'.

# Deleting all data

Should you need to delete all data, execute this command:

```shell
docker-compose down; docker volume rm odooclient_odoo{,-postgresql}-data.oauth-client

```

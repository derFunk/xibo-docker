# xibo-docker
Docker container for the Xibo Digital Signage CMS

# Environment variables

Pass these environment variables when running the container to modify settings:

Variable Name | Description | Default Value
--------------|-------------|--------------
MYSQL_HOST    | The MySQL Hostname/IP | localhost
MYSQL_PASS    | A MySQL user "admin" will be created, this is his password | changeme
XIBO_ADMIN_PASS | A Xibo user "admin" will be created, this is his password | changeme
MYSQL_DBNAME | The name of the database which should be created for Xibo | xibo


# Running the container

`docker run -p 80:80 -e XIBO_ADMIN_PASS=secret -e MYSQL_PASS=topsecret chimeradev/xibo`

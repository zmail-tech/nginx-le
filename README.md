# nginx-le
Nginix proxy for docker containers with LE integration based on jwilder proxy

# Description
This compose file is the basis for all of my docker projects. Any docker webservices run while this is in affect will automatically have an https 
certificate generated and be proxied through.

This allows automatic LE creation and renewal without any interaction from the admin and allows multiple websites to be run from one static IP address.

# Deployment
Add your email into the docker-compose.yml file in the spot designated. This is use for LE automation

Then run 
> docker-compose up -d

# Notes
Usually the nginx directory is dynamic and does not need to be mounted in as a volume. However in some cases modifications need to be manually made to the files
that allow for changes to persist by mounting it as a volume

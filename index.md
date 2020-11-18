## Home Server Gandolf Like!
### Startup

Edit the docker-compose.yml file to your liking 

```markdown
- environment variables (DOMAIN & DOMAIN@EMAIL)
- change root password of Maria-DB
- change persistant data volumes for the containers
```

Before you start up the containers for this to work you need to create a seperate network.

```markdown
-$ docker network create nginx-proxy
```

Don't just spin up everything spin up the database first.

```markdown
-$ docker-compose up -d db
```

After you let that start up spin up the rest.

```markdown
-$ docker-compose up -d
```
Once you have done this let LetsEncrypt get the certs and everything set up, it may take awhile so be patient.

Now access your DOMAIN and do the initial setup of NextCloud and your all set.

To update all of your containers with the latest updates use the commands below:

```markdown
(stops and removes these containers)
-$ docker-compose down 

(pulls the new updated images)
-$ docker-compose pull 

(starts your containers with the new updated images)
-$ docker-compose up -d 
```

In the "docker-compose.yml" are the Factorio Server disabled.
Try to enable and change ports and stuff!

### Support or Contact

Check out my [github](https://github.com/Gandolf90/home-server) 
# Nexus repository oss

The free artifact repository with universal format support.

* Single source of truth for all of your components, binaries, and build artifacts.
* Efficiently distribute parts and containers to developers.
* Deployed at more than 100,000 organizations globally.

Supports Nexus push command for composer.

## Configure and install

Copy `.env.example` to `.env`

Edit `.env` and update the `NEXUS_DATA_DIR` parameter.

Run container:
```
docker-composer up -d --build
```

## Repository manager

Navigate to [http://localhost:8081](http://localhost:8081)

The repository manager ships with two users by default: admin and anonymous. 
The admin user has all privileges and the anonymous user has read-only privileges. 
The initial password for the admin user can be found in an `admin.password` file found in the
 ``NEXUS_DATA_DIR`` directory after starting the server. 

## Links

* https://www.sonatype.com/nexus-repository-oss
* https://hub.docker.com/r/sonatype/nexus3/
* https://community.sonatype.com/t/nexus-repository-3-composer-php-format/1321
* https://blog.sonatype.com/using-nexus-3-as-your-repository-part-2-npm-packages
* https://github.com/Elendev/nexus-composer-push

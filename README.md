# DevOpsWithDocker
DevOps with Docker courses exercises

The [course](https://docker-hy.github.io/) is an introductory course to Docker and docker-compose and their usage in single host deployments. Course will also introduce other container management tools.

Course also looks into what different parts web services consist of such as reverse proxies, caches and databases.

## Usefull commands

``` $ docker pull "name" 
    $ docker images
    $ docker run "name"
    $ docker ps -a
``` 
-The **pull** command fetches the busybox image from the Docker registry and saves it to our system
-Use **docker images** command to see a list of all images on your system
- **Run** commnd runs a Docker container based on this image. the Docker client finds the image, loads up the container and then runs a command in that container.
- Use **ps -a** to see a list of all containers that we ran.

```
$ docker run -it "name" sh
/ # ls
bin   dev   etc   home  proc  root  sys   tmp   usr   var
/ # uptime
 05:45:21 up  5:58,  0 users,  load average: 0.00, 0.01, 0.04
/ # exit 
$ docker run -it "name" sh
``` 
Running the **run command with the -it flags** attaches us to an interactive tty in the container. Now we can run as many commands in the container as we want. Take some time to run your favorite commands.You can exit the container typing **exit** and  Enter and then start it up again with the **docker run -it busybox sh** command. 

## Links
https://docs.docker.com/
https://docker-curriculum.com/

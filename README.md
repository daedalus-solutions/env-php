# PHP Environment
This is a generic php docker container that has most of the commonly required components for hosting a php based website.
The container expects the root of the application to be placed inside /var/www/site

The suggested usage of this image is to create a virtual directory on the host system that points to the containers /var/www/site container
```
docker -run -v /var/www/sites/<containerfolder>:/var/www/site ...
```
This means that the host folder can be changed and the container just uses the changes. This also means that if the container is stopped and started again, the data is still sitting on the host system

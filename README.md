# docker-localdev
Storage space for docker httpd setup scripts and website code.



## docker-compose.yml

The above docker-compose file is my attempt at creating an automated solution for easily building local web servers using docker. To create a new site, you just need to change a single value in the service name, container name, port number, and folder name. This is usually done using version numbers and I suggest simply incrementing by number (website1, website2, website3; port 8081, port 8082, etc) for simplicity and organization. 

Of course, you can name them anything you want, it's only important that the names are unique to their own container. This also scales very nicely, as this process can be done pretty much indefinitely up to hundreds of sites. In the near future i'd like to find a way to automate that process as well, but until now this is much quicker than the alternatives, where we can have a new site set up with it's own folder and index.html in under a minute, and them simply running docker compose up -d. 

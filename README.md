# wordpress-local-environment
A local Wordpress / mysql / phpadmin setup for development purposes. 

## How to get started 

Requirements:
- docker (recommend Docker Desktop)

## Setup

First git clone this repository then enter the directory. 
Once you do this you can this command

`docker-compose up -d`

This will start a basic deployment of wordpress with a local mysql database. 
In addition to that phpadmin is installed to allow you an easy way to inspect the database. 

While it is a local installation, the passwords and such are pretty much place holders. I recommend you change them if you plan on using this for anything more than local development. 

Important local links: 

http://localhost:9000  (wordpress)

http://localhost:9090  (phpadmin for dbase debugging)

There is a content and database volume.  Those should be set as persistent docker volumes in the docker-compose.yml file, but if you want to easily access the files without going into the docker VM, use the mapping as it is so you can update things and or commit files to your own wordpress repo.  

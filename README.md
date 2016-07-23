# symfony-admin-starter-kit
This is an easy way to start with [sonata admin](https://sonata-project.org/).

## What's under the hood?
This build contains:
* [Docker](https://docs.docker.com/) support - the easiest way for now to build and delivery projects.
* [Symfony 2.8](http://symfony.com/doc/2.8/book/index.html) - modern framework which gives you a chance to create you app faster.
* [SonataAdminBundle](https://sonata-project.org/bundles/) - the greatest tool for building own admin panel in a seconds.
* [FOSUserBundle](https://github.com/FriendsOfSymfony/FOSUserBundle) - a bundle for user management.

## How to run it
* Copy parameters.yml file in docker folder with command

`cp ./docker/parameters.yml.dist ./docker/parameters.yml`

* Run containers with a command

`docker-compose up -d`

* Create tables in the database 

`docker-compose run --rm admin-panel app/console doctrine:schema:update --force`

* Create admin user 

`docker-compose run --rm admin-panel app/console fos:user:create admin admin admin --super-admin`

* Go to [http://192.168.99.100:8000/admin/](http://192.168.99.100:8000/admin/) in your browser.

* Enjoy

![Sonata Admin Panel](http://g.recordit.co/EMsRl0fZKv.gif)

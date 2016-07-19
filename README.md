# symfony-admin-starter-kit
This is the simplest way to start [sonata admin]() project.

## What's under the hood?
This build contains:
* [Docker](https://docs.docker.com/) support - the easiest way for now to build and delivery projects.
* [Symfony 2.8](http://symfony.com/doc/2.8/book/index.html) - modern framework which gives you a chance to create you app faster.
* [SonataAdminBundle](https://sonata-project.org/bundles/) - the greatest tool for building own admin panel in a seconds.
* [FOSUserBundle](https://github.com/FriendsOfSymfony/FOSUserBundle) - a bundle for user management.

## How to run it
* Copy parameters.yml file in docker folder with command `cp ./docker/parameters.yml.dist ./docker/parameters.yml`
* Run containers with command `docker-compose up` 
* Go to [http://192.168.99.100:8000/admin/](http://192.168.99.100:8000/admin/) in your browser.
* Enjoy

![Sonata Admin Panel](https://i.gyazo.com/80e8b73196c75d14653fe3c55fc39f3a.png)

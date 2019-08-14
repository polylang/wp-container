# Wordpress Container

A basic WordPress Docker container for manual testing plugins and themes

## Prerequisistes

You need to have a local installation of the [Docker Engine](https://docs.docker.com/engine/) and [Docker Compose](https://docs.docker.com/compose/) to use these images on your computer.

## Instructions

1. Clone this directory.
2. Copy the plugins and themes you want to use in the `plugins` and `themes` folders respectively.
3. In a terminal, enter the following command from inside the `wp-container` folder: `docker-compose up`. (Note: If your OS is a Linux distribution, you may have to run this command with root privileges, check for details in [docker's official documentation](https://docs.docker.com/install/linux/linux-postinstall/) ).
4. Open your browser and browse the following url: `http://localhost:8000`
5. Follow the steps of WordPress' 'five minutes installation'.
6. Go to *Plugins > Installed Plugins* and activate the plugins you want to use.
7. Go to *Appearance > Themes* and select the theme you want to use.
8. After you've finished using this container, remove it by using the command: `docker-compose down --volumes`. This will destroy the container and then all created data will be lost.

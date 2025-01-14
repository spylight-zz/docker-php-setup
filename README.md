# Setup PHP environment dev on Docker
This is for my learning and note on nextime, this is my setup for development web using PHP on Docker.
if you want, please use it for your development,

------------
#### Prerequisites
Docker must be installed on your system / server

------------

#### Features

My setup are using Ubuntu 24.04 and installed :
1. PHP 8.1 and PHP 7.4 (you can see on folder imageXX)
2. Ruby
3. Some utilities 
	- unzip
	- mcrypt
	- bzip2
	- chrpath libssl-dev libxft-dev
	- libfreetype6 libfreetype6-dev libfontconfig1 libfontconfig1-dev
4. Apache2
5. Git
6. Composer

------------
#### How To
1. Open your terminal 
2. Navigate to setup  `cd docker-php-setup`
3. Build image `docker build -t docker-php ./image74` or other version
    if finish build the image, you can check with `docker image ls`
4. Run `docker-compose up -d`, see docker-compose.yml settings
5. Done, but if you want to access the terminal console, run with this command `docker exec -it docker-php-setup_php_1 bash`

All is ok, you can check your browser and open http://localhost:5000 you will see your web server 
to navigate database you can open http://localhost:5050 with the login username : root and password : toor

to add/edit your PHP file/project you can navigate on folder `myapplication`

That's it and Happy Coding :smile:
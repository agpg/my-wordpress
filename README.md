


1. Install the docker instance.
     # sudo apt-get install -y --no-install-recommends     apt-transport-https     ca-certificates     curl     software-properties-common
   # curl -fsSL https://apt.dockerproject.org/gpg | sudo apt-key add -
   # apt-key fingerprint 58118E89F3A912897C070ADBF76221572C52609D
   # sudo add-apt-repository        "deb https://apt.dockerproject.org/repo/ \
       ubuntu-$(lsb_release -cs) \
       main"
   # sudo apt-get update
   # sudo apt-get -y install docker-engine
   # sudo apt-get -y install docker-engine
   #  apt-cache madison docker-engine
   #  sudo apt-get -y install docker-engine=1.13.1-0
   #  sudo apt-get -y install docker-engine=1.13.1
   #  sudo apt-get -y install docker-engine=1.13.1-0~ubuntu-trusty

2. Generate the self signed ssl certificate.
 
               # sudo openssl req -x509 -nodes -days 730 -newkey rsa:2048 -keyout blog.domain.com.key -out blog.domain.com.crt
       # openssl rsa -in blog.domain.com.key -out blog.domain.com.key
       # wget http://www.startssl.com/certs/sub.class1.server.ca.pem
       # cat blog.domain.com.crt sub.class1.server.ca.pem > blog.domain.com.crt.new
       # mv -f blog.domain.com.crt.new blog.domain.com.crt

3. Geneatre the wordp[ress data content:

   #sudo docker run -d -v /var/lib/mysql -v /var/www/html/wp-content --name wordpress1_data debian:jessie
   
4. Pull and start the mariadb database instance container.
  #sudo docker run -d --restart=always --name wordpress1_mariadb --volumes-from wordpress1_data -e MYSQL_ROOT_PASSWORD=Passw0rd123 mariadb
   
5. Pull and run  wordpress container with link with mariah database.
  #sudo docker run -d --restart=always --name wordpress1 --volumes-from wordpress1_data --link wordpress1_mariadb:mysql -e VIRTUAL_HOST=node02.example.com wordpress
  
6. Start Nginx-proxy server to direct to wordpress with ssl.  

 sudo docker run -d --restart=always --name nginx-proxy --security-opt=label:type:docker_t -p 80:80 -p 443:443 -v /home/certs:/etc/nginx/certs -v /var/run/docker.sock:/tmp/docker.sock jwilder/nginx-proxy

7. connect to wordpress convaincre:

   docker exec -i -t wordpress1 /bin/bash

8. Install MailCatcher in wordpress:

    apt-get install -q -y \ libsqlite3-dev \ ruby \ ruby-dev \ build-essential
    apt-get install -q -y \ libsqlite3-dev \ ruby \ ruby-dev \ build-essential
    apt-get install -y libsqlite3-dev ruby ruby-dev build-essential
    apt-get install -y  ruby
    gem install --no-ri --no-rdoc mailcatcher

9. Install wp cli :

    curl -O https://raw.githubusercontent.com/wp-cli/builds/gh-pages/phar/wp-cli.phar
    php wp-cli.phar --info
    chmod +x wp-cli.phar
    sudo mv wp-cli.phar /usr/local/bin/wp
    mv wp-cli.phar /usr/local/bin/wp
    wp --info

10. opne the wordpress throguh browser:

     htpps://hostname/
     
     
 11. newly created image file which wordpress with mailcatcher and wp cli.
 
     agpg/wordpress1    
     
      you can use if you dont want stesp to do 5,8,9 steps.
   
  

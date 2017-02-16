{\rtf1\ansi\ansicpg1252\cocoartf1504
{\fonttbl\f0\fswiss\fcharset0 Helvetica;\f1\fnil\fcharset0 Menlo-Regular;\f2\fmodern\fcharset0 Courier;
}
{\colortbl;\red255\green255\blue255;\red0\green0\blue0;\red255\green255\blue255;\red0\green0\blue0;
}
{\*\expandedcolortbl;\csgray\c100000;\csgray\c0;\csgray\c100000;\cssrgb\c0\c0\c0;
}
\margl1440\margr1440\vieww25100\viewh13380\viewkind0
\pard\tx720\tx1440\tx2160\tx2880\tx3600\tx4320\tx5040\tx5760\tx6480\tx7200\tx7920\tx8640\pardirnatural\partightenfactor0

\f0\fs24 \cf0 \
\
\
1. Install the docker instance.\
     # 
\f1\fs22 \cf2 \cb3 \CocoaLigature0 sudo apt-get install -y --no-install-recommends     apt-transport-https     ca-certificates     curl     software-properties-common\
\pard\tx560\tx1120\tx1680\tx2240\tx2800\tx3360\tx3920\tx4480\tx5040\tx5600\tx6160\tx6720\pardirnatural\partightenfactor0
\cf2    # curl -fsSL https://apt.dockerproject.org/gpg | sudo apt-key add -\
   # apt-key fingerprint 58118E89F3A912897C070ADBF76221572C52609D\
   # sudo add-apt-repository        "deb https://apt.dockerproject.org/repo/ \\\
       ubuntu-$(lsb_release -cs) \\\
       main"\
   # sudo apt-get update\
   # sudo apt-get -y install docker-engine\
   # sudo apt-get -y install docker-engine\
   #  apt-cache madison docker-engine\
   #  sudo apt-get -y install docker-engine=1.13.1-0\
   #  sudo apt-get -y install docker-engine=1.13.1\
   #  sudo apt-get -y install docker-engine=1.13.1-0~ubuntu-trusty
\f0\fs24 \cf0 \cb1 \CocoaLigature1 \
\pard\tx720\tx1440\tx2160\tx2880\tx3600\tx4320\tx5040\tx5760\tx6480\tx7200\tx7920\tx8640\pardirnatural\partightenfactor0
\cf0 \
2. Generate the self signed ssl certificate.\
 \
\pard\tx720\tx1440\tx2160\tx2880\tx3600\tx4320\tx5040\tx5760\tx6480\tx7200\tx7920\tx8640\pardirnatural\partightenfactor0
\cf0                # 
\f2 \cf4 \expnd0\expndtw0\kerning0
sudo openssl req -x509 -nodes -days 730 -newkey rsa:2048 -keyout blog.domain.com.key -out blog.domain.com.crt\
\pard\pardeftab720\sl280\partightenfactor0
\cf4        # openssl rsa -in blog.domain.com.key -out blog.domain.com.key\
       # wget http://www.startssl.com/certs/sub.class1.server.ca.pem\
       # cat blog.domain.com.crt sub.class1.server.ca.pem > blog.domain.com.crt.new\
       # mv -f blog.domain.com.crt.new blog.domain.com.crt
\f0 \cf0 \kerning1\expnd0\expndtw0 \
\pard\tx720\tx1440\tx2160\tx2880\tx3600\tx4320\tx5040\tx5760\tx6480\tx7200\tx7920\tx8640\pardirnatural\partightenfactor0
\cf0 \
3. Geneatre the wordp[ress data content:\
\
\pard\tx560\tx1120\tx1680\tx2240\tx2800\tx3360\tx3920\tx4480\tx5040\tx5600\tx6160\tx6720\pardirnatural\partightenfactor0

\f1\fs22 \cf2 \cb3 \CocoaLigature0    #sudo docker run -d -v /var/lib/mysql -v /var/www/html/wp-content --name wordpress1_data debian:jessie\
   \
4. Pull and start the mariadb database instance container.\
  #sudo docker run -d --restart=always --name wordpress1_mariadb --volumes-from wordpress1_data -e MYSQL_ROOT_PASSWORD=Passw0rd123 mariadb\
   \
5. Pull and run  wordpress container with link with mariah database.\
  #sudo docker run -d --restart=always --name wordpress1 --volumes-from wordpress1_data --link wordpress1_mariadb:mysql -e VIRTUAL_HOST=node02.example.com wordpress\
  \
6. Start Nginx-proxy server to direct to wordpress with ssl.  \
\
 sudo docker run -d --restart=always --name nginx-proxy --security-opt=label:type:docker_t -p 80:80 -p 443:443 -v /home/certs:/etc/nginx/certs -v /var/run/docker.sock:/tmp/docker.sock jwilder/nginx-proxy\
\
7. connect to wordpress convaincre:\
\
   docker exec -i -t wordpress1 /bin/bash\
\
8. Install MailCatcher in wordpress:\
\
    apt-get install -q -y \\ libsqlite3-dev \\ ruby \\ ruby-dev \\ build-essential\
    apt-get install -q -y \\ libsqlite3-dev \\ ruby \\ ruby-dev \\ build-essential\
    apt-get install -y libsqlite3-dev ruby ruby-dev build-essential\
    apt-get install -y  ruby\
    gem install --no-ri --no-rdoc mailcatcher\
\
9. Install wp cli :\
\
    curl -O https://raw.githubusercontent.com/wp-cli/builds/gh-pages/phar/wp-cli.phar\
    php wp-cli.phar --info\
    chmod +x wp-cli.phar\
    sudo mv wp-cli.phar /usr/local/bin/wp\
    mv wp-cli.phar /usr/local/bin/wp\
    wp --info\
\
\
   }
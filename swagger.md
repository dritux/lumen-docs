## Docs Swagger
```
composer require gossi/swagger
```

#### IBM swagger
```
sudo apt-get install linux-libc-dev
sudo apt-get install php7.0-dev
sudo apt-get install gcc make autoconf libc-dev pkg-config
sudo pecl install yaml-2.0.0
/usr/lib/php/20151012/yaml.so

/etc/php/7.0/mods-available/

php tools/swagger-to-html.php salesconnect.swagger/MASTER.yaml --set demo > c:/swagger/salesconnectAPI.html
```

#### Pretty swag
```
https://twskj.github.io/pretty-swag/

sudo apt-get install -y nodejs
sudo apt install npm

npm install pretty-swag -g
sudo ln -s /usr/bin/nodejs /usr/bin/node
pretty-swag -i swagger.json -o output.html
```

#### bootprint
```
npm install -g bootprint
npm install -g bootprint-swagger
bootprint swagger http://petstore.swagger.io/v2/swagger.json target
```

#### Swagger codegen
```
wget http://central.maven.org/maven2/io/swagger/swagger-codegen-cli/2.2.2/swagger-codegen-cli-2.2.2.jar -O swagger-codegen-cli.jar
java -jar swagger-codegen-cli.jar generate -i swagger.json -l dynamic-html
```

#### swagger editor
```
git clone http://github.com/itayB/swagger-editor.git
cd swagger-editor
npm install
npm start
```
#### Urls

[Yaml](https://forum.phalconphp.com/discussion/13753/config-yaml-in-php-7)

# qbox-docker
Código-fote para usar containers docker no projeto QBox


```yaml

version: '3'

services:
    # wwwapp:
    #     image: php:7.1.8-cli
    #     volumes:
    #         - "../src:/src"
    #     ports:
    #         - "8000:8000"
    db:
        image: mysql
        # volumes:
        #     - "./.data/db:/var/lib/mysql"
        restart: always
        environment:
          MYSQL_ROOT_PASSWORD: root
          MYSQL_DATABASE: blog
          MYSQL_USER: laravel
          MYSQL_PASSWORD: laravel
        ports:
          - "6306:3306"
```

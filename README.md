# nginx
version: '3'
services:
    databases_test:
      image: mysql
      ports:
      - "3307:3306"
      environment:
      - MYSQL_ROOT_PASSWORD=password
      - MYSQL_USER=user
      - MYSQL_PASSWORD=password
      - MYSQL_DATABASE=demodb
    web_test:
      image: nginx

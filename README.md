# Docker Nginx + PHP

一个使用 Docker 构建 Nginx 和 PHP 环境的项目。

## 项目简介

该项目提供了一个简单的 Docker 配置，用于快速搭建 Nginx 和 PHP 的开发环境。通过 Docker Compose，可以轻松启动 Nginx 和 PHP 服务，并支持自定义配置。

## 环境依赖

- Docker
- Docker Compose v2

## 快速开始

编辑 docker-compose.yml 文件，修改相关配置，挂载相应目录。

必须要挂载以下目录：
- ./nginx.conf:/etc/nginx/nginx.conf
- ./conf.d:/etc/nginx/conf.d

项目目录
- {项目路径}:/var/www

```bash
git clone https://github.com/mr-money/docker-nginx-php.git
cd docker-nginx-php

docker-compose up -d
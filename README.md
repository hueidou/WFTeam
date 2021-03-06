# WFTeam

![logo](https://raw.githubusercontent.com/hueidou/WFTeam/master/public/img/logo.png)

> A assistant for wanfang team

[![Build Status](https://travis-ci.org/hueidou/WFTeam.svg?branch=travis)](https://travis-ci.org/hueidou/WFTeam)
[![dependencies Status](https://david-dm.org/hueidou/wfteam/status.svg)](https://david-dm.org/hueidou/wfteam)
[![devDependencies Status](https://david-dm.org/hueidou/wfteam/dev-status.svg)](https://david-dm.org/hueidou/wfteam?type=dev)

## 开发

``` bash
# web
cd WFTeam

# install dependencies
npm install

# Compiles and hot-reloads for development
npm run serve

# Compiles and minifies for production
npm run build

# Run your tests
npm run test

# Lints and fixes files
npm run lint
```

``` bash
# 设置MongoDB环境变量
export MONGODB_CONNECTION=127.0.0.1:27017/wfteam

# server
cd server

# install dependencies
npm install

# serve with hot reload at localhost:8000
npm start
```

## Swagger

``` bash
# https://www.npmjs.com/package/swagger

# start the project(restart on changes)
swagger project start

# open Swagger editor for this project
swagger project edit
```

## 构建&部署

``` bash
# build
cd WFTeam
docker build -f Dockerfile -t wfteam:latest .

# deploy & run
docker run --name wfteam -p 8000:8000 -e "MONGODB_CONNECTION=127.0.0.1:27017/wfteam" -d wfteam:latest
docker start wfteam
```

## 其他

建议使用淘宝NPM源：

``` bash
npm config set registry https://registry.npm.taobao.org
```

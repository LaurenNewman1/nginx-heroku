## Run nginx on Heroku Cedar Stack

Inspired by https://github.com/adamwiggins/nginx-as-heroku-app

This repo contains the following (latest versions as of 5/7/12)

    nginx-1.2.0
    openssl-1.0.1b
    pcre-8.30
    zlib-1.2.7
    nginx_substitutions_filter


## Run locally

    ./configure
    make
    foreman start

## Deploy to Heroku

    heroku create -s cedar --buildpack https://github.com/heroku/heroku-buildpack-c
    git push heroku master
    heroku open
    heroku logs


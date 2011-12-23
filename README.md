Heroku buildpack: liquidsoap
============================

This is a [Heroku buildpack](http://devcenter.heroku.com/articles/buildpack) for liquidsoap apps.

Usage
-----

Example usage:

    $ ls
    Procfile  app.liq

    $ heroku create --stack cedar --buildpack http://github.com/savonet/heroku-buildpack-liquidsoap.git

    $ git push heroku master
    ...
    -----> Heroku receiving push
    -----> Fetching custom buildpack
    -----> liquidsoap app detected
    -----> Vendoring liquidsoap 1.0.0

The buildpack will detect your app as liquidsoap if it has the file `app.liq` in the root.  


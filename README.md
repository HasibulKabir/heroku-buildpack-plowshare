Heroku buildpack: heroku-buildpack-plowshare
======================

This buildpack is made by [Hasibul Kabir](https://github.com/HasibulKabir).
This is a [Heroku buildpack](http://devcenter.heroku.com/articles/buildpacks)
for adding [Plowshare](https://github.com/mcrapet/plowshare) to your application.

Multipacks
----------

The easiest way to do this is with a [multipack](https://github.com/ddollar/heroku-buildpack-multi),
where this is just one of the buildpacks you'll be working with.

    $ cat .buildpacks
    git://github.com/hasibulkabir/heroku-buildpack-plowshare.git
    
    $ heroku config:add BUILDPACK_URL=git://github.com/ddollar/heroku-buildpack-multi.git

By this you can use plowshare in your application.

### Another method
    heroku config:add BUILDPACK_URL=git://github.com/HasibulKabir/heroku-buildpack-plowshare.git
    
### You have to use this command on heroku application commandline
    plowmod --install
    

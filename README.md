# dev-dyno
A Heroku app to, hopefully, provide development environment on a one-off dyno

## Deploy
```
$ hreoku create
$ heroku buildpack:set https://github.com/heroku/heroku-buildpack-multi.git
$ git push heroku master
```

To play aroud, you may sometimes have to do the following:

```
$ heroku config:unset BUILDPACK_URL
```

```
$ git rm .buildpacks
$ git commit
```

```
$ heroku plugins:install https://github.com/heroku/heroku-repo.git
$ heroku repo:purge_cache
```

## Use
```
$ heroku run bash
~ $ vim.nox test.txt
```

## Todo
- update-alternatives

# dev-dyno
A Heroku app to, hopefully, provide development environment on a one-off dyno

## Deploy
```
$ hreoku create
$ heroku config:add BUILDPACK_URL=https://github.com/ddollar/heroku-buildpack-multi.git
$ git push heroku master
```

## Use
```
$ heroku run bash
~ $ vim.nox test.txt
```

## Todo
- update-alternatives

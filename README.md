# dev-dyno
A Heroku app to, hopefully, provide development environment on a one-off dyno

## Deploy
```
$ hreoku create
$ heroku buildpack:set https://github.com/heroku/heroku-buildpack-multi.git
$ git push heroku master
```

## Use
```
$ heroku run bash
~ $ vim.nox test.txt
```

## Todo
- update-alternatives

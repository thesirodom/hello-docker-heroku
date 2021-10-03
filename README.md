# Hello-docker-heroku

initialize postgres and python web-app (flask) containers on heroku

## Installation

Log-in to heroku account
```sh
heroku login
```

Sign into Container Registry.
```sh
heroku container:login
```

Remote to heroku server.
```sh
git init
heroku git:remote -a <your_app_name>
```

Build and push images (web, db)
```sh
heroku container:push web db --recursive
```

# Test
```sh
heroku ps
```

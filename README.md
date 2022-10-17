# R7 view component

## Running your App

The simplest way to start this up is by using [docker-compose](https://docs.docker.com/compose/):

```bash
docker-compose up
```

```
rails db:setup
rails db:migrate
rails server
```

Open your browser on [localhost:3000](http://localhost:3000).

## Development

This app was generated using [Klueless - RailsAppGenerator](https://github.com/klueless-io/rails_app_generator) - there are tons of little tweaks to simplify your development workflow.

For more details refer to the [Documentation](https://github.com/klueless-io/rails_app_generator)

## Deployment

Deploy this application using Capistrano. Make sure you have a server set up and edit [deploy.rb](./config/deploy.rb) and [config/production.rb](./config/deploy/production.rb).

``` ruby
# deploy.rb
set :repo_url, "git@github.com:user/your-project.git"

# production.rb
server "myserver.com", user: "deploy", roles: %w{app db web}
```

Then run:

```bash
cap production deploy
```

For more information on how to prepare a server for deployment you can follow [this guide](https://gorails.com/deploy/ubuntu/20.04).

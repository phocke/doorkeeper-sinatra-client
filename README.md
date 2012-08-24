# Doorkeeper Sinatra Client

This app is an example of OAuth 2 client. It was built in order to test the [doorkeeper provider example](http://doorkeeper-provider.herokuapp.com/). It uses [oauth2](https://github.com/intridea/oauth2) and [sinatra](http://www.sinatrarb.com/) gems. Check out the [live app here](http://doorkeeper-sinatra.herokuapp.com/). The source code is, as always, [available on GitHub](https://github.com/applicake/doorkeeper-sinatra-client).

## About Doorkeeper Gem

For more information [about the gem](https://github.com/applicake/doorkeeper), [documentation](https://github.com/applicake/doorkeeper#readme), [wiki](https://github.com/applicake/doorkeeper/wiki/_pages) and another resources, check out the project [on GitHub](https://github.com/applicake/doorkeeper).

## Installation

First clone the [repository from GitHub](https://github.com/applicake/doorkeeper-sinatra-client):

    git clone git://github.com/applicake/doorkeeper-sinatra-client.git

Install all dependencies with:

    bundle install

## Configuration

### Client application

If you have your own provider or you are using [this example](http://doorkeeper-provider.herokuapp.com/), you'll need to create a new client for this application. Make sure to append the `/callback` to the `redirect uri` (e.g. `http://localhost:9393/callback`).

### Environment variables

You just need to 

		mv env.rb.example to env.rb

If you use seed.rb in ideonetapp they will work together, as the app secret and app id are the same. 

## Start the server

Fire up the server with:

    rackup config.ru

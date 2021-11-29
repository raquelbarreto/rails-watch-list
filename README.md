# rails-watch-list

RailsWatchList is a platform where users can create lists of movies, to share with friends.

The following third party services are used by this app:
- [Cloudinary](https://cloudinary.com/)
- [MapBox](https://www.mapbox.com/)

# Development

This is a Ruby on Rails project. In order to run it locally, ensure you have installed:

- Correct Ruby version (see [.ruby-version](./.ruby-version))
- [PostgreSQL](https://www.postgresql.org/download/)

## Credentials

Ensure you have an account with Cloudinary and MapBox, then create a local `.env` file with your credentials.
The file expects one credential for each service, like:

```
$ cat .env
CLOUDINARY_URL=cloudinary://foo:bar
MAPBOX_API_KEY=foobar
```

## Database Setup

On the first local run, setup your database and seed it:
```
bundle exec rails db:setup
bundle exec rails db:seed
```

## Run the server

```
bundle exec rails s
```

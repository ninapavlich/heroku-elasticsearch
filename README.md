# ElasticSearch on Heroku

This simple Java application is an ElasticSearch server.

It uses Amazon S3 for index persistience.

## Deploy in Seconds

Quite simple.

    $ git clone https://github.com/kennethreitz/heroku-elasticsearch.git
    $ heroku create
    $ heroku config:set AWS_ACCESS_KEY=:key AWS_SECRET_KEY=:key S3_BUCKET=:bucket
    $ git push heroku master

That's it!

## Considerations

- There is no HTTP authentication. Your index is open for the world to read/write.
- The Elastic Search S3 backend is deprecated.

## Based On

This project is based on the work by [jordansissel](https://github.com/jordansissel/elasticsearch-on-heroku).

# Infrastructure

The project relies entirely on `AWS` services.

`Elastic beanstalk` is used to host the backend API while the postgres database is hosted on `AWS RSD`.

The client and the image assets are hosted on two different `S3 buckets`. The one hosting the static front end is enable fr static file serving, the other is a regular object storage
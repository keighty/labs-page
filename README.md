## Scaffold for quick static sites hosted on AWS

* requires [aws command line toolkit](https://aws.amazon.com/cli/)
* requires administrative user credentials for an AWS S3 instance (follow the instructions [here](http://docs.aws.amazon.com/gettingstarted/latest/swh/setting-up.html))

### Create an aws bucket to hold the site

```bash
./manage.sh create bucket.name
```

### Deploy the site

```bash
./manage.sh deploy bucket.name
```

### View the site

Go to http://bucket.name.s3-website-us-east-1.amazonaws.com .

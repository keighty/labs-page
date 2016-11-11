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

### Example

```bash
$ scaffold ./manage.sh create static.scaffold
make_bucket: s3://static.scaffold/
Website endpoint is: http://static.scaffold.s3-website-us-east-1.amazonaws.com
$ scaffold ./manage.sh deploy static.scaffold
s3://static.scaffold
upload: Documents/projects/scaffold/public/stylesheets/index.css to s3://static.scaffold/stylesheets/index.css
upload: Documents/projects/scaffold/public/app.js to s3://static.scaffold/app.js
upload: Documents/projects/scaffold/public/index.html to s3://static.scaffold/index.html
upload: Documents/projects/scaffold/public/favicon.ico to s3://static.scaffold/favicon.ico
upload: Documents/projects/scaffold/public/images/HeroImage.jpg to s3://static.scaffold/images/HeroImage.jpg
upload: Documents/projects/scaffold/public/vendor.js to s3://static.scaffold/vendor.js
View the site at http://static.scaffold.s3-website-us-east-1.amazonaws.com
```

[http://static.scaffold.s3-website-us-east-1.amazonaws.com/](http://static.scaffold.s3-website-us-east-1.amazonaws.com/)

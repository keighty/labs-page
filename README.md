## Scaffold for quick static sites hosted on AWS

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

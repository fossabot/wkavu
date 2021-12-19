# wkavu

![GitHub Workflow Status (branch)](https://img.shields.io/github/workflow/status/htynkn/wkavu/Rust/master)
![Docker Image Size (tag)](https://img.shields.io/docker/image-size/htynkn/wkavu/latest)
![Docker Pulls](https://img.shields.io/docker/pulls/htynkn/wkavu)

A simple (also minimal) torznab protocol implement which can work with sonarr.

Put http://your-ip:8000/ in settings and leave anything in api key.

## Docker

### pull

```
docker pull htynkn/wkavu
```

### create

```
docker run -d --name wkavu --privileged -v /mnt/appdata/wkavu:/data -e DB_URL=sqlite:///data/db.db -p 8991:8000 htynkn/wkavu
```

Docker image tested with TNAS F4-221
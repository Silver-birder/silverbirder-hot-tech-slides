# Docker Run

```
$ docker build -t tech-slide-app-batch:0.0.1 .
$ docker run -v <GOOGLE_APPLICATION_CREDENTIALS_PATH>:/usr/src/app/sa.json  -v $(pwd)/.env:/usr/src/app/.env --rm tech-slide-app-batch:0.0.1
```

# Build&Deploy

```
$ gcloud builds submit --tag gcr.io/silverbirder-hot-tech-slides/tech-slide-app-batch
$ gcloud run deploy --image gcr.io/silverbirder-hot-tech-slides/tech-slide-app-batch
```
#Google Function Example
## HTTP Functions testing
https://cloud.google.com/functions/docs/writing/http
## How to run emulator on your local machine
https://cloud.google.com/functions/docs/emulator

## deploy to Google Cloud
```
gsutil mb gs://gcf_http_staging
cd ~/gcf_http
gcloud beta functions deploy helloWorld --stage-bucket  gcf_http_staging --trigger-http
```
```
Copying file:///var/folders/wt/h0h1vm010551ds2_tk9dc3sm0000gn/T/tmpGgUnhu/fun.zip [Content-Type=application/zip]...
- [1 files][ 19.5 KiB/ 19.5 KiB]
Operation completed over 1 objects/19.5 KiB.
Deploying function (may take a while - up to 2 minutes)...done.
availableMemoryMb: 256
entryPoint: helloWorld
httpsTrigger:
  url: https://us-central1-winter-wonder-647.cloudfunctions.net/helloWorld
labels:
  deployment-tool: cli-gcloud
latestOperation: operations/d2ludGVyLXdvbmRlci02NDcvdXMtY2VudHJhbDEvaGVsbG9Xb3JsZC9EajRVNHNWY0E1UQ
name: projects/winter-wonder-647/locations/us-central1/functions/helloWorld
serviceAccount: winter-wonder-647@appspot.gserviceaccount.com
sourceArchiveUrl: gs://gcf_http_staging/us-central1-helloWorld-vrbhrkncnvcy.zip
status: READY
timeout: 60s
updateTime: '2017-09-14T11:31:36Z'
versionId: '1'
```

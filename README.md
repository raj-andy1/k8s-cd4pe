### Usage

#### Required for persistant volumes:

```
gcloud compute disks create --size 50GB pipelines-cd4pe-artifactory --project YOUR_GCLOUD_PROJECT --zone YOUR_K8S_ZONE

gcloud compute disks create --size 50GB pipelines-cd4pe-mysql --project YOUR_GCLOUD_PROJECT --zone YOUR_K8S_ZONE
```

#### Installation:

Put this in a kubernetes cluster by cloning the project.

From the project directory first run `kubectl create namespace cd4pe`

and then run `kubectl create -R -f .`

## Pipeline Chart
Creates and starts pipleline using Tekton that pulls source code and uses s2i to create an image that it pushes to an ImageStream


## ** REQUIRED ** Create docker config

Create docker config secret running the following:

```
oc create secret docker-registry dockerconfigjson \
  --docker-username=jland \
  --docker-password=pass113 \
  --docker-email=jland@acme.com
```
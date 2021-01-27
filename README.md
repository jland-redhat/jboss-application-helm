## Prerequisites

* Openshift 4.4+
* Opensshift Piplelines(tekton)


## Deployment

#### Update Helm Dependencies (Must be run every time the pipeline is updated)

```
helm dependency update
```

#### Install Helm Chart (First time installation)

```
helm install <RELEASE_NAME> . 
```

### Update Existing Helm Chart


```
helm upgrade <TEMPLATE_NAME> .
```

## Branch Notes

Intended to be used a more basic argo release example.

## ** REQUIRED ** Create docker config

Create docker config secret running the following:

```
oc create secret docker-registry dockerconfigjson \
  --docker-username=jland \
  --docker-password=pass113 \
  --docker-email=jland@acme.com
```
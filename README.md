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
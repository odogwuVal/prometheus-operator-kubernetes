# prometheus-operator-kubernetes
Everything prometheus
##### NB: When deploying your applications to custom namespaces eg: "staging", set a label
##### monitoring: prometheus{same with what you have set on your monitoring namespace}
##### this enables you create service monitors and pod monitors in the same namespace.
##### you can also create the pod and service monitors in the monitoring namespace if you prefer that approach. 
```
    apiVersion: v1
    kind: Namespace
    metadata:
        name: monitoring
        labels:
            monitoring: prometheus
```

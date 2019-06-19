# Single-pod-graylog-with-PVC
single Statefulset graylog cluster kubernetes setup with PVC


## Change value in value.yaml

add the value in `value.yaml` file.

All deployment are stateful set with PVC.

```
helm install --name graylog .
```

Table of content 

| Statefulsets        | Image version           | PVC mountpath  |
| ------------- |:-------------:| -----:|
| Elasticsearch      | elasticsearch:6.5.0 | /usr/share/elasticsearch/data |
| Graylog      | graylog/graylog:3.0.1      |   /usr/share/graylog/data/journal |
| MongoDB | mongo:3      |    /data/db |

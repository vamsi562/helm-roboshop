## Helm commands

```
    helm install <chart_name> .
```

```
    helm uninstall <chart_name>
```

```
    helm upgrade <chart_name> .
```

```
    helm list
```

```
    helm history <chart_name> - we can see all revisions of a chart
```

```
    helm upgrade <chart_name> . --key "value"
    # here for key in chart yaml its value can be replaced with command line
```

```
    helm rollback <chart_name> <revision>
    # roll back to required version
```

# roboshop helm command
```
    for i in mongodb redis rabbitmq mysql catalogue cart user shipping payment frontend; do cd $i && helm install $i . && cd ..; done
```
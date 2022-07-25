## References 
- [https://github.com/aquasecurity/kube-hunter](https://github.com/aquasecurity/kube-bench)

### Need to set schedule time to run kube-bench in ivari-sandbox-values.yaml
```yaml
image:
  registry: aquasec
  repository: kube-bench
  tag: latest
  pullPolicy: IfNotPresent

imagePullSecrets: []
nameOverride: ""
fullnameOverride: ""

schedule: "*/5 * * * *"  # run at every 5 minuits
```

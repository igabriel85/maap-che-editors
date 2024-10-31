# Getting started samples

In the `maap_full_samples.json` you can find all gettings tarted workspaces for Ecllipse Che.

In order to add them to your Eclipse Che instance, you can use the following command:

```bash
kubectl create configmap getting-started-samples --from-file=maap_full_sample.json -n eclipse-che
```

```bash
kubectl label configmap getting-started-samples app.kubernetes.io/part-of=che.eclipse.org app.kubernetes.io/component=getting-started-samples -n eclipse-che
```
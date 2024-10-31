# Setup of Custom Jupyter IDE in Eclipse che 7.x

Custom IDE definition are to be added using configMap in the che-server deployment. 
The plugin registry is to be deprecated in future versions.

```bash
kubectl create configmap my-editor-polinsar --from-file=che-editor-polinsar.yaml  -n eclipse-che
```

```bash
kubectl label configmap my-editor-polinsar app.kubernetes.io/part-of=che.eclipse.org app.kubernetes.io/component=editor-definition -n eclipse-che
```

For more details please consult the official Eclipse Che [documentation](https://eclipse.dev/che/docs/stable/administration-guide/configuring-editors-definitions/)


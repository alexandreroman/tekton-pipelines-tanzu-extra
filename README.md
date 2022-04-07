# Tekton Pipelines - Carvel package for Tanzu

This project defines a [Carvel package](https://carvel.dev/kapp-controller/docs/latest/packaging/)
for [Tekton Pipelines](https://tekton.dev/docs/pipelines), a powerful and flexible open-source framework
for creating CI/CD systems for Kubernetes clusters.

Please note this package only includes the [Tekton Pipelines](https://github.com/tektoncd/pipeline) module.

## How to use it?

This package is part of the
[Tanzu Extra package repository](https://github.com/alexandreroman/tanzu-extra-repo).
Please refer to this page for installation instructions.

Here are the configuration parameters for this package:

| Key                                   | Description                           |
|---------------------------------------|---------------------------------------|
| tekton.pipelines.pvc.size             | Size for Persistent Volume requests   |
| tekton.pipelines.pvc.storageClassName | Storage class name                    |

Configuration example:

```yaml
tekton:
  pipelines:
    pvc:
      size: 5Gi
      storageClassName: default
```

## Contribute

Contributions are always welcome!

Feel free to open issues & send PR.

## License

Copyright &copy; 2022 [VMware, Inc. or its affiliates](https://vmware.com).

This project is licensed under the [Apache Software License version 2.0](https://www.apache.org/licenses/LICENSE-2.0).

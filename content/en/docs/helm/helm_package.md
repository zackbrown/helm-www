---
title: "Helm Package"
weight: 23
---

## helm package

package a chart directory into a chart archive

### Synopsis



This command packages a chart into a versioned chart archive file. If a path
is given, this will look at that path for a chart (which must contain a
Chart.yaml file) and then package that directory.

If no path is given, this will look in the present working directory for a
Chart.yaml file, and (if found) build the current directory into a chart.

Versioned chart archives are used by Helm package repositories.


```
helm package [flags] [CHART_PATH] [...]
```

### Options

```
  -u, --dependency-update    update dependencies from "requirements.yaml" to dir "charts/" before packaging
  -d, --destination string   location to write the chart. (default ".")
      --key string           name of the key to use when signing. Used if --sign is true
      --keyring string       location of a public keyring (default "/Users/roflynnc/.gnupg/pubring.gpg")
      --save                 save packaged chart to local chart repository (default true)
      --sign                 use a PGP private key to sign this package
      --version string       set the version on the chart to this semver version
```

### Options inherited from parent commands

```
      --debug                     enable verbose output
      --home string               location of your Helm config. Overrides $HELM_HOME (default "/Users/roflynnc/.helm")
      --host string               address of Tiller. Overrides $HELM_HOST
      --kube-context string       name of the kubeconfig context to use
      --tiller-namespace string   namespace of Tiller (default "kube-system")
```

### SEE ALSO
* [helm](../helm)	 - The Helm package manager for Kubernetes.

###### Auto generated by spf13/cobra on 13-Jan-2020

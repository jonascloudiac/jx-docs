---
date: 2019-07-03T03:57:13Z
title: "jx step e2e label"
slug: jx_step_e2e_label
url: /commands/jx_step_e2e_label/
---
## jx step e2e label

Removes unused e2e clusters

### Synopsis

Add a label to a cluster used for e2e testing

```
jx step e2e label [flags]
```

### Examples

```
  # Mark a cluster to not be deleted by the gc
  jx step e2e label --keep clusterName
  
  # Mark a cluster to be deleted by the gc
  jx step e2e label --delete clusterName
```

### Options

```
  -d, --delete              Add a label top mark cluster for deletion
  -h, --help                help for label
  -k, --keep                Add a label top mark cluster for non deletion
  -p, --project-id string   Google Project ID to delete cluster from
      --region string       GKE region to use. Default: europe-west1-c (default "europe-west1-c")
```

### Options inherited from parent commands

```
  -b, --batch-mode                Runs in batch mode without prompting for user input (default true)
      --config-file string        Configuration file used for installation
      --install-dependencies      Enables automatic dependencies installation when required
      --no-brew                   Disables brew package manager on MacOS when installing binary dependencies
      --skip-auth-secrets-merge   Skips merging the secrets from local files with the secrets from Kubernetes cluster
      --verbose                   Enables verbose output
```

### SEE ALSO

* [jx step e2e](/commands/jx_step_e2e/)	 - e2e [command]

###### Auto generated by spf13/cobra on 3-Jul-2019
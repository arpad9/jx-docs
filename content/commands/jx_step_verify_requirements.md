---
date: 2019-08-07T10:12:06Z
title: "jx step verify requirements"
slug: jx_step_verify_requirements
url: /commands/jx_step_verify_requirements/
---
## jx step verify requirements

Verifies all the helm requirements.yaml files have a version number populated from the Version Stream

### Synopsis

Verifies all the helm requirements.yaml files have a version number populated from the Version Stream.
  
See Also: 

  * jx create project : https://jenkins-x.io/commands/jx_create_project

```
jx step verify requirements [flags]
```

### Examples

```
  Verifies all the helm requirements.yaml files have a version number populated from the Version Stream
  
  # verify packages and fail if any are not valid:
  jx step verify packages
  
  # override the error if the 'jx' binary is out of range (e.g. for development)
  export JX_DISABLE_VERIFY_JX="true"
  jx step verify packages
```

### Options

```
  -d, --dir string   the directory to recursively look for 'requirements.yaml' files (default ".")
  -h, --help         help for requirements
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

* [jx step verify](/commands/jx_step_verify/)	 - verify [command]

###### Auto generated by spf13/cobra on 7-Aug-2019
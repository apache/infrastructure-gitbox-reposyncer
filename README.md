# infrastructure-gitbox-reposyncer
ASF Infra GitBox repository sync mechanism

This service runs on GitBox v2 and synchronizes from GitHub to GitBox via AWS SQS events.
It is installed by defining the following pipservice setup in the node's YAML:

~~~yaml
pipservice:
  gitbox-reposyncer:
    tag: master
~~~

Furthermore, there is a configuration defined in EYAML (see sample config also).

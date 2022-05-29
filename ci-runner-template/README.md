# ci-runner


Go to config ruuner file:
/etc/gitlab-runner/config.toml


#### Daemon socket option
volumes = ["/var/run/docker.sock:/var/run/docker.sock","/cache"]

#### fixed host in local runner server
extra_hosts = ["{gitlab_name}:x.x.x.x"]

#### how to fixed pull docker every jobs
set pull_policy="if-not-present" 

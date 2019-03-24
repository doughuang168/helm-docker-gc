# helm-docker-gc
Helm Chart deploy as DaemonSet to perform GC

# Docker container
Modify Spotif Helm Chart to use docker image clockworksoul/docker-gc-cron

# Dry run and debug
helm --kube-context  <clusterenv> install --name docker-gc-cron --namespace default --dry-run --debug ./helm-docker-gc

# Install
helm --kube-context  <clusterenv> install --name docker-gc-cron --namespace default --debug ./helm-docker-gc

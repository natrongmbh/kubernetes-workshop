# DaemonSets
A DaemonSet is almost identical to a normal Deployment. The difference is that it makes sure that exactly one Pod is running on every (or some specified) Node. When a new Node is added, the DaemonSet automatically deploys a Pod on the new Node if its selector matches. When the DaemonSet is deleted, all related Pods are deleted.

One obvious use case for a DaemonSet is some kind of agent or daemon to e.g. grab logs from each Node of the cluster (e.g., Fluentd, Logstash or a Splunk forwarder).

More information about DaemonSet can be found in the [Kubernetes DaemonSet Documentation](https://kubernetes.io/docs/concepts/workloads/controllers/daemonset/).

# NOTE

This script is only to be invoked against CDK clusters that have been upgraded to 1.10 or higher.

## Instructions

Download this script:

```
$ wget https://raw.githubusercontent.com/juju-solutions/cdk-etcd-2to3/master/migrate
```

Make it executable:
```
$ chmod +x migrate
```

Execute it:

```
$ ./migrate
· Waiting for etcd units to be active and idle...
· Acquiring configured version of etcd...
· Upgrading etcd to version 3.0/stable from 2.3/stable.
· Waiting for etcd upgrade to 3.0/stable............................................................
· Waiting for etcd units to be active and idle....................................................
· Waiting for etcd cluster convergence...
· Stopping all Kubernetes api servers...
· Waiting for etcd cluster convergence...
· Stopping etcd...
· Migrating etcd/0...
· Migrating etcd/1...
· Migrating etcd/2...
· Starting etcd...
· Configuring storage-backend to etcd3...
· Waiting for all Kubernetes api servers to restart.......
· Done.
```

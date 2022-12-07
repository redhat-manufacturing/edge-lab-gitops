# Notes

This instance will not progress before you label nodes

```
oc label node cluster.ocs.openshift.io/openshift-storage="" --all

oc annotate sc ocs-storagecluster-cephfs storageclass.kubernetes.io/is-default-class="true"
```
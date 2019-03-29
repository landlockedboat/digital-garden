# Kubernetes

## Volumes

### PersistentVolume (PV)

An abstraction of the physical filesystem.

### PersistentVolumeClaim (PVC)

A reference to a `PV`. One `PVC` can only be assigned to a `PV`, but multiple pods can use the same `PVC`.

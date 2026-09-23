# Kubernetes Task

## Objective

Set up Minikube locally and explore Kubernetes namespaces using WSL2, Docker, VirtualBox, Minikube, and kubectl.

## Technologies Used

- Windows
- WSL2 with Ubuntu
- Docker Desktop
- VirtualBox
- Minikube v1.39.0
- kubectl
- Kubernetes v1.37.0

## Environment Setup

The following components were configured on the local system:

1. Enabled Intel Virtualization Technology in BIOS.
2. Installed and configured WSL2 with Ubuntu.
3. Installed Docker Desktop and enabled WSL2 integration.
4. Installed Oracle VirtualBox.
5. Installed Minikube v1.39.0.
6. Started a Minikube Kubernetes cluster using the VirtualBox driver.
7. Verified the Kubernetes control plane and node status using Minikube and kubectl.

## Minikube Cluster

Minikube was started using the VirtualBox driver:

```text
minikube start --driver=virtualbox --no-vtx-check

```

The cluster was verified using Minikube and kubectl.

Verified components included:

- Control Plane
- Host
- Kubelet
- API Server
- Kubeconfig
- Kubernetes node

## Kubernetes Namespaces

The default Kubernetes namespaces were verified.

Two custom namespaces were successfully created:

- dev
- test

The namespaces were verified using:

```text
kubectl get namespaces
```

Both custom namespaces showed an Active status.

## Namespace Commands

Create namespaces:

```text
kubectl create namespace dev
kubectl create namespace test
```

List namespaces:

```text
kubectl get namespaces
```

Explore namespaces:

```text
kubectl describe namespace dev
kubectl describe namespace test
```

## Result

A local Minikube Kubernetes cluster was successfully configured using VirtualBox. Kubernetes namespaces were explored, and custom namespaces named dev and test were successfully created and verified.

## Conclusion

This task demonstrated the basic setup and operation of a local Kubernetes environment using WSL2, Docker, VirtualBox, Minikube, and kubectl. The Kubernetes cluster was successfully started and custom namespaces were created and verified.```

The cluster was verified using Minikube and kubectl.

Verified components included:

- Control Plane
- Host
- Kubelet
- API Server
- Kubeconfig
- Kubernetes node

## Kubernetes Namespaces

The default Kubernetes namespaces were verified.

Two custom namespaces were successfully created:

- dev
- test

The namespaces were verified using:

```text
kubectl get namespaces
```

Both custom namespaces showed an Active status.

## Namespace Commands

Create namespaces:

```text
kubectl create namespace dev
kubectl create namespace test
```

List namespaces:

```text
kubectl get namespaces
```

Explore namespaces:

```text
kubectl describe namespace dev
kubectl describe namespace test
```

## Result

A local Minikube Kubernetes cluster was successfully configured using VirtualBox. Kubernetes namespaces were explored, and custom namespaces named dev and test were successfully created and verified.

## Conclusion

This task demonstrated the basic setup and operation of a local Kubernetes environment using WSL2, Docker, VirtualBox, Minikube, and kubectl. The Kubernetes cluster was successfully started and custom namespaces were created and verified.

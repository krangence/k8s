# k8s

This repository contains the Kubernetes configuration files managed by GitOps, specifically [Flux](https://fluxcd.io/) and is a work is progress / under development.

Using a combination of a variety of resources such as [Vault](https://www.vaultproject.io/), [ArgoCD](https://argo-cd.readthedocs.io/en/stable/), [SOPS](https://github.com/mozilla/sops), [Age](https://github.com/FiloSottile/age)


## TODO

- [x] Folder Structure Setup
- [ ] Secret Management - SOPS & Age
- [ ] Flux Setup / Deployment
- [ ] Ingress
- [ ] Security
- [ ] CI / CD
- [ ] Backups
- [ ] Monitoring & Alerting

## 📂 Repository structure



## Setup

### Prerequisites for Cluster:
 
**CSI Driver** - Access to remote storage via a CIFs Share. To install use one of the following depending on Host Node OS:

    ```
    Ubuntu: `sudo apt-get install -y cifs-utils`
    CentOS: `yum -y install cifs-utils`
    ```

### 💾 Storage

Remote Storage: 
This functionality requires the CSI-Driver to be install from the `Prerequisites for Cluster:` section. Once install will provide the ability of the cluster to reference remote storage options such as [Hetzner's Storage Boxes](https://www.hetzner.com/storage/storage-box), which are scaleable options for remote storage.

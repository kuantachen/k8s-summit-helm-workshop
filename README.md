# k8s-summit-helm-workshop
## Usage

[Helm](https://helm.sh) must be installed to use the charts.  Please refer to
Helm's [documentation](https://helm.sh/docs) to get started.

Once Helm has been set up correctly, add the repo as follows:

    helm repo add k8s-summit-helm-workshop https://kuantachen.github.io/k8s-summit-helm-workshop

If you had already added this repo earlier, run `helm repo update` to retrieve the latest versions of the packages.  You can then run `helm search repo <alias>` to see the charts.

To install the myapi chart:

    helm install kuantachen-myapi k8s-summit-helm-workshop/myapi

To uninstall the chart:

    helm delete k8s-summit-helm-workshop/myapi

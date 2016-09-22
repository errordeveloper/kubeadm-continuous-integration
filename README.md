The CI is running on GKE.

If you had been added to `kubeadm` GCP project, you will need to do this to get your `kubeconfig` file:

```
export KUBECONFIG="$(pwd)/kubeconfig"
gcloud container clusters --project kubeadm --zone europe-west1-d get-credentials kubeadm-continuous-integration
```

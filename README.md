#This repository contains a Helm chart for deploying a Redis cluster.

### Prerequisites

- Helm 3.x on your local
- A running Kubernetes cluster

### Installation

1. Clone this repository:
    ```bash
    git clone https://github.com/mahmoodr/RedisCluster_HelmChart.git
    cd ./RedisCluster_HelmChart
    ```

2. Install the Helm chart:
    ```bash
    helm install redis-cluster ./RedisCluster_HelmChart
    ```

    This will install the Redis cluster in your Kubernetes cluster using the default values.

3. Customize your installation (optional):
    You can customize the installation by modifying the `values.yaml` file or by providing your own values file during installation:
    ```bash
    helm install redis-cluster ./RedisCluster_HelmChart -f custom-values.yaml
    ```

4. Upgrade the chart:
    If you make changes to the `values.yaml` or the chart itself, you can upgrade the release:
    ```bash
    helm upgrade redis-cluster ./RedisCluster_HelmChart
    ```

5. Uninstall the chart:
    To uninstall and delete the Redis cluster:
    ```bash
    helm uninstall redis-cluster
    ```

## Contribution
Feel free to submit issues and pull requests to help improve this Helm chart.



# ML-Platform

## JupyterHub
The jupyterHub folder contains:
  - A DockerFile for the creation of a Docker image for the creating of a all-spark-notebook that includes the Azure Data Lake dependecies.
  - A Config file which is passes to the Jupyter/Jupyterhub public helm chart at install. 
  


### Installing the Chart

Follow the guide on: https://zero-to-jupyterhub.readthedocs.io/en/v0.4-doc/setup-jupyterhub.html#install-jupyterhub 

Create the secrets and put them into your config.yaml file

To install the chart with the release name `jupyterhub`:

```bash
$  helm repo add jupyterhub https://jupyterhub.github.io/helm-chart/
$  helm repo update
$  helm install --version 0.7.0 --name=jhub --values config.yaml jupyterhub/jupyterhub 
```


## Spark
The Spark folder, is a Spark Helm chart.
For more information, see the chart. 

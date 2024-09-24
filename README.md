# Helmchart for generic python application

[![Packahe Helm Chart](https://github.com/zcsadmin/ml-pyhchart-helmchart/actions/workflows/helm-package.yml/badge.svg)](https://github.com/zcsadmin/ml-pyhchart-helmchart/actions/workflows/helm-package.yml)

[![Push Helm Chart to Artifact Registry](https://github.com/zcsadmin/ml-pyhchart-helmchart/actions/workflows/helm-push.yml/badge.svg)](https://github.com/zcsadmin/ml-pyhchart-helmchart/actions/workflows/helm-push.yml)


## Changelog

### 0.2.2 
Set container name for deployment.

### 0.2.1
Enhance secrets support.

### 0.2.0
Add support for secret values.

### 0.1.0
Initial chart release.

## Artifact Repository

`oci://europe-west1-docker.pkg.dev/ai-accounting-405809/ml-helm-charts/pyhchart`

List docker images from cli:
```bash
gcloud artifacts docker images list europe-west1-docker.pkg.dev/ai-accounting-405809/ml-helm-charts
```

## Example deploy

You need to download the chart locally and `appVersion` value in `Chart.yaml` file.
Also, you need a `values-app.yaml` file with the specific values for your application.
Then, you can install the application with the following command:
```bash
helm install YOUR_APP -f values-app.yaml .
```

## Useful links

 - [Artifact repository](https://console.cloud.google.com/artifacts/docker/ai-accounting-405809/europe-west1/ml-helm-charts/pyhchart?project=ai-accounting-405809)

# Description

This repository contains packaged charts from the [helloworld-chart](https://github.com/workload-assessment-openshift4/helm-examples/tree/main/helloworld-chart) in our helm-examples repository. It also contains a CRD for adding this repo to the developer catalog in Openshift.

## Adding new .tgz packages

1. Clone [this](https://github.com/workload-assessment-openshift4/helm-examples) repository.
2. Checkout this repository and navigate to the root directory.
3. `helm package <path-of-repo-in-first-step>/helloworld-chart`
4. `helm repo index . --url https://github.com/workload-assessment-openshift4/helm-releases`
5. Commit and push all changes.
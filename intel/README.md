# Intel managed distribution of Istio

Intel managed distribution of Istio is a project aiming to showcase and integrate various Intel technologies into Istio and Envoy. The focus is in letting both upstream community and users know what Intel is working on, finding gaps in upstream project features in relation to hardware enablement, and testing and deploying Intel features for Istio service mesh.

## Features

* [TLS handshake acceleration with AVX512 (CryptoMB)](docs/CRYPTOMB.md)
* [TLS handshake acceleration with QAT2.0](docs/QAT.md)
* [HTTP data compression acceleration with QAT2.0](docs/QAT.md)
* [Private key protection with SGX](docs/SGX-mTLS.md)

## Supported versions
* Kubernetes v1.24
* Istio v1.15
* cert-manager v1.7 or later
* Linux kernel 5.18 or later
* Intel Device Plugins for Kubernetes v0.24

## Install

Use the follwoing command for basic installation:

```bash
istioctl install --set hub=docker.io/intel --set tag=1.15.1-intel.0

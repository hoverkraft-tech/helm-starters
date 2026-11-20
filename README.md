# 🚀 Hoverkraft-Tech Helm Starter Pack

[![License](https://img.shields.io/badge/License-MIT-blue.svg)](LICENSE)
[![Helm](https://img.shields.io/badge/Helm-v3-informational?logo=helm)](https://helm.sh/)
[![Kubernetes](https://img.shields.io/badge/Kubernetes-1.16+-blue?logo=kubernetes)](https://kubernetes.io/)

A comprehensive Helm starter pack for rapid application deployment on Kubernetes.
This repository is suposed to be used as an helm starter and provides a solid foundation with best practices, security defaults, and production-ready configurations.

## ✨ Features

- 🔧 **Production-ready templates** with security best practices
- 📊 **Horizontal Pod Autoscaling** support
- 🌐 **Ingress configuration** with TLS/SSL support
- 🔍 **Health checks** (liveness, readiness, startup probes)
- 🔐 **ServiceAccount** with configurable RBAC
- 📈 **Resource management** with presets and custom configurations
- 🧪 **CI/CD ready** with Chart Testing configuration
- 📋 **Comprehensive documentation** and examples
- 🔄 **Bitnami Common** library integration for enhanced functionality

## Usage

```sh
helm starter fetch https://github.com/hoverkraft-tech/helm-starters [version]
helm starter list
helm create myapp -p helm-starters/default
```

## Contributing

- We use [mise](https://mise.jdx.dev/) for tooling. You will need to install it.
- run the following commands :

```shell
mise trust
mise install
mise exec -- uv sync
helm plugin install https://github.com/jtyr/kubeconform-helm
prek install
```

### Running tests

You can run tests with mise commands:

```shell
mise run tests # run all tests
mise run <test name> # just run one test (ex: kubeconform)
```

---

Made with ❤️ by Hoverkraft-Tech
